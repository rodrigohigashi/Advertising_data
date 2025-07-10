
Anúncio na Internet - Análise e Previsão de Performance 📊💻

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


=======
Visão Geral do Projeto

Este projeto tem como objetivo a criação de um modelo de machine learning para prever a performance de anúncios na internet. Utilizando dados históricos de campanhas publicitárias, o modelo de regressão linear é aplicado para prever o desempenho dos anúncios, com foco em variáveis como o valor investido, o tipo de anúncio, e os resultados obtidos em termos de cliques, conversões e vendas.

A análise inclui métricas como R² (coeficiente de determinação), validação cruzada, e erros de previsão, com o intuito de entender a precisão do modelo e identificar as principais variáveis que afetam a performance dos anúncios.

Objetivos do Projeto:
Prever o desempenho de anúncios na internet, com base em variáveis como o orçamento investido, tipo de anúncio, e outros parâmetros.
Analisar a relação entre as variáveis e a performance dos anúncios.
Implementar técnicas de validação cruzada e análise de erros para avaliar o desempenho do modelo.
Utilizar a regressão linear como modelo principal para prever cliques e conversões.
Dataset
O conjunto de dados utilizado contém informações sobre campanhas de anúncios, incluindo variáveis como:

Orçamento: Valor investido na campanha.
Tipo de Anúncio: O formato do anúncio (ex: display, pesquisa, vídeo).
Cliques: Número de cliques obtidos pelo anúncio.
Conversões: Número de conversões realizadas a partir do anúncio.
Vendas: Vendas realizadas através dos cliques no anúncio.
Tamanho: Aproximadamente 2.000 registros.

Ferramentas e Tecnologias
Python: Linguagem principal para desenvolvimento.
Pandas: Manipulação e análise dos dados.
Scikit-learn: Implementação da regressão linear e validação cruzada.
Matplotlib & Seaborn: Visualizações dos dados e resultados.
Como Rodar o Projeto
Clone o Repositório

Primeiro, clone o repositório para sua máquina local:

git clone https://github.com/seu-usuario/anuncio-na-internet.git
cd anuncio-na-internet
Instale as Dependências

Instale as dependências necessárias para rodar o projeto:

pip install -r requirements.txt
Execute o Script de Análise

Execute o script principal para rodar a análise e gerar as previsões:

python analise_anuncio.py
Acesse os Resultados

O modelo gerará os resultados da previsão de cliques, conversões e vendas, e exibirá as métricas de performance do modelo, como R² e Erro Médio Absoluto (MAE).

Estrutura do Projeto

anuncio-na-internet/
├── data/
│   └── anuncios.csv             # Dataset com informações de anúncios
├── analise_anuncio.py          # Script principal com a análise
├── requirements.txt            # Lista de dependências
└── README.md                   # Documentação do projeto
Análise de Resultados
R² (Coeficiente de Determinação): O R² mede a capacidade do modelo em explicar a variabilidade dos dados. Quanto mais próximo de 1, melhor o modelo se ajusta aos dados.
Erro Médio Absoluto (MAE): Este valor indica o erro médio do modelo nas previsões.
Validação Cruzada: A validação cruzada foi utilizada para garantir a robustez do modelo e avaliar sua performance em diferentes subconjuntos de dados.
Lições Aprendidas
A regressão linear mostrou-se uma boa abordagem inicial para a previsão da performance de anúncios, embora existam outras técnicas que podem ser exploradas para um modelo mais complexo.
A validação cruzada é essencial para avaliar a robustez do modelo, especialmente em conjuntos de dados limitados.
O modelo pode ser ajustado com novas variáveis, como a segmentação do público-alvo e a análise de diferentes canais de anúncios.
Melhorias Futuras
Explorar outros modelos de machine learning, como árvores de decisão e redes neurais, para melhorar a acurácia das previsões.
Incluir variáveis adicionais, como a segmentação demográfica e comportamental dos usuários, para prever de forma mais precisa a conversão.
Implementar técnicas de otimização, como regularização, para evitar o overfitting e melhorar o desempenho do modelo.
=======
# Anúncio na Internet - Previsão de Cliques com Regressão Logística 📊💻

## Visão Geral do Projeto

Este projeto aplica **regressão logística** para prever a probabilidade de um usuário clicar em um anúncio online, com base em variáveis como idade, tempo no site, área de interesse, entre outras.

A análise inclui o uso de **validação cruzada**, **matriz de confusão** e métricas como **acurácia**, **precisão**, **revocação** e **F1-score**, visando avaliar a performance do modelo em diferentes divisões dos dados.

---

## Objetivos do Projeto

- Prever a probabilidade de cliques em anúncios com base em variáveis do usuário.
- Analisar métricas de classificação para avaliar o desempenho do modelo.
- Aplicar validação cruzada para garantir robustez e evitar overfitting.
- Explorar o impacto do ajuste do limiar de decisão (threshold).

---

## Dataset

O conjunto de dados está localizado em `data/advertising.csv` e contém:

- `Age`: Idade do usuário  
- `Daily Time Spent on Site`: Tempo médio gasto no site  
- `Area Income`: Renda média da região do usuário  
- `Daily Internet Usage`: Uso médio diário da internet  
- `Clicked on Ad`: Variável alvo (1 = clicou, 0 = não clicou)

---

## Ferramentas e Tecnologias

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn

---

## Como Rodar o Projeto

### 1. Clone o Repositório

```bash
git clone https://github.com/rodrigohigashi/Advertising_data.git
cd Advertising_data

2. Crie o Ambiente Virtual (opcional)

python -m venv venv
Ative o ambiente:

Windows: venv\Scripts\activate

Linux/macOS: source venv/bin/activate

3. Instale as Dependências

pip install -r requirements.txt

4. Execute o Notebook
Abra o Jupyter Notebook ou use o VS Code para executar:

cd PT
jupyter notebook projeto-de-regressao-logistica.ipynb

Estrutura do Projeto

Advertising_data/
├── data/
│   └── advertising.csv
├── EN/
│   └── logistic-regression.ipynb
│   └── README_EN.md
├── PT/
│   └── projeto-de-regressao-logistica.ipynb
│   └── README_PT.md
├── requirements.txt
└── README.md

Resultados e Métricas

Acurácia média: 97,0%
Precisão média: 98,2%
Revocação média: 95,8%
F1-score médio: 96,9%

Esses resultados foram obtidos com validação cruzada (5 folds), indicando um modelo robusto e confiável para prever cliques em anúncios.

Licença
Este projeto está licenciado sob a Licença MIT.


