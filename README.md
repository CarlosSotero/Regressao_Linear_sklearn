# Regressao_Linear_sklearn
## Previsão de Preço de Carros com Regressão Linear
Este projeto utiliza regressão linear com a biblioteca sklearn para prever o preço de carros com base em um conjunto de dados chamado CarPrice_Assignment.csv. O método MRLS foi utilizado para a verificação do p-value das variáveis, e o método de eliminação reversa (Backward Elimination) foi aplicado para eliminar variáveis com p-value alto.

### Estrutura do Dataset
O dataset CarPrice_Assignment.csv possui as seguintes colunas:

1. car_ID: Identificação única do carro
2. symboling: Classificação de risco de seguro (quanto maior, maior o risco)
3. CarName: Nome do carro
4. fueltype: Tipo de combustível
5. aspiration: Tipo de aspiração do motor (normal ou turbo)
6. doornumber: Número de portas do carro
7. carbody: Tipo de carroceria
8. drivewheel: Tipo de tração
9. enginelocation: Localização do motor
10. wheelbase: Distância entre os eixos do carro
11. carlength: Comprimento do carro
12. carwidth: Largura do carro
13. carheight: Altura do carro
14. curbweight: Peso do carro sem carga
15. enginesize: Tamanho do motor em centímetros cúbicos
16. fuelsystem: Sistema de combustível
17. boreratio: Diâmetro do cilindro do motor
18. stroke: Curso do pistão do motor
19. compressionratio: Taxa de compressão do motor
20. horsepower: Potência do motor em cavalos
21. peakrpm: Rotação máxima do motor por minuto
22. citympg: Consumo de combustível na cidade 
23. highwaympg: Consumo de combustível na estrada
24. price: Preço do carro

### Metodologia
1. Carregamento e Pré-processamento dos Dados:
    1. Carregar o dataset CarPrice_Assignment.csv.
    2. Realizar transformação dos dados conforme necessário.
2. Análise Exploratória dos Dados:
    1. Analisar a distribuição das variáveis.
    2. Identificar a quantidade de carros por preço.
3. Verificação do p-value com MRLS:
    1. Utilizar o método MRLS para verificar o p-value das variáveis.
    2. Selecionar variáveis significativas para o modelo.
4. Eliminação Reversa (Backward Elimination):
    1. Aplicar o método de eliminação reversa para remover variáveis com p-value alto.
    2. Refinar o modelo de regressão linear.
5. Treinamento e Avaliação do Modelo:
    1. Dividir os dados em conjuntos de treinamento e teste.
    2. Treinar o modelo de regressão linear com sklearn.
    3. Avaliar o desempenho do modelo com as métricas Coeficiênte de Determinação (R^2), Mean Absolute Error (MAE), Mean Squared Error (MSE) e RMSE (raiz quadrada do MSE).
