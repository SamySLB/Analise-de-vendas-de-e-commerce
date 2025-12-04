Análise de Vendas de E-commerce – Projeto de Data Analytics

Este projeto tem como objetivo aplicar técnicas de engenharia, análise e visualização de dados sobre um dataset de vendas de e-commerce.
O fluxo foi desenvolvido utilizando Python (Pandas, Matplotlib) para limpeza e exploração dos dados, e Power BI para criação de um dashboard interativo.


🚀 Objetivos do Projeto

Realizar ingestão e padronização do dataset.

Aplicar limpeza, tratamento e otimização de tipos de dados.

Gerar estatísticas descritivas e análises exploratórias.

Produzir visualizações profissionais em Python.

Exportar dados preparados para o Power BI.

Criar um dashboard completo com indicadores chave de desempenho (KPIs).

🧼 1. Preparação e Limpeza dos Dados (Notebook: analise_ecommerce.ipynb)
✔ Leitura do dataset original

Carregamento realizado com pandas.read_csv() usando dtypes otimizados.

✔ Padronização dos nomes das colunas

Conversão para letras minúsculas

Remoção de espaços

Estrutura uniforme no formato snake_case

✔ Limpeza e tratamento

Remoção de duplicatas

Remoção de linhas inválidas

Tratamento de valores ausentes

Conversão de datas e tipos numéricos

✔ Exportação otimizada

Salvamento do DataFrame limpo em formato Parquet:

df.to_parquet('data/ecommerce_clean.parquet', index=False)

🔎 2. Análise Exploratória (Notebook: explore_ecommerce.ipynb)

As principais etapas incluem:
 Resumo dos dados

df.info()

Estatísticas descritivas (df.describe())

Contagem de valores nulos

Indicadores gerais

Receita total

Número de transações

Unidades vendidas

 10 produtos mais vendidos


3. Visualizações em Python

Foram criados gráficos exploratórios como:

Faturamento mensal (linha)

Top produtos mais vendidos (barras)

Distribuição de vendas

Análises complementares para insights

📤 4. Exportação para Power BI

O dataset final foi exportado para .csv para ser utilizado no Power BI:

df.to_csv('data/ecommerce_final.csv', index=False)

📈 5. Dashboard no Power BI
📍 KPIs incluídos

Receita total

Número de transações

Total de unidades vendidas

Ticket médio


 Tecnologias de transformação

Power Query

DAX para medidas personalizadas

🛠 Tecnologias Utilizadas
Ferramenta / Biblioteca	Uso
Python	ETL e análise exploratória
Pandas	Limpeza e manipulação de dados
Matplotlib	Visualizações
Parquet	Armazenamento eficiente
Power BI	Dashboard
VS Code	Desenvolvimento
Git/GitHub	Versionamento
