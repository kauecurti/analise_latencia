Projeto de Detecção e Análise de Anomalias em Dados de Latência

Este projeto combina várias técnicas de aprendizado de máquina e análise estatística para detectar e analisar anomalias em dados de latência de serviços. Utiliza algoritmos de Floresta Aleatória e CNN-LSTM para classificar tempos de resposta como normais ou anômalos, e aplica análise estatística descritiva para uma compreensão mais profunda da distribuição dos dados. Além disso, inclui uma aplicação web Dash para visualização em tempo real das classificações de anomalias e utiliza Seaborn para visualizações estáticas.

Pré-requisitos

Certifique-se de ter as seguintes bibliotecas Python instaladas:

pandas
numpy
scikit-learn
joblib
TensorFlow
Plotly
Dash
matplotlib
seaborn
Você pode instalar todas as dependências necessárias com o comando:


pip install pandas numpy scikit-learn joblib tensorflow plotly dash matplotlib seaborn
Conjunto de Dados

Os conjuntos de dados esperados são arquivos Excel contendo dados de latência, onde cada valor é uma lista de latências separadas por vírgulas. Estes arquivos devem estar nomeados de acordo com o script específico que será executado, por exemplo, latencies by service.xlsx para análise estatística descritiva e detecção de anomalias com CNN-LSTM, e latencia2.xlsx para detecção de anomalias com Floresta Aleatória.

Estrutura do Projeto

Este projeto é dividido em três partes principais:

Detecção de Anomalias com Floresta Aleatória e Visualização com Dash: Utiliza um modelo de Floresta Aleatória para classificar dados de latência como normais ou anômalos e uma aplicação Dash para visualizar as classificações em tempo real.
Detecção de Anomalias com CNN-LSTM: Aplica uma abordagem de aprendizado profundo utilizando CNN-LSTM para detectar anomalias em séries temporais de dados de latência.
Análise Estatística Descritiva e Visualização com Seaborn: Realiza uma análise estatística descritiva dos dados de latência e utiliza Seaborn para criar visualizações estáticas que destacam anomalias.
Execução

Para executar cada parte do projeto, siga as instruções específicas contidas nos scripts correspondentes. Certifique-se de ajustar os caminhos dos arquivos de dados conforme necessário e de ter todas as dependências instaladas.

Treinamento e Salvamento do Modelo
Execute os scripts de treinamento apropriados para gerar os modelos de detecção de anomalias, salvando-os para uso posterior ou visualização em tempo real com Dash.

Visualização de Anomalias
Para visualizações em tempo real, utilize o script Dash após treinar o modelo de Floresta Aleatória.
Para visualizações estáticas, execute o script de análise estatística descritiva com Seaborn.
Visualizações

Este projeto oferece duas formas de visualização:

Dash: Para uma visualização interativa e em tempo real das classificações de anomalias.
Seaborn: Para visualizações estáticas que oferecem insights sobre a distribuição dos dados e a localização das anomalias.