# warpage_analysis
Um repositório com a análise realizada para meu projeto de conclusão de curso. 

## Descrição dos Dados
Os dados utilizado neste trabalho são baseados no artigo de [Taghizadeh](http://jps.shirazu.ac.ir/article_1744_b7eb8ed50d88a80fe3a7ade4b30059fb.pdf), que buscou prever o rechupe em uma peça circular de plástico, concebida pelo processo de injeção sob diversos parâmetros. Para obtenção dos dados Taghizadeh, utilizou o Moldflow Plastics Insight (MPI).
A princípio foi concebido o desenho 3D de uma peça com geometria similar a calços, espaçadores automotivos, transmissão e geração de energia. A peça em questão foi escolhida, justamente, por conta da importância que a sua forma final em relação ao seu desempenho. O plástico utilizado na simulação foi o Polietileno de baixa densidade (LDPE), com as seguintes propriedades:

* Temperatura de Injeção (°C): 180~280
* Temperatura do Molde (°C): 20~70
* Condutividade Térmica (W/m°C): 0.31
* Calor Específico(J/kg°C): 3400

O modelo foi importado para o MPI e em seguida foi aplicada uma malha, antes de se realizar a análise. Foi escolhida uma malha de elementos triangulares. O tipo de malha foi a malha para superfícies fundidas. De maneira que ao fim do processo foram obtidos 1174 nós, com 2204 elementos triangulares, e com Match ratio (**entender oq é**) de 97%. 
Vale ressaltar que foram também simulados canais de resfriamento situados a 15 mm da superfície da peça e com distâncias entre canais de 55mm.

Ao todo foram selecionados para a simulação cinco níveis de temperatura de injeção (280,255,230,205 e 180°C), três níveis da pressão de recalque(90,75 e 60% da pressão máxima de injeção), três níveis de  temperatura do molde (70,45 e 20°C). A partir desses valores foi criado um conjunto de dados de treino, utilizando-se o método fatorial de design de experimento
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTYxOTk5MjQyLDE0OTgxNTI2MTQsLTE1Mz
E2MzI4NTFdfQ==
-->