# Análise de Vendas de E-commerce – Projeto de Data Analytics

Este projeto tem como objetivo aplicar técnicas de engenharia, análise e visualização de dados sobre um dataset de vendas de e-commerce.  
O fluxo foi desenvolvido utilizando Python (Pandas, Matplotlib) para limpeza e exploração dos dados, e Power BI para criação de um dashboard interativo.

---

## Objetivos do Projeto

- Realizar ingestão e padronização do dataset
- Aplicar limpeza, tratamento e otimização de tipos de dados
- Gerar estatísticas descritivas e análises exploratórias
- Produzir visualizações profissionais em Python
- Exportar dados preparados para o Power BI
- Criar um dashboard completo com indicadores chave de desempenho (KPIs)

---

## 1. Preparação e Limpeza dos Dados  
**Notebook: analise_ecommerce.ipynb**

### Etapas realizadas

**Leitura do dataset original**  
- Carregamento realizado com `pandas.read_csv()` usando dtypes otimizados

**Padronização dos nomes das colunas**  
- Conversão para letras minúsculas  
- Remoção de espaços  
- Formatação no padrão `snake_case`

**Limpeza e tratamento**  
- Remoção de duplicatas  
- Remoção de linhas inválidas  
- Tratamento de valores ausentes  
- Conversão de datas e tipos numéricos

**Exportação otimizada**  
Salvamento do DataFrame limpo em formato Parquet:
python

## 2. Análise Exploratória  
**Notebook: explore_ecommerce.ipynb**

### Principais etapas da EDA

- Resumo dos dados (`df.info()`)
- Estatísticas descritivas (`df.describe()`)
- Contagem de valores nulos
- Cálculo de indicadores gerais:
  - Receita total
  - Número de transações
  - Total de unidades vendidas
- Identificação dos 10 produtos mais vendidos

---

## 3. Visualizações em Python

Foram criados gráficos para análise inicial, incluindo:

- Faturamento mensal (gráfico de linha)
- Top 10 produtos mais vendidos (gráfico de barras)
- Distribuição de vendas
- Análises complementares para geração de insights

---

## 4. Exportação para Power BI

O dataset final foi exportado para CSV para consumo no Power BI:

```python
df.to_csv('data/ecommerce_final.csv', index=False)

df.to_parquet('data/ecommerce_clean.parquet', index=False)
