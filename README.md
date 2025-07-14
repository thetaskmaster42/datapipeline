# Introduction

The goal of this project to build to local lakehouse using apache Iceberg with REST Catalog.

Local Lakehouse is build with

1. Pyspark Apache Iceberg
2. Minio for Storage
3. Postgres SQL
ßß
## Datapipeline

1. Create a postgres database source as ODS
2. Create a FASTAPI streaming applicaion (WIP)
3. Create a pyspark notebook to read data from different sources.
4. Write a dataset in iceberg format using REST catalog
5. Create a batch pipeline for incrementatal ingestion, transformation in spark.
6. Do some exploratory analysis