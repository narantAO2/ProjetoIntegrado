## 📋 Modelos de Processo e Planejamento

## 🧠 Scrum

### Justificativa
O Scrum é adequado ao BankFlow porque o projeto envolve desenvolvimento incremental, validação frequente com a área financeira e integração entre backend, e serviços externos. Como a Sprint Review serve para inspecionar o incremento entregue e adaptar o Product Backlog com base no feedback dos stakeholders, esse modelo ajuda a alinhar a solução ao processo real de cobrança da empresa.

***

## ⚙️ Estrutura do Processo

Descreva como o projeto será executado:

- **Iterações (sprints):** sprints incrementais com priorização contínua do backlog e revisão ao final de cada ciclo.
- **Duração:** 1 a 2 semanas.
- **Entregas:** funcionalidades completas por incremento, priorizando cadastro de regras, cálculo do SaaS, geração de cobranças e monitoramento de pagamentos.

***

## 👥 Papéis da Equipe

- **Integrante 1 — Responsabilidade:** Gabriel Naranti — backend em Node.js, modelagem de dados, telas de cadastro e automações.
- **Integrante 2 — Responsabilidade:** João Miguel Firmino — , regras de negócio, , dashboard, experiência do usuário e integração com Asaas.

***

## 📌 Backlog Inicial

Liste as funcionalidades:

| ID | Funcionalidade | Prioridade |
|----|--------------|------------|
| 1  | Cadastro de minibancos | Alta |
| 2  | Cadastro de taxas por minibanco | Alta |
| 3  | Cálculo automático do valor mensal do SaaS | Alta |
| 4  | Geração de cobranças com integração Asaas | Alta |
| 5  | Monitoramento de pagamentos por webhooks | Alta |
| 6  | Bloqueio automático por inadimplência | Alta |
| 7  | Dashboard financeiro com visão de cobranças e inadimplência | Média |
| 8  | Histórico de cobranças | Média |
| 9  | Configuração de regras de cobrança | Média |

***

## 📅 Cronograma

| Semana | Atividade |
|--------|----------|
| 1 | Levantamento de requisitos e entendimento do processo atual |
| 2 | Modelagem do banco de dados e estrutura inicial do backend |
| 3 | Implementação do cadastro de minibancos e taxas |
| 4 | Desenvolvimento do cálculo automático do SaaS |
| 5 | Integração com a API do Asaas para geração de cobranças |
| 6 | Implementação de webhooks para acompanhamento de pagamentos |
| 7 | Regra de bloqueio por inadimplência e ajustes de negócio |
| 8 | Desenvolvimento das telas e dashboard |
| 9 | Testes integrados e validação com usuários |
| 10 | Correções finais e preparação da entrega |

***

## 🛠️ Ferramentas Utilizadas

- **GitHub:** versionamento de código, armazenamento do projeto e documentação em Markdown.
- **Trello / Jira:** organização do backlog, acompanhamento das sprints e controle das tarefas.
- **Outros:** Node.js, Postman, API do Asaas.

***

## 📌 Considerações

O planejamento do BankFlow foi estruturado para permitir entregas incrementais, foco nas funcionalidades mais críticas e adaptação contínua conforme o feedback do negócio. Além disso, a integração com o Asaas pode usar webhooks para manter a aplicação sincronizada com eventos de cobrança, o que fortalece a proposta de automação do projeto.
