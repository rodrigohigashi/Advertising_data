# Publicidade Online - Previsão de Cliques com Regressão Logística 📊💻

## Visão Geral do Projeto

Este projeto aplica **regressão logística** para prever a probabilidade de um usuário clicar em um anúncio online, com base em variáveis como idade, tempo gasto no site, renda média da região e uso diário da internet.

A análise inclui **validação cruzada**, **matriz de confusão** e métricas de classificação como **acurácia**, **precisão**, **recall** e **F1-score**, com o objetivo de avaliar o desempenho do modelo em diferentes divisões dos dados.

---

## Objetivos do Projeto

- Prever a probabilidade de cliques em anúncios com base em atributos dos usuários.  
- Avaliar o desempenho da classificação por meio de várias métricas.  
- Aplicar validação cruzada para garantir a robustez do modelo.  
- Explorar o ajuste do limiar de decisão (threshold) para equilibrar precisão e recall.

---

## Conjunto de Dados

O conjunto de dados está localizado em `data/advertising.csv` e inclui:

- `Age`: Idade do usuário  
- `Daily Time Spent on Site`: Tempo gasto no site  
- `Area Income`: Renda média da região do usuário  
- `Daily Internet Usage`: Uso diário da internet (minutos)  
- `Clicked on Ad`: Variável alvo (1 = clicou, 0 = não clicou)

---

## Ferramentas e Tecnologias

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn

---

## Como Executar o Projeto

### 1. Clonar o Repositório

```bash
git clone https://github.com/rodrigohigashi/Advertising_data.git
cd Advertising_data
2. Criar Ambiente Virtual (opcional)

python -m venv venv
Ativar o ambiente:

Windows:

venv\Scripts\activate
Linux/macOS:

source venv/bin/activate
3. Instalar as Dependências

pip install -r requirements.txt
4. Executar o Notebook
Abra no Jupyter Notebook ou no VS Code:

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

Recall médio: 95,8%

F1-score médio: 96,9%

Essas métricas foram obtidas com validação cruzada (5 folds), demonstrando um desempenho forte e consistente do modelo na previsão de cliques em anúncios.

Contribuição
Faça um fork deste repositório.

Crie uma branch para sua feature:

git checkout -b feature/MinhaFeature
Faça as modificações necessárias e dê commit:

git commit -am "Adicionando nova feature"
Envie para seu fork:

git push origin feature/MinhaFeature
Abra um pull request.

Licença
Este projeto está licenciado sob a Licença MIT.
Veja o arquivo LICENSE para mais detalhes.