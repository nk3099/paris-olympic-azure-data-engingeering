# paris-olympic-azure-data-engingeering
> This project is to analyze Olympic data using various tools and technologies, including Azure Data Factory, Data Lake Gen 2, Synapse Analytics, and Azure Databricks.

## Table of Contents:
- [Overview of the Design](overview-of-the-design)
- [Problem Statement](problem-statement)
- [Dataset](Dataset)

## Overview of the Design
![Architecture_Design](https://github.com/user-attachments/assets/515b8754-98a5-4046-bd1b-9a98cc15c4df)

## Dataset:
For this project, we are going to use the kaggle dataset : [Paris 2024 Olympic Summer Games Dataset](https://www.kaggle.com/datasets/piterfm/paris-2024-olympic-summer-games). 

We are considering following four tables within the [data](https://github.com/nk3099/paris-olympic-azure-data-engingeering/tree/main/data) folder:
- [athletes.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/athletes.csv)
- [coaches.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/coaches.csv)
- [medals.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/medals.csv)
- [teams.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/teams.csv)

## Tech Stack / Skill used:
- Spark
- SQL

## Setting the workspace:
We will use Databricks Community Edition which is free of cost to perform the Spark operations if you prefer to use spark locally or in the Hadoop cluster it’s fine.

Refer: https://www.databricks.com/product/faq/community-edition

After setting up the workspace create a cluster and Open a workbook. You are all set to go.

Project:
Now it's time to add our data to the Databricks.
