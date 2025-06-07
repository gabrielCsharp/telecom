# 📊 Análise de Churn de Clientes – Telecom X

Bem-vindo ao projeto de análise de **evasão de clientes (Churn)** da empresa **Telecom X**. Este repositório apresenta um estudo exploratório dos dados de clientes com o objetivo de identificar os principais fatores associados ao cancelamento dos serviços da empresa.

---

## 🎯 Objetivo

A **Telecom X** enfrenta uma taxa significativa de cancelamentos por parte dos clientes. O objetivo deste projeto é:

- Realizar o **tratamento e a limpeza dos dados** fornecidos pela empresa.
- Conduzir uma **Análise Exploratória de Dados (EDA)** para descobrir padrões de comportamento.
- Extrair **insights acionáveis** para auxiliar na tomada de decisões estratégicas voltadas à **retenção de clientes**.

---

## ⚙️ Tecnologias e Bibliotecas Utilizadas

O projeto foi desenvolvido em **Python 3.10+**, utilizando ferramentas amplamente adotadas em ciência de dados:

- **Pandas** e **NumPy** – Manipulação e análise de dados
- **Matplotlib** e **Seaborn** – Visualização de dados
- **Jupyter Notebook** – Desenvolvimento iterativo e visual
- (Opcional) **Plotly**, **Sweetviz** ou **Pandas Profiling** – Para análises complementares e visualizações interativas

---

## 📁 Estrutura do Repositório

```bash
├── Challenge_ETL_telecomX.ipynb              # Notebook com o pipeline de ETL e análise exploratória
├── dataset/
│   └── telecomx_data_gold.csv                # Conjunto de dados tratado (camada "gold")
├── requirements.txt                          # Bibliotecas necessárias para rodar o projeto
└── README.md                                 # Documentação do projeto
```

---

## 🔍 Etapas do Projeto

### 1. 📥 Coleta e Preparação dos Dados
- Extração via **API** no formato **JSON**.
- Normalização e padronização de colunas.
- Conversão e correção de tipos de dados.
- Tratamento de **valores ausentes e inconsistentes**.
- Criação de **variáveis derivadas**, como `Daily_Charges`.

### 2. 📊 Análise Exploratória de Dados (EDA)
- Estudo da variável-alvo `Churn`.
- Análise segmentada por:
  - Tipo de contrato
  - Tempo de permanência (`tenure`)
  - Serviços contratados
  - Forma de pagamento
  - Valor cobrado por dia (`Daily_Charges`)

### 3. 🔗 Análise de Correlação
- Avaliação da relação entre atributos e a variável `Churn`.
- Utilização de **mapas de calor** e **gráficos de dispersão** para facilitar a interpretação.

---

## 📈 Principais Insights

- **Clientes com contrato mensal** apresentam maior propensão ao cancelamento.
- **Curto tempo de permanência** está altamente associado ao churn.
- A ausência de serviços adicionais (como suporte técnico, backup e segurança) aumenta o risco de evasão.
- Clientes com **faturas diárias elevadas** tendem a cancelar com mais frequência.
- A modalidade de **cobrança eletrônica (Paperless Billing)** está correlacionada com maior churn.

---

## ✅ Conclusões e Recomendações

Com base nos achados, recomenda-se:

- Incentivar **contratos de longa duração**, oferecendo benefícios e descontos progressivos.
- Criar **pacotes combinados** com serviços de maior valor percebido.
- Implementar **ações de retenção no início da jornada do cliente**, fase crítica para churn.
- Utilizar campanhas de **reengajamento automatizadas** para clientes com perfil de risco elevado.

---

## 🔮 Próximos Passos

- Aplicar **modelos preditivos de machine learning** para previsão de churn (ex: Random Forest, XGBoost).
- Balancear a variável alvo (`Churn`) utilizando técnicas como **SMOTE**.
- Avaliar desempenho com **validação cruzada** e métricas como AUC, F1-score e precisão.
- Desenvolver **dashboards interativos** com ferramentas como **Power BI**, **Tableau** ou **Plotly Dash**.

---

## 🚀 Como Executar o Projeto

1. **Clone o repositório:**
```bash
git clone https://github.com/albvieiraa/churn-de-clientes-telecom-x.git
```

2. **Crie um ambiente virtual:**
```bash
python -m venv venv
source venv/bin/activate     # Linux/macOS
venv\Scripts\activate        # Windows
```

3. **Instale as dependências:**
```bash
pip install -r requirements.txt
```

4. **Abra o notebook Jupyter:**
```bash
jupyter notebook
```

---

## 👤 Autoria

Projeto desenvolvido por **Maryllian Vieira**, como parte do **Challenge da Trilha de Especialização em Data Science** do programa **ONE: Oracle Next Education**, em parceria com a **Alura**.

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
