# Anúncio na Internet

Esse repositório contém um projeto de **regressão logística** para prever cliques em anúncios online. A estrutura está dividida em duas pastas de idioma, além dos dados e dependências:

Advertising_data/
├── data/
│ └── advertising.csv # Dataset com informações de anúncios
├── EN/
│ ├── logistic-regression-project.ipynb
│ └── README_EN.md # Documentação em inglês
├── PT/
│ ├── projeto-de-regressao-logistica.ipynb
│ └── README_PT.md # Documentação em português
├── requirements.txt # Lista de dependências
└── README.md # Este arquivo


---

## Escolha seu idioma

- 🇧🇷 [Português](PT/README_PT.md)  
- 🇺🇸 [English](EN/README_EN.md)

---

## Como rodar

1. **Clone** o repositório  
   ```bash
   git clone https://github.com/seu-usuario/Advertising_data.git
   cd Advertising_data
(Opcional) Crie e ative um ambiente virtual

python -m venv venv
# Windows
venv\Scripts\activate
# Linux/macOS
source venv/bin/activate
Instale as dependências


pip install -r requirements.txt
Abra o notebook na pasta desejada

Português:

cd PT
jupyter notebook projeto-de-regressao-logistica.ipynb
English:

cd EN
jupyter notebook logistic-regression-project.ipynb
Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.



### Ajustes no `README_PT.md`
No seu `PT/README_PT.md`, valide se:

1. **Caminho do CSV** aponta para `../data/advertising.csv`.
2. A seção “Como rodar” faça `cd PT` antes de abrir o notebook.
3. A árvore do projeto reflita apenas o conteúdo de `PT/`.

Por exemplo, no topo do `README_PT.md`:

```markdown
# Anúncio na Internet (Português)

📂 **Estrutura desta pasta**

├── projeto-de-regressao-logistica.ipynb
├── README_PT.md

E no carregamento dos dados:

```python
dados = pd.read_csv('../data/advertising.csv', sep=',')