# Visão Lógica

## Componentes Principais

- **Módulo de Autenticação**: Gerencia login, cadastro e permissões.
- **Módulo de Produtos**: Gerencia cadastro, atualização e exibição de produtos.
- **Módulo de Pedidos**: Gerencia criação, atualização e rastreamento de pedidos. É responsável por disponibilizar informações sobre o andamento do pedido, validar o estoque antes de confirmar o pedido e atualizar o estoque após a realização da compra.
- **Módulo de Pagamentos**: Integração com carteiras digitais e cartões. O pagamento só é liberado após a confirmação da entrega do produto.
- **Módulo Blockchain**: Interface para registro e consulta de eventos na blockchain.

## Comunicação entre Componentes

- Inicialmente, a comunicação entre módulos será realizada via REST API.

## Diagrama de Componentes

Veja o arquivo `diagrama_de_componentes.puml` na pasta `modelos_uml`.

## Fluxos Principais:  
### 1. Realizar Compra

1. Usuário seleciona produtos e inicia o pedido.
2. O Módulo de Pedidos valida o estoque dos produtos.
3. Pedido é criado e registrado na blockchain.
4. Usuário realiza o pagamento (Módulo de Pagamentos).
5. Pedido é atualizado conforme o andamento (envio, entrega), com eventos registrados na blockchain.
6. O pagamento é liberado ao vendedor somente após a confirmação da entrega.

### 2. Cadastro e Autenticação

1. Usuário acessa a interface de cadastro ou login.
2. Dados são enviados ao Módulo de Autenticação via REST API.
3. Para cadastro, o sistema valida dados e cria o usuário no banco de dados.
4. Para autenticação, as credenciais são verificadas e, se válidas, um token de acesso é gerado.
5. Usuário autenticado pode acessar funcionalidades restritas da plataforma.

### 3. Registro e Consulta de Transações na Blockchain

1. Sempre que uma ação crítica ocorre (criação de pedido, atualização de status, avaliação), o Backend/API envia um evento ao Módulo Blockchain.
2. O Módulo Blockchain registra o evento na blockchain, garantindo imutabilidade e rastreabilidade.
3. Para consulta, o Backend/API requisita ao Módulo Blockchain os dados históricos de transações ou eventos relacionados a um pedido.
4. As informações são retornadas ao usuário ou administrador, garantindo transparência e confiança no processo.

## Camadas

- **Apresentação**: Interface do usuário.
- **Aplicação**: Orquestração dos casos de uso.
- **Domínio**: Regras de negócio.
- **Infraestrutura**: Integrações externas (blockchain, banco de dados, pagamentos, transportadora).
