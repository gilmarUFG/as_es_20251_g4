# Visão Geral da Arquitetura

A plataforma será composta por módulos integrados que interagem entre si e com a blockchain. Os principais módulos são:

- **Frontend Web**: Interface para usuários e vendedores.
- **Backend/API**: Lógica de negócio, autenticação, integração com blockchain.
- **Banco de Dados**: Armazenamento de dados não sensíveis e cache.
- **Blockchain**: Registro de transações, avaliações e histórico de pedidos.

O diagrama a seguir ilustra a interação entre os módulos (ver diagramas na pasta `diagramas`).

## Principais Fluxos
- Cadastro e autenticação de usuários/vendedores.
- Registro e consulta de transações na blockchain.
- Atualização e consulta de estoque e pedidos.