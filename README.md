# Prediction_of_Wine_Quality
Modelo para estimar a qualidade do vinho, baseado em variáveis retiradas de testes físico-químicos.

Perguntas que guiaram esse estudo:

## a. Como foi a definição da sua estratégia de modelagem?

  A estratégia de modelagem seguiu os passos mais comuns de projetos de Data Science:

  - Primeiro, foi feita uma Análise Exploratória dos Dados para entender as variáveis que seriam utilizadas nos modelos, e também para verificar a existência de lacunas nos dados que deveriam ser tratadas, como dados faltantes (null), dados repetidos etc.

  - Neste processo, foi feita a análise de correlação dos dados para verificar a possível influência das variáveis de entrada entre si e também a influência dessas variáveis com a variável resposta.

  - Depois de tudo isso, foi feito o processamento das váriveis para serem utilizadas por modelos estatísticos.

  - O projeto terminou com a análise de modelos estatísticos para a resolução do problema e mudanças na variável resposta.

## b. Como foi definida a função de custo utilizada?

  A função de custo levou em consideração a quantidade de operações realizadas para processamento dos dados e a variação dos resultados obtidos. Se uma operação não tivesse ganhos perceptiveis na saida do modelo, ela não era executada. Por exemplo, o PCA não foi utilizado na versão final desse projeto, pois os resultados finais não sofriam mudanças significativas.

## c. Qual foi o critério utilizado na seleção do modelo final?

  O critério utilizado foi o desempenho do modelo no processo de validação.

## d. Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar este método?
  
  Para validação dos modelos foi utilizado como critério o maior valor encontrado nas seguintes variáveis para cada modelo:
  - Precision, Recall, F1-score
  - Matriz de Confusão
  
  Este método foi selecionado, pois acredito que ele facilita a comunicação do desempenho de modelos entre desenvolvedores e clientes.

## e. Quais evidências você possui de que seu modelo é suficientemente bom?
  - Ele possui melhores resultados no processo de validação do que outros 3 modelos que também foram analisados, e além disso, é simples para apresentar para um cliente e uma equipe de desenvolvimento.
