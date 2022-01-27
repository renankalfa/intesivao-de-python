# Semanas e Eventos
Neste repositório serão armazenados os arquivos, descrições dos eventos e os meus aprendizados.

## Intensivão de Python - Hashtag Programação
Um evento focado em Python para utilizá-lo na **automatização de qualquer processo, Análise de Dados, Web Ccraping** e um **projeto de Ciência de Dados e Inteligência Artificial** do começo ao fim. Em como funcionam, de maneira geral, as bibliotecas utilizadas e a implementação do código em Python. 

### Aprendizados
Os principais aprendizados durante esse intensivão foram na parte de **automatização de projetos, análise de dados** e um **projeto inteiro de Ciência de Dados**.
#### Aula 1 - **Automação de Sistemas e Processos com Python**
##### Desafio
Todos os dias, o nosso sistema atualiza as vendas do dia anterior. O seu trabalho diário, como analista, é enviar um e-mail para a diretoria, assim que começar a trabalhar, com o faturamento e a quantidade de produtos vendidos no dia anterior.
##### Como resolvi o desafio?
- Usando o **pyautogui** e o **pyperclip** automatizei o processo de entrar no sistema, navegar pelo sistema e baixar uma base de dados;
- Usando a biblioteca **pandas**, analisamos a base de dados baixada e obtive o faturamento e a quantidade de produtos vendidas (armazenei em uma variável);
- Por fim, para enviar um e-mail utilizei de novo o **pyautogui** e o **pyperclip**.

Ao automatizar pela primeira vez eu fiquei encantado. Porém, a limitação desse modo é não poder realizar outra tarefa enquanto a automatização é feita.

#### Aula 2 - **Análise de dados**
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

#### Aula 3 - **Web Scraping**
##### Desafio
Trabalhamos em uma importadora e o preço dos nossos produtos é vinculado a cotação de dólar, euro e ouro. Precisamos pegar na internet, de forma automática, a cotação desses 3 itens e saber quanto devemos cobrar pelos nossos produtos, considerando uma margem de contribuição que temos na nossa base de dados.
##### Como resolvi o desafio?
- **Pegando as cotações**: utilizando o **selenium** (configurei para abrir o Chrome), automatizei para pesquisar e guardar a cotação do dólar, euro e do ouro em uma variável.
- **Atualizando a base de dados**: depois de aberto a base de dados, utilizando o **pandas**, programei para atualizar as cotações, preço de comprae preço de venda. Depois, para exportar como excel.

#### Aula 4 - **Ciência de dados e Inteligência artificial**
##### Desafio
Nosso desafio é conseguir prever as vendas que vamos ter em determinado período com base nos gastos em anúncios nas 3 grandes redes que a empresa Hashtag investe: TV, Jornal e Rádio. TV, Jornal e Rádio estão em milhares de reais e vendas estão em milhões.
##### Como resolvi o desafio?
Depois de entender sobre o desafio, a área e a empresa, hora de botar a mão na massa (ou no Python). Importei a base de dados e no caso ela já veio "limpa".
- **Análise Exploratória**: depois de visualizar sobre como cada item está distribuído, por meio de gráficos das bibliotecas **seaborn** e **matplotlib**, foi possível visualizar a correlação entre cada coluna (por exemplo, a de vendas com a quantidade investida em anúncios na TV);
- **Modelagem + Algoritmos**: agora, separei a base de dados em uma parte para treinar (70% da base de dados) dois algoritmo e a outra parte para testar (30%), carreguei os modelos pela biblioteca **sklearn** (Regressão Linear e Random Forest), os treinei e gerei previsões. No meu caso, o modelo Random Forest, obteve uma melhor precisão.
- **Realização das previsões de vendas**: com o modelo treinado, agora foi possível gerar previsões para cada caso de investimento em anúncios.

Informações como essas, poderiam ser usadas pela galera de marketing para saber onde investir mais ou até deixar de investir em um meio; pela galera do gerenciamento de custos para ter uma dimensão melhor do quanto poderá ser gasto (despesas por exemplo) e como forma de incentivar o investimento nessa empresa demonstrando a sua mudança e o quanto a mais poderá ser retornado.

##
