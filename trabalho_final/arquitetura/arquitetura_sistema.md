# Arquitetura do Sistema

## 1. Introdução
Este documento descreve a arquitetura necessária e suficiente para suportar o desenvolvimento dos requisitos definidos para a plataforma de e-commerce baseada em blockchain.

## 2. Objetivos Arquiteturais
- Garantir rastreabilidade e segurança das transações.
- Permitir integração com blockchain para registro de eventos.
- Suportar autenticação robusta de usuários e vendedores.
- Facilitar manutenção e evolução do sistema.

## 3. Visões Arquiteturais
- [Visão Geral](./visao_geral.md): Apresenta os módulos principais e os fluxos do sistema.
- [Visão Lógica](./visao_logica.md): Detalha os componentes, camadas e diagramas lógicos.
- [Visão Física](./visao_fisica.md): Descreve a infraestrutura proposta e possibilidades de evolução.

## 4. Diagramas
Os diagramas UML e PlantUML estão disponíveis na pasta `diagramas`.

## 5. Decisões Arquiteturais
- Uso de blockchain para registro de transações e avaliações.
- Separação de camadas (apresentação, aplicação, domínio, infraestrutura).
- Armazenamento seguro de dados sensíveis.
- Uso da AWS como infraestrtura principal.
- Armazenamento de arquivos estáticos no Amazon S3.
- Persistência de dados operacionais em Amazon RDS.
- Integração com Amazon Managed Blockchain.
- Gerenciamento de requisições HTTP via AWS API Gateway.
- Possibilidade de evolução para arquitetura serverless (AWS Lambda).

## 6. Histórias de Usuário
As histórias de usuário estão disponíveis no repositório original:
- [Pasta historias_usuarios](https://github.com/gilmarUFG/rs_es_20251_g4/tree/estudante/trabalho_final/historias_usuarios)

## 7. Referências
- [Definição dos Requisitos](../definicao_trabalho_final_g4.md)