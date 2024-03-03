# Caracterização dos movimentos pendulares nas principais vias de acesso à cidade de Lisboa



## Abstract
This report presents a study aimed at analyzing the daily traffic flows during peak hours in 
Lisbon, considering factors such as the school calendar, vacation periods, and the 
occurrence of rainy periods at the city's main entry and exit points. Using mobile data, we 
investigated how people move during the morning (7:00 am - 10:00 am) and afternoon 
(5:00 pm - 8:00 pm) peak hours, as well as other periods with high traffic, such as Fridays 
and Sundays. Additionally, we applied predictive models to anticipate future mobility 
scenarios. These models were based on recurrent neural networks (RNNs), specifically the 
GRU (Gated Recurrent Unit). We demonstrated that these models could predict mobile 
traffic intensity with some accuracy, achieving error rates below 10%. Thus, enabling the 
anticipation of future mobility scenarios and the identification of critical congestion points 
on the main city access routes at different times of the week.

Keywords: Daily traffic flows, City entry and exit points, Peak hours, Lisbon, Mobile data, 
School calendar, Vacation periods, Rainy periods, Mobility, Predictive models, GRU 
(Gated Recurrent Unit), Critical congestion points.

## Resultados

### MAPE GRU prever à frente 1,2,4,8h para os Eixos da Cidade de Lisboa | Lag:24

| Prever à frente | A1   | A5   | A36  | Calçada Carriche | IC16 | IC19 | IC2 (Sacavém) | Marginal | N117 | Ponte 25 Abril | Ponte Vasco Gama |
|-------|------|------|------|------------------|------|------|---------------|----------|------|----------------|------------------|
| 1h    | 2.56 | 1.80 | 1.06 | 1.82             | 2.17 | 1.82 | 2.72          | 1.52     | 1.84 | 1.71           | 1.84             |
| 2h    | 4.11 | 2.20 | 1.10 | 2.36             | 2.12 | 2.15 | 3.47          | 1.29     | 2.29 | 2.00           | 2.21             |
| 4h    | 4.65 | 2.51 | 1.39 | 2.15             | 2.53 | 3.14 | 3.21          | 1.58     | 3.30 | 2.13           | 2.77             |
| 8h    | 4.93 | 2.74 | 1.28 | 1.99             | 2.73 | 2.67 | 3.38          | 1.53     | 2.83 | 2.34           | 2.69             |



## Usage
[Explain how to use your project. Provide examples, if applicable, and describe any commands or inputs required to run the project. Include screenshots or gifs to demonstrate its functionality, if possible.]

## Contributing
[Include guidelines for contributing to your project. This may involve instructions on how to report bugs, submit feature requests, or contribute code. Be sure to specify any coding standards or conventions to follow.]

## License
[Specify the license under which your project is distributed. Include any terms or conditions for using, modifying, or distributing your project.]
