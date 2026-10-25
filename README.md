# 🦠 Análise Exploratória de Dados — Ebola na África Subsaariana

Projeto acadêmico de **Análise Exploratória de Dados (EDA)** sobre registros históricos relacionados ao Ebola na África Subsaariana, abrangendo o período de 2014 a 2026. O trabalho explora padrões temporais e geográficos, indicadores epidemiológicos, relações entre variáveis e técnicas de análise estatística e aprendizado de máquina.

O projeto foi desenvolvido em Python como parte da atividade de Análise Exploratória de Dados da Faculdade Impacta de Tecnologia.

---

## 🎯 Objetivos

- Explorar a distribuição dos registros epidemiológicos por país e período.
- Investigar o comportamento da taxa de letalidade e dos casos confirmados.
- Preparar, limpar e transformar os dados para análise.
- Construir visualizações para identificar padrões e possíveis associações.
- Aplicar técnicas de inferência estatística, regressão linear e clusterização.
- Comunicar os resultados por meio de um relatório executivo e de um cartaz informativo.
- Documentar as limitações dos dados e seus impactos na interpretação dos resultados.

## 🛠️ Tecnologias utilizadas

| Tecnologia | Aplicação |
|---|---|
| Python | Linguagem principal |
| Pandas e NumPy | Manipulação, limpeza e transformação dos dados |
| Matplotlib e Seaborn | Visualização de dados |
| Plotly | Visualizações interativas |
| SciPy | Testes estatísticos e intervalos de confiança |
| Scikit-learn | Regressão e clusterização |
| Jupyter Notebook | Desenvolvimento e documentação das análises |

## 📁 Estrutura do projeto

```text
EP-EDA-EBOLA/
├── dados/
│   └── ebola_historico_africa_subsaariana_2014_2026.xlsx
├── notebooks/
│   └── EP_Ebola_EDA.ipynb
├── resultados/
│   ├── figs/
│   ├── Relatorio_Executivo_Ebola_OMS.pdf
│   └── Cartaz_Campanha_Ebola.png
├── .gitignore
├── requirements.txt
└── README.md
```

*Os nomes e caminhos dos arquivos acima devem corresponder aos arquivos efetivamente presentes no repositório.*

## 🔬 Etapas da análise

### 1. Preparação e tratamento dos dados
- Inspeção da estrutura e dos tipos das variáveis.
- Verificação de valores ausentes e registros duplicados.
- Investigação de possíveis valores atípicos.
- Criação de variáveis derivadas e indicadores para as análises.

### 2. Análise exploratória de dados
- Distribuição dos registros por país e ano.
- Evolução temporal dos casos e da taxa de letalidade.
- Comparações entre países e períodos.
- Análise de distribuições e correlações.
- Construção de gráficos para apoiar a interpretação dos padrões identificados.

### 3. Análise estatística e modelagem
- Estimação de intervalo de confiança de 95% para a taxa média de letalidade.
- Testes de hipóteses para comparação entre grupos.
- Teste de associação por qui-quadrado com variáveis categorizadas.
- Regressão linear simples para investigar a relação entre dias até a internação e taxa de letalidade.
- Aplicação do algoritmo K-Means para explorar agrupamentos de registros.

### 4. Comunicação dos resultados
- Relatório executivo com resultados, interpretações e recomendações.
- Cartaz informativo com mensagens relacionadas à prevenção e ao enfrentamento do Ebola.

## 📊 Principais resultados

Entre os resultados obtidos na base analisada, destacam-se:

- **57,22%:** taxa média de letalidade registrada.
- **56,75% a 57,70%:** intervalo de confiança de 95% calculado para a média.
- **0,5507:** coeficiente de determinação (\(R^2\)) da regressão linear na amostra utilizada pelo modelo.
- **73,90%:** previsão estimada pelo modelo para o cenário de 10 dias até a internação.

Esses resultados são descritivos e exploratórios. Não devem ser interpretados isoladamente como estimativas oficiais da epidemiologia do Ebola ou como evidência de causalidade.

## ⚠️ Limitações da análise

A interpretação dos resultados considera as seguintes limitações:

- A base não contém registros observados de óbitos, sobrevivência individual ou acesso individual à UTI.
- Os óbitos derivados da taxa de letalidade são estimativas, não contagens observadas.
- A disponibilidade de leitos hospitalares por 10 mil habitantes não equivale ao acesso individual à UTI.
- Algumas análises utilizam variáveis categorizadas ou aproximações para viabilizar comparações estatísticas.
- As médias móveis calculadas sobre registros não representam necessariamente intervalos de dias consecutivos.
- Os resultados da regressão e da clusterização dependem das variáveis, dos registros disponíveis e das escolhas metodológicas.
- Os padrões encontrados representam associações na base analisada e não comprovam relações de causa e efeito.

Por essas razões, as conclusões devem ser interpretadas dentro do escopo e das limitações do conjunto de dados utilizado.

## ▶️ Como executar o projeto

### Pré-requisitos

- Python 3.10 ou superior.
- Git.
- Jupyter Notebook ou JupyterLab.

### 1. Clone o repositório

```bash
git clone https://github.com/marialuiza-mdealcantara/EP-EDA-EBOLA.git
cd EP-EDA-EBOLA
```

### 2. Crie e ative um ambiente virtual

No Windows, usando PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

### 4. Abra o notebook

```bash
jupyter notebook
```

Abra `notebooks/EP_Ebola_EDA.ipynb` e execute as células na ordem apresentada.

> **Importante:** os caminhos utilizados para carregar a planilha e salvar os gráficos devem ser compatíveis com a estrutura de diretórios do projeto.

## 📄 Resultados e materiais

- **Notebook:** [`notebooks/EP_Ebola_EDA.ipynb`](notebooks/EP_Ebola_EDA.ipynb)
- **Relatório executivo:** [`resultados/Relatorio_Executivo_Ebola_OMS.pdf`](resultados/Relatorio_Executivo_Ebola_OMS.pdf)
- **Cartaz informativo:** [`resultados/Cartaz_Campanha_Ebola.png`](resultados/Cartaz_Campanha_Ebola.png)

## 👩‍💻 Autoria

**Maria Luiza Moreira de Alcantara**

Projeto acadêmico desenvolvido para a disciplina de Análise Exploratória de Dados — Faculdade Impacta de Tecnologia.

---

*Este projeto tem finalidade acadêmica e educacional. As análises não substituem dados epidemiológicos oficiais nem avaliações realizadas por profissionais de saúde pública.*
