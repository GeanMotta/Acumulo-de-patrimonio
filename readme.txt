Estas ferramentas buscam mostrar o efeito do acúmulo de patrimônio ao longo do tempo. É uma forma de demonstrar empiricamente que o preço dos ativos comprados não é mais importante que o hábito de poupar constantemente. A volatilidade implícita dos ativos permite a diluição do preço médio, ao ponto de que o mesmo deixa de ser relevante para propósito outro ao de declarar o imposto de renda.

O programa simula o valor acumulado de patrimônio investindo-se em ações aleatórias do S&P 500 ou do Ibovespa, considerando-se o primeiro preço de cada mês, o menor preço de cada mês e o maior preço de cada mês. Com isso podemos ver melhor se é realmente importante dar a "tacada certa", ou se ter constância nos aportes é bom o suficiente.

Como usar: Utilize o arquivo acumulação.ipynb para rodar a simulação. As variáveis de interesse são "tickers",empr_estudadas, start, end e investimento, presentes na célula 2.


Em tickers, use a função traz_ibov() para escolher ações do Ibovespa e traz_SP() para trazer ações do S&P 500. O argumento da função é o número de ações que será estudado.

Use as variáveis start e end para determinar respectivamente as datas de início e fim da análise. A variável investimento é o valor monetário investido em CADA UMA das ações. Então se traz_ibov(5) e investimento = 1000, o investimento mensal será 5 * 1000 = 5000.


As ações são escolhidas aleatoriamente pelo programa e o dataframe mega_frame contém os valores acumuldos nas 3 categorias de investimento.
O resultado será plotado ao final, junto com o nome das ações envolvidas na análise.

Utilize as variáveis p, m_maior e m_menor para ver dataframes mostrando o desempenho de cada ação estudada comprando-se respectivamente no primeiro preço de fechamento de cada mês, no maior preço de cada mês e no menor preço de cada mês.

__________________

Use "Constant investment over random stock"" to simulate the investment of a fixed value (variable monthly_investment) in random stocks of the S&P 500 index. The program is meant to show that diversification (and random diversification at that!) is a sustainable and mostly carefree way of accumalating capital in the stock market.

How to use: Just open "Constant investiments.inpynb" and change the montly_investment variable to fit your investment value. Based on the present S&P stocks and the period of time set in "Dates_stocks.csv", the program will calculate the accumulated capital on random stocks, following the adjusted close price in the first day of every month of the given period of time.

The last simulation made is saved as "Latest simulation.csv" in the same folder.
ALL DATA GOES THROUGH YAHOO, THE REASON WHY THE BIGGER THE TIMEFRAME, THE LONGER IT WILL TAKE TO DO A SIMULATION.