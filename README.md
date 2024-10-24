# paris-olympic-azure-data-engingeering
> This project is to analyze Olympic data using various tools and technologies, including Azure Data Factory, Data Lake Gen 2, Synapse Analytics, and Azure Databricks.

# Table of Contents
- [Overview of the Design](overview-of-the-design)
- [Problem Statement](problem-statement)
- [Dataset](Dataset)
- [Tech Stack](Tech-Stack)
- [Azure Services](Azure-Services)

# Overview of the Design
![Architecture_Design](https://github.com/user-attachments/assets/515b8754-98a5-4046-bd1b-9a98cc15c4df)

# Dataset
For this project, we are going to use the kaggle dataset : [Paris 2024 Olympic Summer Games Dataset](https://www.kaggle.com/datasets/piterfm/paris-2024-olympic-summer-games). 

We are considering following four tables within the [data](https://github.com/nk3099/paris-olympic-azure-data-engingeering/tree/main/data) folder:
- [athletes.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/athletes.csv)
- [coaches.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/coaches.csv)
- [medals.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/medals.csv)
- [teams.csv](https://github.com/nk3099/paris-olympic-azure-data-engingeering/blob/main/data/teams.csv)

# Tech Stack
- PySpark
- SQL
- Azure
- Databricks

# Azure Services:
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

# Setting the workspace:
![setting_workspace](https://github.com/user-attachments/assets/2941ea54-9abe-4157-9021-6e76d4d2ed88)


# Databricks-backed secret scope
A Databricks-backed secret scope is stored in (backed by) an encrypted database owned and managed by Azure Databricks.\
![paris-olympic-scopes](https://github.com/user-attachments/assets/aac172ae-657e-4d6b-b97b-8bf102417ddb)

## Steps:

1.Install Databricks CLI and configure with your workspace. \
```
1.pip install databricks-cli
2.databricsk configure --help
3.databricks configure --token
4.Go to C:\Users\.databrickscg (databricks configuration file) and make sure host_url and token is pasted correctly.
```

![configure-databricks-cli](https://github.com/user-attachments/assets/fbae4641-71a9-4306-8c08-86562670478c)

2.Creating databricks-backed secret scope commands:
```
1.databricks secrets create-scope --scope <scope-name> --initial-manage-principal users
2.databricks secret put --scope <scope-name> --key <key-name>
3.databricks secrets list --scope <scope-name>
4.databricks secrets delete-scope --scope <scope-name>
```
![scopes](https://github.com/user-attachments/assets/03580fcb-e38c-4fe4-8ef0-861595a1f8da)




![synapse-sql](https://github.com/user-attachments/assets/4c878f9e-9779-4c0b-b991-7a6bd4959c5c)


