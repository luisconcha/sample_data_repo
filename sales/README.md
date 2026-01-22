# 📦 Sales Dataset (Synthetic)

Dataset sintético de **vendas** utilizado para estudos, testes e protótipos em
**Data Engineering, Analytics, PySpark e Databricks**.

Todos os dados são **fictícios**, gerados para simular cenários reais de operação
comercial, logística, marketing e avaliação de clientes.

---

## 🎯 Objetivo do Dataset

- Simular um **processo completo de vendas**
- Permitir estudos de:
  - métricas comerciais
  - performance logística
  - comportamento do cliente
  - funil de vendas
  - análise financeira (receita, lucro, desconto)
- Servir como massa de dados para:
  - Spark / PySpark
  - Databricks
  - Pandas
  - DuckDB

---

## 📊 Volume e Período

- **Período:** 2021 a 2024
- **Registros por arquivo:** 300.000
- **Tamanho médio por arquivo:** ~78 MB
- **Formato:** CSV
- **Separador:** `,`
- **Encoding:** UTF-8
- **Dados:** 100% sintéticos

---

## 🗂️ Estrutura do Diretório

```text
sales/
├── sales_2021.csv
├── sales_2022.csv
├── sales_2023.csv
├── sales_2024.csv
└── README.md
```

Cada arquivo representa um ano completo de vendas.

## 🧱 Schema do Dataset

| Campo                  | Tipo    | Descrição                                      |
| ---------------------- | ------- | ---------------------------------------------- |
| `id_pedido`            | string  | Identificador único do pedido                  |
| `id_cliente`           | integer | Identificador do cliente                       |
| `nome_cliente`         | string  | Nome fictício do cliente                       |
| `segmento_cliente`     | string  | Segmento do cliente (ex: Standard, Premium)    |
| `data_pedido`          | date    | Data de criação do pedido                      |
| `data_envio`           | date    | Data de envio do pedido                        |
| `data_entrega`         | date    | Data de entrega do pedido                      |
| `data_cancelamento`    | date    | Data de cancelamento (quando aplicável)        |
| `tempo_entrega_dias`   | integer | Tempo de entrega em dias                       |
| `pais`                 | string  | País do cliente                                |
| `estado_cliente`       | string  | Estado do cliente                              |
| `cidade_cliente`       | string  | Cidade do cliente                              |
| `id_loja`              | integer | Identificador da loja                          |
| `nome_loja`            | string  | Nome da loja                                   |
| `cidade_loja`          | string  | Cidade da loja                                 |
| `estado_loja`          | string  | Estado da loja                                 |
| `produto`              | string  | Nome do produto                                |
| `categoria`            | string  | Categoria do produto                           |
| `sub_categoria`        | string  | Subcategoria do produto                        |
| `qtd`                  | integer | Quantidade vendida                             |
| `custo_unitario`       | decimal | Custo unitário do produto                      |
| `preco_unitario`       | decimal | Preço unitário de venda                        |
| `vl_desconto_unitario` | decimal | Valor de desconto unitário                     |
| `vl_total_bruto`       | decimal | Valor total bruto do pedido                    |
| `vl_total_liquido`     | decimal | Valor total líquido após descontos             |
| `lucro_pedido`         | decimal | Lucro do pedido                                |
| `status_pedido`        | string  | Status do pedido (Entregue, Cancelado, etc.)   |
| `canal_venda`          | string  | Canal de venda (E-commerce, Loja Física, etc.) |
| `forma_pagamento`      | string  | Forma de pagamento                             |
| `utm_source`           | string  | Origem da campanha (marketing)                 |
| `utm_medium`           | string  | Meio da campanha                               |
| `utm_campaign`         | string  | Nome da campanha                               |
| `avaliacao_nota`       | decimal | Nota de avaliação do pedido                    |
| `avaliacao_comentario` | string  | Comentário da avaliação                        |

---

## 🧪 Casos de Uso Sugeridos

- Receita e lucro por período
- Tempo médio de entrega por estado
- Taxa de cancelamento
- Análise de desconto vs lucro
- Avaliação de clientes por segmento
- Performance de campanhas (UTM)


## ⚠️ Disclaimer

> Todos os dados deste diretório são totalmente fictícios, gerados de forma sintética
para fins educacionais e demonstrativos. Nenhuma informação representa pessoas, empresas ou operações reais.