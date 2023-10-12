# Price-Sarima

Previsão de Séries Temporais com SARIMA
Este é um script Python que demonstra como realizar previsões de séries temporais de preços de ações usando o modelo SARIMA (Seasonal Autoregressive Integrated Moving Average).

Resumo do Script
Importação de Bibliotecas: O script começa importando as bibliotecas necessárias, incluindo pandas, numpy, matplotlib, seaborn, statsmodels e pmdarima.

Carregamento dos Dados: Os dados são carregados a partir de um arquivo CSV chamado "price.csv". As primeiras linhas do conjunto de dados são exibidas, e a média dos valores "Low" e "High" é calculada e armazenada em uma nova coluna chamada "Mean".

Pré-processamento dos Dados: Uma cópia do conjunto de dados é criada para fins de previsão. Os valores da coluna "Mean" são deslocados por um número especificado de passos para criar os valores "Atuais" a serem previstos. As linhas com dados ausentes são removidas.

Manipulação de Datas: A coluna "Date" é convertida para o formato de data e definida como o índice do conjunto de dados.

Visualização dos Dados: O script gera gráficos usando o Matplotlib para visualizar os dados de preço das ações e o volume de negociação.

Escalonamento dos Dados: O script utiliza o MinMaxScaler para dimensionar os dados de entrada e saída para um intervalo entre 0 e 1. Os dados de entrada incluem as colunas "Low", "High", "Open", "Close", "Volume", "Adj Close" e "Mean", enquanto os dados de saída são da coluna "Atual".

Modelagem SARIMA: O modelo SARIMA é configurado com base nos parâmetros selecionados usando a função auto_arima do pmdarima. O modelo é treinado nos dados de treinamento.

Previsões e Avaliação: O modelo SARIMA é usado para fazer previsões nos dados de teste. O Erro Quadrático Médio da Raiz (RMSE) é calculado para avaliar o desempenho do modelo.

Visualização das Previsões: As previsões e os valores reais são plotados para visualizar o desempenho do modelo.

Previsões Futuras: O script realiza previsões de preços de ações futuros e as visualiza.

Requisitos
Python 3
Bibliotecas Python: pandas, numpy, matplotlib, seaborn, statsmodels, pmdarima, entre outras (consulte o início do script).
Uso
Para executar o script, siga estas etapas:

Certifique-se de ter instalado todas as bibliotecas necessárias.
Faça o download do conjunto de dados de preços de ações e salve-o como "price.csv" no mesmo diretório do script.
Execute o script em um ambiente Python.
Resultados
O script fornecerá previsões de preços de ações e avaliará o desempenho do modelo usando RMSE.

Este projeto é uma demonstração básica de como aplicar modelagem SARIMA para previsões de séries temporais e pode ser estendido e aprimorado para prever preços de ações em cenários do mundo real.

Nota: Certifique-se de entender os conceitos de séries temporais e os detalhes da modelagem SARIMA antes de usar este script em um contexto de negócios ou financeiro.
