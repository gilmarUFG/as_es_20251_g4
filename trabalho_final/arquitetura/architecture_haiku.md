# Architecture Haiku — E-commerce Blockchain

## Haiku Arquitetural

Blocos conectados,  
Confiança na cadeia,  
Fluxo transparente.

---

## Essência Arquitetural

- **Transparência e rastreabilidade**: Blockchain registra transações, avaliações e eventos críticos, garantindo confiança.
- **Segurança**: Autenticação robusta, armazenamento seguro de dados sensíveis e integração com provedores confiáveis.
- **Escalabilidade e flexibilidade**: Arquitetura modular baseada em serviços gerenciados da AWS.
- **Evolução contínua**: Pontos de extensão previstos, como integração futura com transportadoras e análise de dados em lakehouse.

---

## Stack Tecnológico

- **Frontend Web (SPA)**: Desenvolvido em **React**, hospedado em Amazon S3 ou EC2.
- **Backend/API**: Desenvolvido em **.NET**, exposto via REST API.
- **Banco de Dados Relacional (PostgreSQL no Amazon RDS)**: Persistência de dados operacionais.
- **Blockchain (Amazon Managed Blockchain)**: Registro imutável de eventos e transações.
- **AWS API Gateway**: Gerenciamento de requisições HTTP.
- **Gateways de Pagamento**: Integração para pagamentos digitais.
- **Serviços de Autenticação de Terceiros**: Login social e autenticação federada.

---

## Princípios

- **Separação de responsabilidades**: Camadas bem definidas (apresentação, aplicação, domínio, infraestrutura).
- **Baixo acoplamento, alta coesão**: Módulos independentes, comunicação via APIs.
- **Imutabilidade e confiança**: Blockchain como fonte de verdade para eventos críticos.
- **Documentação viva**: Diagramas PlantUML e especificações versionadas.

---

## Referências

- [Definição dos Requisitos](../definicao_trabalho_final_g4.md)
- [Histórias de Usuário](https://github.com/gilmarUFG/rs_es_20251_g4/tree/estudante/trabalho_final/historias_usuarios)
- [Diagramas UML](../modelos_uml)
