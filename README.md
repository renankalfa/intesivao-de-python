# Semanas e Eventos
Neste repositório serão armazenados os arquivos, descrições dos eventos e os meus aprendizados.

## Intensivão de Python - Hashtag Programação
Um evento focado em Python para utilizá-lo na **automatização de qualquer processo, Análise de Dados, Web Ccraping** e um **projeto de Ciência de Dados e Inteligência Artificial** do começo ao fim.

### Aprendizados
#### Aula 1 - Automação de Sistemas e Processos com Python
##### Desafio
Todos os dias, o nosso sistema atualiza as vendas do dia anterior. O seu trabalho diário, como analista, é enviar um e-mail para a diretoria, assim que começar a trabalhar, com o faturamento e a quantidade de produtos vendidos no dia anterior.
##### Como resolvi o desafio?
- Usando o **pyautogui** e o **pyperclip** automatizei o processo de entrar no sistema, navegar pelo sistema e baixar uma base de dados;
- Usando a biblioteca **pandas**, analisamos a base de dados baixada e obtive o faturamento e a quantidade de produtos vendidas (armazenei em uma variável);
- Por fim, para enviar um e-mail utilizei de novo o **pyautogui** e o **pyperclip**.

Ao automatizar pela primeira vez eu fiquei encantado. Porém, a limitação desse modo é não poder realizar outra tarefa enquanto a automatização é feita.

#### Aula 2
##### Desafio
Você trabalha em uma empresa de telecom e tem clientes de vários serviços diferentes, entre os principais: internet e telefone. O problema é que, analisando o histórico dos clientes dos últimos anos, você percebeu que a empresa está com Churn de mais de 26% dos clientes. Isso representa uma perda de milhões para a empresa. O que a empresa precisa fazer para resolver isso?
##### Como resolvi o desafio?
- **Tratamento dos dados**: depois de importar a base usando o **pandas**, tratei valores vazios e analisei e troquei o tipo primitivo dos dados de uma tabela (de string para float);
- **Análise inicial**: será mesmo que temos mais de 26% dos clientes estão cancelando os serviços? depois de uma pequena análise confirmei que sim;
- **Análise detalhada**: criei cada gráfico que relaciona cada coluna com a situação Churn. Com isso, foi possível analisar e tirar insights.
##### Insights
- Pessoas com famílias menos tem mais chance de cancelar
    - Criar um plano família
- Nos primeiros meses as pessoas cancelam mais (**maioria**)
    - Criar algum plano fidelidade (bônus)
    - Quanto mais tempo com a gente, menos chance tem de cancelares
    - Primeira experiência ruim (**resolver**)
- A taxa de cancelamento é maior na internet fibra (muito alto)
    - Identificar/resolver os problemas da fibra
- Quantos mais serviços os clientes aceitam, menos as chances deles cancelarem
    - Fornecer mais serviços de forma gratuita ou muito barata
- Quase todos os cancelamentos estão no contrato mensal
- A taxa de cancelamento do boleto é maior
    - Priorizar outras formas de pagamento
    - Desconto nas outras opções

Em construção...
