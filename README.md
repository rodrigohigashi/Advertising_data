# Adverstising_data

Projeto de Regressão Logística
Descrição
Este projeto implementa um modelo de regressão logística utilizando uma base de dados. O objetivo é prever a probabilidade de um determinado evento ocorrer, com base em variáveis independentes, utilizando a técnica de regressão logística. O modelo foi avaliado utilizando métricas como Acurácia, Precisão, Recall e F1-Score.

Funcionalidades
Carregamento e preparação dos dados.
Criação do modelo de regressão logística.
Treinamento do modelo com divisão de dados em treino e teste (train_test_split).
Avaliação do modelo usando métricas de desempenho.
Visualizações gráficas para análise dos resultados.
Requisitos
Para rodar este projeto, é necessário ter instalado:

Python 3.12.8
Bibliotecas:
pandas
numpy
scikit-learn
scipy
seaborn
matplotlib

Instalação
Clone o repositório:


git clone https://github.com/seu-usuario/seu-repositorio.git
Crie um ambiente virtual:


python -m venv venv
Ative o ambiente virtual:

No Windows:

venv\Scripts\activate
No Linux/macOS:

source venv/bin/activate
Instale as dependências:


pip install -r requirements.txt
Como usar
Preparação dos dados: Carregue a base de dados, ajuste as variáveis, e separe em variáveis dependentes e independentes.

Criação e treinamento do modelo: Utilize a função LogisticRegression do scikit-learn para criar o modelo e treinar com o conjunto de dados de treino.

Avaliação do modelo: Use métricas como Acurácia, Precisão, Recall e F1-Score para avaliar a performance do modelo.

Visualização: Gráficos como curvas ROC, gráficos de dispersão, e outros podem ser gerados para facilitar a interpretação dos resultados.

Exemplos
Aqui está um exemplo de código para rodar o modelo:

'''
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score

# Supondo que 'dados' seja o DataFrame com os dados carregados
X = dados.drop('target', axis=1)  # Variáveis independentes
y = dados['target']  # Variável dependente

# Divisão dos dados em treino e teste
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Criação do modelo
modelo = LogisticRegression()

# Treinamento
modelo.fit(X_train, y_train)

# Previsões
y_pred = modelo.predict(X_test)

# Avaliação do modelo
print(f'Acurácia: {accuracy_score(y_test, y_pred)}')
print(f'Precisão: {precision_score(y_test, y_pred)}')
print(f'Recall: {recall_score(y_test, y_pred)}')
print(f'F1-Score: {f1_score(y_test, y_pred)}')'''

Contribuição
Faça um fork deste repositório.
Crie uma branch para sua feature (git checkout -b feature/MinhaFeature).
Faça as modificações necessárias e commite (git commit -am 'Adicionando nova feature').
Envie as alterações para o seu fork (git push origin feature/MinhaFeature).
Abra um pull request.

Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para mais detalhes.


