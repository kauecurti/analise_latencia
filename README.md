Detecção de Anomalias em Latências de Serviços com Visualizações

Descrição Geral

Este projeto apresenta um pipeline integrado para análise, detecção de anomalias e visualização em latências de serviços. Utilizando dados de latência armazenados em arquivos Excel, o pipeline envolve o carregamento desses dados em um banco de dados PostgreSQL, a transferência para o Google BigQuery, análise exploratória e estatística, modelagem preditiva com classificadores Random Forest, e visualizações interativas utilizando Dash e Plotly.

Pipeline de Dados

1. Carregamento e Preparação dos Dados
   
Carregamento de Dados: Os dados são carregados de arquivos Excel (e.g., latencia2.xlsx), contendo registros de latências de serviços.
Armazenamento de Dados: Os dados são armazenados em uma tabela (e.g., latencias, latencias2) num banco de dados PostgreSQL. Este passo facilita a manipulação e a análise subsequente dos dados.
Transferência para BigQuery: Os dados são transferidos para o Google BigQuery para permitir análises escaláveis e o armazenamento seguro na nuvem.

2. Análise Exploratória e Preparação dos Dados
   
Transformação de Dados: As strings de latências são convertidas em listas de inteiros para análise.
Cálculo de Percentis: Percentis (e.g., 60º, 90º, 95º) são calculados para estabelecer limiares na identificação de anomalias. Os percentis servem como referência para rotular os dados com base na distribuição de latências.

3. Detecção de Anomalias
   
Rotulagem de Dados: Dados são rotulados como anômalos ou normais com base nos limiares definidos pelos percentis calculados.
Modelagem com Random Forest: Utiliza-se o classificador Random Forest para treinar modelos capazes de prever anomalias. A modelagem é iterativa, buscando o melhor modelo com base na acurácia.

4. Visualização de Dados
   
Dash e Plotly: Para a visualização em tempo real e interativa das previsões de anomalias, utiliza-se uma aplicação Dash com gráficos gerados pelo Plotly.
Boxplot e Gráficos de Barras: São criados para visualizar a distribuição das latências e as previsões de anomalias, respectivamente, facilitando a identificação visual de padrões anômalos.
Porcentos Usados

60º Percentil: Usado para rotular latências como anômalas em um dos pipelines, ajudando a focar em valores significativamente altos que podem indicar problemas.
90º e 95º Percentis: Utilizados para categorizar latências em "Normal", "Possible Anomaly", e "Severe Anomaly", permitindo uma granularidade maior na análise de anomalias.
Requisitos

Python
Pandas
SQLAlchemy
Numpy
Scikit-Learn
Joblib
Dash
Plotly
Google Cloud BigQuery
PostgreSQL
Uso

Para utilizar este pipeline, instale as dependências necessárias e configure o acesso ao PostgreSQL e ao Google Cloud. Execute os scripts na ordem apresentada para carregar os dados, realizar a análise, treinar o modelo e visualizar os resultados. Ajuste os limiares dos percentis conforme necessário para adequar-se às especificidades dos seus dados de latência.

Conclusão

Este pipeline integrado oferece uma abordagem robusta para a detecção e análise de anomalias em dados de latência de serviços. Através da combinação de análises estatísticas, modelagem preditiva, e visualizações interativas, facilita-se a identificação de problemas de performance e a tomada de decisões baseada em dados.
