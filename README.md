Previsão de Preços de Ações com Modelos ARIMA e SARIMAX

Este repositório contém um notebook Colab detalhado para a previsão de preços de ações usando os modelos ARIMA (AutoARIMA) e SARIMAX. O processo abrange desde a preparação inicial dos dados até a avaliação do desempenho do modelo com o Root Mean Squared Error (RMSE).
Conteúdo do Notebook:

    Introdução
        Importação de bibliotecas e carregamento do conjunto de dados.

    Pré-processamento de Dados
        Cálculo da média entre os preços mais baixos e mais altos.
        Criação da coluna "Actual" com deslocamento para frente.

    Visualização de Séries Temporais
        Plotagem da média dos valores das ações.
        Visualização do volume de ações vendidas.

    Normalização dos Dados e Divisão em Conjuntos de Treino e Teste
        Aplicação da normalização aos dados.
        Divisão dos dados em conjuntos de treino e teste.

    Análise de Séries Temporais
        Decomposição sazonal da série temporal.
        Verificação da estacionariedade com o teste ADF (Augmented Dickey-Fuller).

    Modelagem com AutoARIMA e SARIMAX
        Utilização do AutoARIMA para encontrar os melhores parâmetros.
        Implementação do modelo SARIMAX com Statsmodels.

    Geração de Previsões e Avaliação do Modelo
        Geração de previsões com o modelo treinado.
        Avaliação do desempenho utilizando o RMSE.

    Inversão da Normalização e Visualização dos Resultados Finais
        Inversão da normalização para comparar os resultados com os valores reais.

Utilização:

    Abra o notebook no Colab para uma experiência interativa.
    Siga cada etapa para entender e aplicar o processo de previsão de séries temporais.
    Experimente com diferentes conjuntos de dados ou ajuste os parâmetros do modelo.

Este projeto visa fornecer uma visão prática e educacional do uso de modelos ARIMA e SARIMAX na previsão de preços de ações. Sinta-se à vontade para explorar, aprender e contribuir!
