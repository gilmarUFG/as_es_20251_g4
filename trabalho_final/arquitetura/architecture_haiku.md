# E-commerce Blockchain Architecture Haiku

## Haiku

Blocos conectados,  
Confiança na cadeia,  
Fluxo transparente.

---

## Objetivo

- Prover uma plataforma de e-commerce segura, transparente e rastreável, utilizando blockchain para registrar eventos críticos e garantir confiança entre usuários.

---

## Requisitos Funcionais

- Cadastro e autenticação de usuários e vendedores.
- Exibição e busca de produtos.
- Realização de pedidos com validação e atualização automática de estoque.
- Pagamentos digitais (criptomoedas e cartões).
- Registro imutável de transações, avaliações e status de pedidos na blockchain.
- Consulta ao histórico de pedidos e avaliações.
- Integração futura com transportadoras e análise de dados.

---

## Restrições Técnicas

- Utilizar **React** para o frontend (SPA).
- Backend implementado em **.NET**.
- Banco de dados relacional **PostgreSQL** (Amazon RDS).
- Blockchain via **Amazon Managed Blockchain**.
- Comunicação entre módulos via **REST API**.
- Infraestrutura baseada em serviços gerenciados da **AWS**.
- Integração com gateways de pagamento e autenticação de terceiros.

---

## Atributos de Qualidade

- **Segurança**: Autenticação robusta, armazenamento seguro de dados sensíveis.
- **Transparência e rastreabilidade**: Blockchain como fonte de verdade.
- **Escalabilidade**: Arquitetura modular e uso de serviços gerenciados.
- **Evolução**: Pontos de extensão previstos para integrações futuras.
- **Usabilidade**: Interface intuitiva e responsiva.

---

## Decisões de Design

- Separação de camadas: apresentação, aplicação, domínio e infraestrutura.
- Modularização dos principais domínios: pedidos, produtos, pagamentos, autenticação, blockchain.
- Uso de REST API para comunicação interna e externa.
- PlantUML para documentação dos diagramas.
- Versionamento e documentação viva no repositório.

---

## Planos Futuros

- Integração com arquitetura lakehouse para análise avançada de dados.
- Migração de partes do backend para serverless (AWS Lambda).
- Ampliação das integrações com transportadoras e novos métodos de pagamento.
- Melhoria contínua da experiência do usuário e dos mecanismos de segurança.

---

## Referências

- [Definição dos Requisitos](../definicao_trabalho_final_g4.md)
- [Histórias de Usuário](https://github.com/gilmarUFG/rs_es_20251_g4/tree/estudante/trabalho_final/historias_usuarios)
- [Diagramas UML](../modelos_uml)
