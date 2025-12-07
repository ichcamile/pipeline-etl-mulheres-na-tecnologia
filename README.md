# 🚀 Pipeline de ETL Integrado — Mulheres na Tecnologia

Este projeto faz parte de um **desafio prático de dados** com o objetivo de entender o **cenário global da mulher na tecnologia**, utilizando um **Pipeline de ETL integrado**, desde a extração dos dados até a visualização final em dashboard.

O projeto simula um contexto real, onde atuamos como **analistas de dados da WoMakersCode**, utilizando múltiplas fontes e ferramentas modernas do ecossistema de dados.

---

## 🎯 Propósito do Projeto

Os dados estão por toda parte — e, neste projeto, usamos dados para:

- Entender o cenário da mulher na tecnologia  
- Apoiar decisões baseadas em dados  
- Exercitar conceitos reais de **engenharia e análise de dados**  
- Construir um pipeline completo, automatizado e confiável  

---

## 🧱 Conceito de ETL

O projeto segue o conceito tradicional de **ETL (Extract, Transform, Load)**:

### 🔹 Extract (Extrair)
- Coleta de dados brutos a partir de diferentes fontes  
- Ex: arquivos CSV, JSON, bancos de dados ou APIs  

### 🔹 Transform (Transformar)
- Limpeza, padronização e validação dos dados  
- Enriquecimento e organização das informações  
- Preparação dos dados para análise  

### 🔹 Load (Carregar)
- Armazenamento dos dados transformados em um **Data Warehouse**
- Disponibilização para consumo analítico e visualização  

Também exploramos o conceito de **ELT**, onde parte da transformação ocorre após o carregamento.

---

## 🛠️ Ferramentas Utilizadas

- **Python**  
- **Pandas** — Manipulação e transformação de dados  
- **SQLite** — Data Warehouse local  
- **dbt** — Transformações e modelagem dos dados  
- **Prefect** — Orquestração e automação do pipeline  
- **Google Colab** — Ambiente de desenvolvimento  
- **Power BI** — Criação de dashboards e visualizações  

---

## 🗂️ Estrutura do Projeto

```text
├── data/
│   ├── raw/              # Dados brutos (extração)
│   ├── processed/        # Dados tratados
│   └── warehouse/        # Banco SQLite
│
├── etl/
│   ├── extract.py        # Extração dos dados
│   ├── transform.py     # Transformações
│   └── load.py           # Carga no Data Warehouse
│
├── dbt/
│   └── models/           # Modelos e transformações dbt
│
├── orchestration/
│   └── pipeline.py       # Fluxo orquestrado com Prefect
│
├── dashboard/
│   └── powerbi.pbix      # Dashboard final
│
├── README.md
└── requirements.txt
