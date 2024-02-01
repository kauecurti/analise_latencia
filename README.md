Descrição Geral

Este repositório contém três projetos independentes focados na análise e detecção de anomalias em tempos de resposta (latências) de serviços, utilizando diferentes abordagens e técnicas de machine learning e visualização de dados. Cada projeto é projetado para oferecer insights sobre o comportamento das latências, identificar potenciais anomalias e facilitar a tomada de decisões baseada em dados.

Requisitos Globais

Os projetos utilizam uma variedade de bibliotecas Python, que podem ser instaladas utilizando o gerenciador de pacotes pip. As principais dependências incluem:

Pandas
NumPy
Scikit-learn
TensorFlow/Keras
Matplotlib
Seaborn
Dash
Plotly
Para instalar todas as dependências necessárias para os três projetos, execute o seguinte comando:

bash
Copy code
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn dash plotly joblib
Estrutura dos Projetos

1. Análise Estatística de Latências
Este projeto realiza uma análise detalhada das latências, utilizando estatísticas descritivas para identificar anomalias. Inclui a visualização da distribuição das latências com anomalias identificadas.

2. Detecção de Anomalias com RandomForest e Visualização Dash
Combina análise de dados com machine learning para detectar anomalias em tempos de resposta, utilizando um modelo RandomForestClassifier. Inclui também uma aplicação Dash para visualização em tempo real das predições de anomalias.

3. Detecção de Anomalias com LSTM e Isolation Forest
Utiliza um modelo híbrido que combina Isolation Forest e LSTM (Long Short-Term Memory) para detectar anomalias em sequências temporais de latências, oferecendo uma abordagem avançada para identificação de padrões anômalos.

Como Usar

Cada projeto contido neste repositório pode ser executado independentemente. Siga as instruções específicas no README de cada projeto para detalhes sobre a execução, incluindo como carregar os dados, executar os scripts, e interpretar os resultados.

Funcionalidades Gerais

Análise Estatística e Visualização de Dados: Oferece insights sobre o comportamento das latências e identifica anomalias utilizando técnicas estatísticas.
Detecção de Anomalias com Machine Learning: Utiliza modelos de RandomForest e LSTM para detectar anomalias em dados de latência.
Visualização em Tempo Real: Inclui uma aplicação Dash para visualizar as predições de anomalias em tempo real.
Conclusão

Este repositório oferece uma coleção de ferramentas e técnicas para analisar e detectar anomalias em tempos de resposta de serviços. Cada projeto aborda o problema de uma maneira única, proporcionando uma gama de abordagens que podem ser adaptadas ou expandidas conforme necessário para atender a requisitos específicos de análise de dados.
