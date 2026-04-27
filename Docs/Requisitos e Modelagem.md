# **Requisitos e Modelagem**

## **Requisitos Funcionais**

**RF01:** O sistema deve permitir o cadastro de banqueiros e minibancos, com dados como nome, documento, taxa SaaS e status de contratação.

**RF02:** O sistema deve calcular automaticamente o valor mensal do SaaS de cada banqueiro com base nas regras de negócio configuradas.

**RF03:** O sistema deve gerar cobranças de forma integrada à API do Asaas, registrando o status de cada cobrança no sistema.

---

## **Requisitos Não Funcionais**

**RNF01:** O sistema deve responder às principais operações em até 2 segundos na maioria das requisições.

**RNF02:** O sistema deve garantir segurança dos dados por meio de criptografia em trânsito e controle de acesso por autenticação.

**RNF03:** O sistema deve ser de fácil manutenção, com código organizado, documentação mínima e estrutura modular.

---

## **Casos de Uso**

**Caso 1: Cadastro de banqueiro**  
O usuário administrador acessa o sistema, informa os dados do banqueiro e salva o cadastro. O sistema valida os campos obrigatórios e registra as informações no banco de dados.

**Caso 2: Geração de cobrança**  
O usuário seleciona um banqueiro ativo, o sistema calcula o valor devido e envia a cobrança para a API do Asaas, atualizando o status da cobrança após o retorno.

---

## **Entidades do Sistema**

| Entidade | Atributos |
| :---- | :---- |
| Banqueiro | id, nome, documento, email, telefone, status |
| Minibanco | id, nome, CNPJ, responsável, status |
| Cobrança | id, valor, vencimento, status, data\_criação, banqueiro\_id |
| Usuário | id, nome, email, senha, perfil |
| Pagamento | id, valor, data\_pagamento, método, cobrança\_id |


<img width="1500" height="1800" alt="image" src="https://github.com/user-attachments/assets/58b600a9-b0d3-4f66-b979-f371fd7aa3d0" />


**Regras de Negócio**

**Regra 1:** Apenas banqueiros com status “ativo” podem receber cobrança mensal.

**Regra 2:** Se a cobrança não for paga até a data de vencimento, o sistema deve marcar o banqueiro como inadimplente e registrar essa alteração.

**Considerações**

A modelagem do BankFlow foi construída com foco na automação do processo de cobrança SaaS, controle de inadimplência e integração com serviços externos. Os requisitos funcionais cobrem as operações principais do sistema, enquanto os requisitos não funcionais garantem desempenho, segurança e manutenção. As entidades e regras de negócio representam a base para o desenvolvimento da aplicação e para a estruturação do banco de dados.  
