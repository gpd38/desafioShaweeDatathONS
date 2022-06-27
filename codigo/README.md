# Hackathon de Dados - ONS

<p align="center">
  <a href="#Estudos e Análises">Estudos e Análises</a> •
  <a href="#Carga x Estação">Carga x Estação</a> •
  <a href="#Teste de Causalidade de Granger">Teste de Causalidade de Granger</a> •
  <a href="#EDA">EDA</a> •
  <a href="#Modelo">Modelo</a>
</p>


### Estudos e Análises

Foi utilizado os dados do portal do ONS para a realização deste projeto que tem como objetivo realizar uma correlação entre carga e temperatura.

Extraindo dados do portal 

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/01-estudo-analise.png"/><br>

Construindo dados temporais de carga

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/02-estudo-analise.png"/><br>

Consumo de energia por concessionária

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/03-estudo-analise.png"/><br>

Dataset INMET
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/04-estudo-analise.png"/><br>

Construindo dados temporais de temperatura

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/05-estudo-analise.png"/><br>

Localização geográficas das estações

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/06-estudo-analise.png"/><br>

Dataset Distribuídoras

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/07-estudo-analise.png"/><br>

Ponderando a importância dos postos por localização perto das distribuídoras

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/08-estudo-analise.png"/><br>

### Carga x Estação

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/01-carga-estacao.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/02-carga-estacao.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/03-carga-estacao.png"/><br>

### Teste de Causalidade de Granger

Correlação dos Postos com certa distribuidora

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/01-teste-causalidade.png"/><br>

### EDA

Foi realizada uma análise exploratória de dados para identificar os munícipios que possuem estações de medição por distribuidora e como a temperatura (baixa, média, máxima) estão distribuídas durante o verão no período de 2021/2022.

Separamos os municipios que possuem estação de medição por distribuidora

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/01-eda.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/02-eda.png"/><br>

Como está distribuída a maior, a menor e a temperatura média observada durante o verão 2021 - 2022?

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/03-eda.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/04-eda.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/05-eda.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/06-eda.png"/><br>

### Modelo

Com base na pré análise e manipulação dos dados escolhemos utilizar o modelo KNN, K Nearest Neighbors, para explorar a relação espacial entre carga e temperatura. Em seguida, optamos por utilizar um modelo de rede neural recorrente para prevêr dos dados de carga com base nos dados de temperatura obtidos geoespacialmente.

###### Modelo KNN

Imports

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/01-modelo.png"/><br>

Vizinhos próximos

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/02-modelo.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/03-modelo.png"/><br>

Escolhendo K

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/04-modelo.png"/><br>

###### Modelo de Previsão de Carga

Utilizando a RNN.

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/05-modelo.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/06-modelo.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/07-modelo.png"/><br>
<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/08-modelo.png"/><br>

CPFL Paulista

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/09-modelo.png"/><br>

ELEKTRO

<img src="https://github.com/gpd38/desafioShaweeDatathONS/blob/main/codigo/print/10-modelo.png"/><br>