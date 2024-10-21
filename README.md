# paris-olympic-azure-data-engingeering

## Table of Contents:
- [Overview of the Design](overview-of-the-design)
- [problem Statement](problem-statement)

## Overview of the Design
![Architecture_Design](https://github.com/user-attachments/assets/515b8754-98a5-4046-bd1b-9a98cc15c4df)




## Problem Statement:
```

We have five data tables which are of type CSV. We are performing basic joins in those tables and Creating a Demoralized data frame so that we could perform some processing and Analytics on top of our Data.

```

```sql
SELECT * FROM
ABC;

```

## Dataset:
For this project, we are going to use the [IPL Dataset](https://data.world/raghu543/ipl-data-till-2017). These Datasets consist of three tables customer, orders, and order_items.

## Tech Stack / Skill used:
- Spark
- SQL

## Setting the workspace:
We will use Databricks Community Edition which is free of cost to perform the Spark operations if you prefer to use spark locally or in the Hadoop cluster it’s fine.

Refer: https://www.databricks.com/product/faq/community-edition

After setting up the workspace create a cluster and Open a workbook. You are all set to go.

Project:
Now it's time to add our data to the Databricks.
