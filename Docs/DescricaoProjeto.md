# BankFlow

## Identificação da Equipe
- **Nome do Projeto:** BankFlow  
- **Integrantes:** Gabriel Naranti, João Miguel Firmino  
- **Repositório:** https://github.com/narantAO2/ProjetoIntegrado  

---

## Descrição do Problema
O BankFlow foi idealizado para resolver um problema crítico na empresa: o processo manual de cobrança e bloqueio do SaaS da BankMe.

Atualmente, o time financeiro:
- Calcula valores em planilhas  
- Gera cobranças manualmente no Asaas  
- Acompanha pagamentos manualmente  
- Depende de comunicação com o time de tecnologia para bloqueios  

Esse processo gera:
- Atrasos  
- Retrabalho  
- Risco de erros  

Com o BankFlow, todo esse fluxo será automatizado:
- O sistema calcula o valor do SaaS  
- Gera cobranças automaticamente  
- Monitora pagamentos  
- Executa bloqueios automaticamente em caso de inadimplência  

---

## Público-Alvo
- **Time financeiro:** cálculo de valores, cobrança e controle de inadimplência  
- **Time comercial:** cadastro de taxas por minibanco  
- **Banqueiros / minibancos:** usuários impactados pelas regras de cobrança  

---

## Justificativa
O BankFlow elimina um processo manual crítico da empresa, trazendo:

- Menos erros  
- Menos retrabalho  
- Mais rapidez na cobrança  
- Mais controle financeiro  

---

## Valor Gerado
- **Redução de trabalho manual:** eliminação de planilhas e processos manuais  
- **Menos erros:** cálculos automatizados com base em regras definidas  
- **Melhor fluxo de caixa:** cobranças mais rápidas e bloqueios no prazo  
- **Escalabilidade:** funciona mesmo com crescimento de minibancos  
- **Mais controle:** visão clara de pagamentos e inadimplência  

---

## Escopo Inicial

### Funcionalidades principais:
- Cadastro de taxas por minibanco  
- Cálculo automático do valor mensal  
- Geração e controle de cobranças (integração com Asaas)  

---

## Análise de Viabilidade

### Viabilidade Técnica
O uso de Node.js é ideal porque:

- Integra facilmente com APIs do Asaas (webhooks e cobranças)  
- Permite processamento assíncrono de regras e cálculos  
- Já é amplamente utilizado em sistemas financeiros no Brasil  

---

### Viabilidade Econômica

**Custos:**
- Desenvolvimento: realizado internamente (sem custo adicional)  
- Infraestrutura: uso da estrutura atual da empresa  
- Asaas: já utilizado atualmente  

**Benefícios:**
- Economia de tempo do time financeiro  
- Melhoria no fluxo de caixa  
- Escalabilidade do sistema  

**Conclusão:**  
Não há custo adicional relevante, apenas ganhos operacionais.

---

### Viabilidade Operacional
O sistema será de fácil utilização:

- Interface simples e intuitiva (React)  
- Automação das tarefas operacionais  
- Dashboard com visão clara dos dados  
- Baixa necessidade de treinamento  

**Conclusão:**  
Os usuários terão mais produtividade e menos erros.

---

## Riscos Iniciais
- Erros no cálculo do SaaS devido a dados incorretos  
- Resistência dos usuários à mudança de processo  
- Insatisfação com bloqueios automáticos por inadimplência  

---

## Considerações Finais
O BankFlow transforma um processo manual, lento e sujeito a erros em um fluxo automatizado, organizado e escalável.

Com a centralização de:
- Cálculo  
- Cobrança  
- Controle de inadimplência  

O sistema proporciona:
- Mais eficiência  
- Mais controle  
- Melhor previsibilidade financeira  

Além disso, permite que a empresa escale suas operações sem depender de planilhas e processos manuais, tornando a gestão mais profissional e eficiente.