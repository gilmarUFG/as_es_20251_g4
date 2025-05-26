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

## Fluxo Principal: Realizar Compra

1. Usuário seleciona produtos e inicia o pedido.
2. O Módulo de Pedidos valida o estoque dos produtos.
3. Pedido é criado e registrado na blockchain.
4. Usuário realiza o pagamento (Módulo de Pagamentos).
5. Pedido é atualizado conforme o andamento (envio, entrega), com eventos registrados na blockchain.
6. O pagamento é liberado ao vendedor somente após a confirmação da entrega.

## Camadas

- **Apresentação**: Interface do usuário.
- **Aplicação**: Orquestração dos casos de uso.
- **Domínio**: Regras de negócio.
- **Infraestrutura**: Integrações externas (blockchain, banco de dados, pagamentos, transportadora).
