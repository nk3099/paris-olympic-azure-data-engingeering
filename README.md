# paris-olympic-azure-data-engingeering
> This project is to analyze Olympic data using various tools and technologies, including Azure Data Factory, Data Lake Gen 2, Synapse Analytics, and Azure Databricks.

### Table of Contents
- [Overview of the Design](overview-of-the-design)
- [Problem Statement](problem-statement)
- [Dataset](Dataset)
- [Tech Stack](Tech-Stack)
- [Azure Services](Azure-Services)

### Overview of the Design
![Architecture_Design](https://github.com/user-attachments/assets/515b8754-98a5-4046-bd1b-9a98cc15c4df)

### Dataset
For this project, we are going to use the kaggle dataset : [Paris 2024 Olympic Summer Games Dataset](https://www.kaggle.com/datasets/piterfm/paris-2024-olympic-summer-games). 

We are considering following four tables within the [data](https://github.com/nk3099/paris-olympic-azure-data-engingeering/tree/main/data) folder:
- [athletes.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/athletes.csv)
- [coaches.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/coaches.csv)
- [medals.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/medals.csv)
- [teams.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/teams.csv)

### Tech Stack
- PySpark
- SQL
- Azure

## Azure Services:
**Data Factory:** 
```
Data integration service that enables you to create, schedule, and manage data pipelines for efficient data movement and transformation between various sources and destinations in Azure and beyond. It simplifies ETL (Extract, Transform, Load) and data integration tasks.
```

**Data Lake Gen 2:** 
```
Data lake solution that combines the capabilities of a data lake with the power of Azure Blob Storage, allowing you to store and analyze large volumes of structured and unstructured data with enhanced performance, security, and analytics capabilities.
```

**Azure Databricks:**
```
Databricks is a unified analytics platform built on top of Apache Spark, designed to help data engineers and data scientists collaborate on big data processing and machine learning tasks. It provides tools for data exploration, data processing, and building machine learning models in a collaborative and scalable environment.
```
**Synapse Analytics:**
```
SQL Data Warehouse, is a cloud-based analytics service provided by Microsoft Azure. It combines big data and data warehousing into a single integrated platform, allowing organizations to analyze and process large volumes of data for business intelligence and data analytics purposes.
```

## Setting the workspace:
We will use Databricks Community Edition which is free of cost to perform the Spark operations if you prefer to use spark locally or in the Hadoop cluster it’s fine.

Refer: https://www.databricks.com/product/faq/community-edition

After setting up the workspace create a cluster and Open a workbook. You are all set to go.

Project:
Now it's time to add our data to the Databricks.
