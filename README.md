# Caracterização dos movimentos pendulares nas principais vias de acesso à cidade de Lisboa

## Resumo

Este relatório apresenta um estudo que tem como objetivo analisar os fluxos diários de 
tráfego nas horas de ponta em Lisboa, considerando fatores como o calendário escolar, 
períodos de férias e a ocorrência de períodos de chuva nos principais pontos de entrada e 
saída da cidade. Utilizando dados de telemóveis, investigamos como as pessoas se 
movimentam durante as horas de ponta da manhã (7:00h-10:00h) e da tarde (17:00h-20:00h), explorando também outros períodos, como dias intensos de tráfego elevado, como 
a sexta-feira e o domingo. Além disso, aplicamos modelos preditivos para antecipar 
cenários futuros de mobilidade. Esses modelos foram baseados em redes neurais 
recorrentes (RNNs), em particular o GRU. Demostramos que esses modelos podem prever 
a intensidade do tráfego móvel com alguma precisão, com erros percentuais inferiores a 
10%. Desta forma, permitindo antecipar cenários futuros de mobilidade e identificar pontos 
críticos de congestionamento nas principais vias de acesso à cidade em diferentes 
momentos da semana

Palavras-chave: Fluxos diários de tráfego, Pontos de entrada e saída da cidade, Horas de 
ponta, Lisboa, Dados de telemóveis, Calendário escolar, Períodos de férias, Períodos de 
chuva, Mobilidade, Modelos preditivos, GRU (Gated Recurrent Unit), Pontos críticos de 
congestionamento.

## Resultados

### MAPE GRU prever à frente 1,2,4,8h para os Eixos da Cidade de Lisboa | Lag:24

| Prever à frente | A1   | A5   | A36  | Calçada Carriche | IC16 | IC19 | IC2 (Sacavém) | Marginal | N117 | Ponte 25 Abril | Ponte Vasco Gama |
|-------|------|------|------|------------------|------|------|---------------|----------|------|----------------|------------------|
| 1h    | 2.56 | 1.80 | 1.06 | 1.82             | 2.17 | 1.82 | 2.72          | 1.52     | 1.84 | 1.71           | 1.84             |
| 2h    | 4.11 | 2.20 | 1.10 | 2.36             | 2.12 | 2.15 | 3.47          | 1.29     | 2.29 | 2.00           | 2.21             |
| 4h    | 4.65 | 2.51 | 1.39 | 2.15             | 2.53 | 3.14 | 3.21          | 1.58     | 3.30 | 2.13           | 2.77             |
| 8h    | 4.93 | 2.74 | 1.28 | 1.99             | 2.73 | 2.67 | 3.38          | 1.53     | 2.83 | 2.34           | 2.69             |

### MAPE GRU prever à frente 1,2,4,8h para os Eixos da Cidade de Lisboa | Lag:12

| Prever à frente | A1   | A5   | A36  | Calçada Carriche | IC16 | IC19 | IC2 (Sacavém) | Marginal | N117 | Ponte 25 Abril | Ponte Vasco Gama |
|-------|------|------|------|------------------|------|------|---------------|----------|------|----------------|------------------|
| 1h    | 2.69 | 2.46 | 2.23 | 1.84             | 2.73 | 1.82 | 2.45          | 1.96     | 2.16 | 1.31           | 1.82             |
| 2h    | 3.78 | 2.58 | 1.32 | 2.01             | 2.35 | 2.57 | 3.61          | 1.79     | 2.55 | 2.20           | 2.76             |
| 4h    | 5.93 | 3.39 | 2.26 | 2.86             | 2.89 | 3.40 | 4.28          | 1.49     | 3.47 | 2.61           | 2.59             |
| 8h    | 5.92 | 3.96 | 1.39 | 2.49             | 2.84 | 2.84 | 3.95          | 1.85     | 4.22 | 2.36           | 2.80             |

### MAPE GRU prever à frente 24h para os Eixos da Cidade de Lisboa | Lag:24*7 (1 semana)

| Prever à frente | A1   | A5   | A36  | Calçada Carriche | IC16 | IC19 | IC2 (Sacavém) | Marginal | N117 | Ponte 25 Abril | Ponte Vasco Gama |
|-------|------|------|------|------------------|------|------|---------------|----------|------|----------------|------------------|
| 1h    | 3.86 | 2.52 | 2.22 | 2.67             | 2.14 | 2.85 | 3.16          | 1.68     | 3.59 | 2.62           | 3.28             |



## Conclusões

Examinámos a previsão de tráfego através dos dados de localização de telemóveis, 
baseada em RNN, em particular o GRU, na qual foi estimada a quantidade de tráfego 
móvel com período de 1 h. O desempenho dos modelos de previsão de tráfego foi 
verificado utilizando os dados realistas recolhidos pelo LxDataLab, durante setembro de 
2021 e dezembro de 2022. Em relação à avaliação do desempenho, confirmamos que a 
intensidade de tráfego móvel pode ser prevista com alguma precisão utilizando o modelo 
GRU. Esta conclusão é sustentada pelos erros percentuais que são relativamente baixos, 
em geral inferiores a 10% tanto para cada um dos 11 eixos como para a soma de todos, 
na previsão com 8 h de antecedência

## Trabalho Futuro

Como trabalho futuro, são apresentadas aqui, as seguintes sugestões:

 - Incorporar modelo para diferenciar dias de semana dos feriados e fins de semana
 - Explorar outros modelos, como LSTM e SAEs
 - Explorar modelos para dados com períodos de amostragem de 5, 15, 30 min


