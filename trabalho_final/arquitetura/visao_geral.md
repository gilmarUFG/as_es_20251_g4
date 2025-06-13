# Visão Geral da Arquitetura

A plataforma é composta por módulos integrados que interagem entre si e com a blockchain, formando a base para um sistema seguro, rastreável e escalável.

## Módulos Principais

- **Frontend Web**: Interface para usuários e vendedores, responsável pela experiência do usuário, exibição de produtos, acompanhamento de pedidos e interação com o backend via REST API.
- **Backend/API**: Centraliza a lógica de negócio, autenticação, autorização, orquestração dos módulos de pedidos, produtos, pagamentos e integração com a blockchain.
- **Banco de Dados**: Armazena dados operacionais (usuários, produtos, pedidos, etc.) e serve de apoio para consultas rápidas e consistentes.
- **Blockchain**: Responsável pelo registro imutável de transações, avaliações, histórico de pedidos e eventos críticos do sistema, garantindo transparência e segurança.

## Integrações

- **Gateways de Pagamento**: Permitem transações com carteiras digitais e cartões.
- **Serviços de Autenticação de Terceiros**: Possibilitam login social ou autenticação federada.
- **Transportadoras**: Integração para rastreamento automático de entregas.

## Principais Fluxos

- **Cadastro e autenticação de usuários/vendedores**: Usuários criam contas e acessam a plataforma de forma segura.
- **Realização de compra**: Seleção de produtos, validação de estoque, criação do pedido, registro na blockchain, pagamento e acompanhamento do status.
- **Registro e consulta de transações na blockchain**: Todas as etapas críticas do pedido são registradas para garantir rastreabilidade.
- **Atualização e consulta de estoque e pedidos**: Estoque é validado e atualizado automaticamente a cada compra, e o usuário pode acompanhar o andamento do pedido em tempo real.

> Consulte os diagramas na pasta `diagramas` para uma visualização gráfica das interações entre os módulos.