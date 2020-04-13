# Prediction_of_Wine_Quality
Modelo para estimar a qualidade do vinho, baseado em variáveis referentes a dados de testes físico-químicos.

Perguntas que guiaram esse estudo:

## a. Como foi a definição da sua estratégia de modelagem?

  Na estratégia de modelagem foi contemplada as seguintes etapas de um projetos de Data Science:

  - Análise Exploratória dos Dados para estudar as variáveis que seriam utilizadas nos modelos, e também para verificar a existência de lacunas nos dados que deveriam ser tratadas, como dados faltantes (null), dados repetidos etc.

  - Análise de correlação dos dados para verificar a possível influência das variáveis de entrada entre si e também a influência dessas variáveis com a variável resposta.

  - Processamento das váriveis que serão utilizadas pelos modelos estatísticos, como transformação de valores categoricos em valores numéricos.

  - Análise de modelos estatísticos para a resolução do problema
  
  - Aprimoramento de resultados.

## b. Como foi definida a função de custo utilizada?

  A função de custo foi definida através da soma ponderada das variáveis de entrada de acordo com o grau de influência das mesmas para definição da variável de resposta. Os graus de influência foram definidos por meio de um algoritmo que implementa uma Floresta Aleatória de Classificação. 
  
## c. Qual foi o critério utilizado na seleção do modelo final?

  O critério utilizado foi o desempenho do modelo no processo de validação.

## d. Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar este método?
  
  Para o processo de validação, os dados foram divididos em conjuntos de treino e teste. O primeiro conjunto foi utilizado para o treinamento dos modelos, enquanto o segundo foi utilizado para mensurar o desempenho dos modelos.
  
  O critério utilizado foi o maior valor encontrado nas seguintes métricas de desempenho, nesta ordem:
  - Precision, Recall, F1-score
  - Diagonal principal da Matriz de Confusão
  
  A escolha deste método permite demostrar a relevância das conclusões do projeto, além de facilitar a comunicação do desempenho dos modelos entre desenvolvedores e clientes.

## e. Quais evidências você possui de que seu modelo é suficientemente bom?

  - Foram encontrados melhores resultados no processo de validação para o modelo selecionado do que para os outros 3 modelos que também foram analisados. Esses modelos foram selecionados de uma forma que permitissemos a comparação de estratégias diferentes de calculo de predição de classes. Por fim, destaca-se que o algoritmo do modelo selecionado é de fácil compreensão por clientes e desenvolvedores.
