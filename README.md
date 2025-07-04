# ifood-case
Códigos e desenvolvimento do case-ifood para a posição de Data Architect

# 🗂️ Case de Dados com Databricks

Este projeto apresenta um case de dados completo, estruturado com ingestão, pré-processamento, análise exploratória e geração de outputs com base em dados de corridas de táxi da cidade de Nova York. A infraestrutura utilizada inclui Databricks, PySpark e arquivos armazenados no Amazon S3.

---

## 📚 Objetivo

Processar e analisar os dados brutos de corridas de táxi da cidade de Nova York, realizando o tratamento, limpeza, enriquecimento e análise dos dados para gerar insights úteis.

---
## 🧾 Dados

Os dados estão armazenados em um bucket S3:
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/green-taxi/
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/green-taxi/green_tripdata_2023-01.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/green-taxi/green_tripdata_2023-02.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/green-taxi/green_tripdata_2023-03.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/green-taxi/green_tripdata_2023-04.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/green-taxi/green_tripdata_2023-05.parquet



https://datalake-joao.s3.us-east-2.amazonaws.com/landing/yellow-taxi/
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/yellow-taxi/yellow_tripdata_2023-01.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/yellow-taxi/yellow_tripdata_2023-02.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/yellow-taxi/yellow_tripdata_2023-03.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/yellow-taxi/yellow_tripdata_2023-04.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/landing/yellow-taxi/yellow_tripdata_2023-05.parquet

## e depois de preprocessados foram disponibilizados na camada de consumo do s3:

https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/green_taxi_curated/
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/green_taxi_curated/part-00000-61de26cc-2a30-4409-975c-c1d265ecf960.c000.snappy.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/green_taxi_curated/part-00000-e355b209-72ea-4a2e-b2c2-54a3782f530b.c000.snappy.parquet

https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/yellow_taxi_curated/
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/yellow_taxi_curated/part-00000-96a89111-154c-4f08-8d01-dbaf8a623357.c000.snappy.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/yellow_taxi_curated/part-00000-a7fc7bdc-1ac0-4327-831d-77d99bbd43e1.c000.snappy.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/yellow_taxi_curated/part-00001-56844ce1-128c-418d-9b47-3c17e05c397c.c000.snappy.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/yellow_taxi_curated/part-00001-79b0e82f-c244-4f97-ba67-547ecf0ac901.c000.snappy.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/yellow_taxi_curated/part-00002-e6e3e67e-44c8-43c6-a96a-8a674248253d.c000.snappy.parquet
https://datalake-joao.s3.us-east-2.amazonaws.com/consumo/yellow_taxi_curated/part-00003-53099eb4-bcea-4bae-b2cd-c73500757ed8.c000.snappy.parquet


▶️ Como executar no Databricks
https://dbc-4fe4d292-522d.cloud.databricks.com/editor/notebooks/365069125504093?o=1988599547531691
Faça login com o usuário fornecido

Vá para: Repos → ifood-case → analysis → notebook

Conecte ao cluster ifood-cluster

Execute o notebook Preprocessing_final.ipynb

Em seguida, execute o notebook Analyzing_final.ipynb
