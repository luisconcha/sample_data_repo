# SAMPLE_DATA_HUB

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Format CSV](https://img.shields.io/badge/Format-CSV-blueviolet)](https://www.ietf.org/rfc/rfc4180.txt)
[![Format JSON](https://img.shields.io/badge/Format-JSON-lightblue)](https://www.json.org/)
[![Spark](https://img.shields.io/badge/Spark-Compatible-brightgreen?logo=apache-spark&logoColor=white)](https://spark.apache.org/)
[![Databricks](https://img.shields.io/badge/Databricks-Ready-red?logo=databricks&logoColor=white)](https://databricks.com/)
[![Data Type](https://img.shields.io/badge/Data-Synthetic-teal)](https://shields.io/)

Repositório público de **dados sintéticos (fake)** para estudos, testes e protótipos em **Data Engineering, Analytics e Machine Learning**.

## 🎯 Propósito

- Disponibilizar **massas de dados fictícias e agnósticas**.
- Formato principal em **CSV**, com expansão futura para **JSON**.
- Uso direto via **URL raw** em notebooks:
  - Databricks
  - Jupyter
  - Google Colab
- Nenhum dado real: **100% gerado para fins educacionais**, ideal para Spark / PySpark.

## 🚀 Como Usar

### Exemplo em PySpark / Databricks

```python
df = spark.read.csv(
    "https://raw.githubusercontent.com/luisconcha/sample-data-hub/main/sales/sales_2021.csv",
    header=True,
    inferSchema=True
)

df.show()
```

## 🗂️ Estrutura do Repositório

```plaintext
sample-data-hub/
├── sales/
│   ├── sales_2021.csv
│   ├── sales_2022.csv
│   ├── sales_2023.csv
│   └── sales_2024.csv
│
├── dre/
│   └── (dados financeiros fictícios, em breve.)
│
├── logistics/
│   └── (dados logísticos fictícios, em breve.)
│
└── README.md

```

Cada diretório representa um domínio de negócio, permitindo estudos independentes ou cruzamentos entre datasets.

## ⚠️ Disclaimer

> Todos os dados disponibilizados neste repositório são totalmente fictícios, gerados de forma sintética com bibliotecas como Faker, exclusivamente para fins de estudo, testes e demonstrações técnicas. Nenhuma informação representa pessoas, empresas ou operações reais.

## 🤝 Créditos e Contato

Repositório desenvolvido por Luis Alberto Concha Curay como parte de um portfólio técnico focado em Engenharia de Dados e Big Data.

- **LinkedIn:** [https://www.linkedin.com/in/luis-alberto-concha-curay/](https://www.linkedin.com/in/luis-alberto-concha-curay/)
- **GitHub:** [https://github.com/luisconcha](https://github.com/luisconcha)
