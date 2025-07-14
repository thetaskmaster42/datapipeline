# Introduction (WIP)

The goal of this project to build to local lakehouse using apache Iceberg with REST Catalog.

Local Lakehouse is build with

1. Pyspark Apache Iceberg
2. Minio for Storage
3. Postgres SQL

## Datapipeline

1. Create a postgres database source as ODS
2. Create a FASTAPI streaming applicaion (WIP)
3. Create a pyspark notebook to read data from different sources.
4. Write a dataset in iceberg format using REST catalog
5. Create a batch pipeline for incrementatal ingestion, transformation in spark.
6. Do some exploratory analysis

## Setup

```bash

cd datapipeline
docker compose up

```

## Notebook

ingestion.ipynb - This notebook walk you through creation of tcph database and ingest the data in to minio and create schema in rest catalog

transform.ipynb - This notebooks walks you through data ingestion, transformation and data validations into silver layer, where Analytics data models are created using star schema

aggregate.ipynb - This notebook helps in defining the aggregate model (data marts) for dashboarding

## Other Query Engine

Dremio is running on localhost:9047 can be configured to minio directly and query the data with sql syntax

