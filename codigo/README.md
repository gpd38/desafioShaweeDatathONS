# Hackathon de Dados - ONS

### Estudos e Análises

Foi utilizado os dados do portal do ONS para a realização deste projeto que tem como objetivo realizar uma correlação entre carga e temperatura.

Foram utilizados os datasets INMET e Distribuidoras.

<img src="codigo/print/01-estudo-analise.png"/><br>
<img src="codigo/print/02-estudo-analise.png"/><br>
<img src="codigo/print/03-estudo-analise.png"/><br>

### EDA

Foi realizada uma análise exploratória de dados para identificar os munícipios que possuem estações de medição por distribuidora e como a temperatura (baixa, média, máxima) estão distribuídas durante o verão no período de 2021/2022.

<img src="codigo/print/01-eda.png"/><br>
<img src="codigo/print/02-eda.png"/><br>
<img src="codigo/print/03-eda.png"/><br>
<img src="codigo/print/04-eda.png"/><br>

### Modelo

Com base na pré análise e manipulação dos dados escolhemos utilizar o modelo KNN, K Nearest Neighbors, para explorar a relação espacial entre carga e temperatura. Em seguida, optamos por utilizar um modelo de rede neural recorrente para prevêr dos dados de carga com base nos dados de temperatura obtidos geoespacialmente.

###### Modelo KNN

<img src="codigo/print/01-modelo.png"/><br>


###### Modelo de Previsão de Carga


