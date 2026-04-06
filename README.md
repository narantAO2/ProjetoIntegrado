# BankFlow

## Identificação da equipe

**Nome do projeto:** BankFlow  
**Integrantes:** Gabriel Naranti, João Miguel Firmino  
**Repositório GitHub:** [Projeto Integrado](https://github.com/narantAO2/ProjetoIntegrado)  
**Disciplina:**  
**Data:**  

## Descrição do problema

O **BankFlow** vai resolver a cobrança e o bloqueio manual do SaaS da BankMe.

Hoje, o time financeiro calcula os valores em planilhas, envia as cobranças no Asaas e depois precisa acompanhar de forma manual quem pagou ou não. Quando há inadimplência, alguém precisa perceber o atraso e avisar o time de tech para bloquear o banqueiro no banco de dados. Isso gera atraso, retrabalho e risco de erro.

Com o **BankFlow**, o processo passa a ser automatizado: o sistema calcula o valor do SaaS de cada minibanco, gera a cobrança, acompanha o pagamento e, se houver atraso, executa o bloqueio automaticamente dentro da plataforma. Assim, a empresa ganha mais controle, menos trabalho manual e uma regra de cobrança mais clara e organizada.

## Público-alvo

- **Time financeiro:** calcula valores, gera cobranças e acompanha inadimplência.
- **Time comercial:** cadastra as taxas negociadas com cada minibanco.
- **Banqueiros/minibancos:** usam a plataforma e são afetados pelas regras de cobrança.

## Justificativa

O **BankFlow** é importante porque tira do manual um processo crítico da empresa: cobrança, acompanhamento de inadimplência e bloqueio de acesso.

Isso gera valor direto em:
- Menos erros.
- Menos retrabalho.
- Mais rapidez na cobrança.
- Mais controle financeiro.

## Valor gerado

- **Redução de trabalho manual:** o time financeiro deixa de calcular valores em planilha e cobrar caso a caso.
- **Menos erros de cobrança:** o sistema calcula e cobra com base nas regras cadastradas, evitando falhas humanas.
- **Melhor fluxo de caixa:** cobranças automáticas e bloqueio no prazo ajudam a receber mais rápido.
- **Mais escala:** o processo funciona mesmo se o número de minibancos crescer muito.
- **Mais previsibilidade e controle:** o financeiro passa a ter visão clara de quem pagou, quem está em atraso e o que precisa ser bloqueado.

## Escopo inicial

### Funcionalidades previstas
1. **Cadastro de taxas por minibanco.**
2. **Cálculo automático do valor mensal.**
3. **Geração e controle da cobrança, com integração com o Asaas.**

## Análise de viabilidade

### Viabilidade técnica

O **Node.js** é uma boa escolha para o **BankFlow** porque:
- Integra facilmente com APIs do Asaas, como webhooks e cobranças.
- Processa cálculos e regras de bloqueio de forma assíncrona.
- Projetos reais de cobrança e PIX no Brasil já usam Node.js.

### Viabilidade econômica

**Custos relevantes:**
- Desenvolvimento: feito pelos devs da empresa, sem custo extra de contratação.
- Infraestrutura: usa a infraestrutura atual da BankMe, sem custo adicional.
- Asaas: já está sendo usado hoje, com o mesmo custo atual.

**Por que vale a pena:**
- Economia de tempo: o time financeiro para de usar planilha e fazer cobrança manual.
- Melhor fluxo de caixa: recebe mais rápido por causa do bloqueio automático.
- Escala: funciona bem mesmo com mais minibancos no futuro.

**Conclusão:** não há custo extra de desenvolvimento ou infraestrutura, apenas benefícios operacionais imediatos.

### Viabilidade operacional

Sim, o sistema será facilmente utilizável pelos usuários.

**Por quê?**
- Interface simples: painel web intuitivo, similar às ferramentas que o financeiro já usa.
- Automação de tarefas: cálculo de valores e geração de cobrança funcionam sozinhos.
- Visão clara: dashboard mostra quem pagou, quem está atrasado e o status dos bloqueios.
- Treinamento mínimo: substitui planilha por algo mais simples de usar.

**Conclusão:** os usuários finais, como financeiro e comercial, vão economizar tempo e ter menos erros, pois o sistema faz o trabalho pesado automaticamente.

## Riscos iniciais

- **Risco 1:** erros no cálculo do SaaS, caso as taxas cadastradas ou os dados de operação estejam incorretos.
- **Risco 2:** resistência dos usuários internos à troca da planilha pelo novo sistema.
- **Risco 3:** insatisfação dos banqueiros com a automação do bloqueio por inadimplência, já que hoje existe mais flexibilidade no pagamento.

## Considerações finais

O **BankFlow** é uma proposta para transformar um processo de cobrança hoje manual, demorado e sujeito a erros em um fluxo mais organizado, automático e fácil de acompanhar.

Ao centralizar o cálculo do SaaS, a geração de cobranças e o controle da inadimplência, o sistema reduz retrabalho, melhora a precisão das cobranças e dá mais previsibilidade para a operação financeira.

Além disso, o projeto gera valor porque ajuda a empresa a escalar esse processo sem depender de planilhas e ações manuais entre diferentes times. Com isso, o **BankFlow** contribui para mais controle interno, melhor acompanhamento dos minibancos e uma gestão de cobrança mais eficiente e profissional.
