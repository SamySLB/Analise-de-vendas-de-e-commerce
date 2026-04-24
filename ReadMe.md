# Analise de Vendas de E-commerce

Projeto de analise de dados com foco em vendas de e-commerce, usando Python, Jupyter Notebook e arquivos preparados para consumo em dashboard. O repositorio cobre desde a limpeza da base ate a exploracao dos dados e a visualizacao de faturamento.

## Objetivo

Organizar, tratar e analisar uma base de vendas online para responder perguntas de negocio como:

- qual o faturamento total do periodo;
- quais categorias e produtos geram mais receita;
- como o faturamento evolui ao longo dos meses;
- quais regioes e meios de pagamento aparecem com mais destaque.

## Estrutura do projeto

```text
.
|-- data/
|   |-- Online Sales Data.csv
|   |-- ecommerce_clean.parquet
|   `-- ecommerce_final.csv
|-- dashboard/
|   |-- dashboard-e-commerce1.png
|   |-- dashboard e-commerce2.png
|   `-- dashboard e-commerce3.png
|-- notebooks/
|   |-- analise_ecommerce.ipynb
|   |-- billing_ecommerce.ipynb
|   `-- explore_ecommerce.ipynb
`-- read.me
```

## Etapas do projeto

### 1. Tratamento dos dados

No notebook `analise_ecommerce.ipynb` a base original e carregada, as colunas sao padronizadas para `snake_case`, registros duplicados sao removidos e o dataset tratado e exportado em dois formatos:

- `ecommerce_clean.parquet`: versao otimizada para analise;
- `ecommerce_final.csv`: versao final para compatibilidade com ferramentas como Power BI.

### 2. Analise exploratoria

No notebook `explore_ecommerce.ipynb` sao analisados:

- estrutura do dataset;
- estatisticas descritivas;
- valores nulos;
- receita total, quantidade de transacoes e volume vendido;
- ranking dos produtos mais vendidos.

### 3. Analise de faturamento

No notebook `billing_ecommerce.ipynb` o foco esta na evolucao temporal das vendas, com agrupamento por mes e geracao de grafico de faturamento mensal.

### 4. Dashboard

A pasta `dashboard/` contem capturas das visualizacoes finais do projeto.

## Base de dados

Arquivo principal: `data/Online Sales Data.csv`

Resumo da base tratada:

- 240 registros;
- 9 colunas;
- periodo analisado de `2024-01-01` a `2024-08-27`;
- 6 categorias de produtos;
- 3 regioes de venda;
- 3 meios de pagamento.

Colunas da base final:

- `transaction_id`
- `date`
- `product_category`
- `product_name`
- `units_sold`
- `unit_price`
- `total_revenue`
- `region`
- `payment_method`


## Tecnologias utilizadas

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Parquet

## Como executar

### 1. Criar e ativar ambiente virtual

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

### 2. Instalar dependencias

```powershell
pip install pandas matplotlib pyarrow notebook
```

### 3. Iniciar o Jupyter

```powershell
jupyter notebook
```

Depois, abra os notebooks da pasta `notebooks/` na ordem sugerida:

1. `analise_ecommerce.ipynb`
2. `explore_ecommerce.ipynb`
3. `billing_ecommerce.ipynb`

## Possibilidades de expansao

- adicionar analise por categoria e por regiao com mais profundidade;
- criar um arquivo `requirements.txt`;




