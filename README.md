# Tokyo Olympics Data Engineering Playground

This project is a playground to explore various Azure solutions for data engineering. It involves ingesting, transforming, and analyzing data from the [Tokyo 2020 Olympics](https://www.kaggle.com/datasets/aliaamiri/2020-summer-olympics-dataset) using several Azure services.

## Overview

The goal is to practice and understand the end-to-end data engineering process using Azure's ecosystem. The data pipeline includes the following steps:

1. **Data Ingestion:** Using Azure Data Factory to load data from a CSV file into Azure Data Lake Storage (ADLS).
2. **Data Transformation:** Utilizing Azure Databricks to perform data transformations and store the transformed data back into ADLS.
3. **Data Analytics:** Using Azure Synapse Analytics to further analyze the transformed data annd load them into a SQL database.
4. **Data Visualization:** Displaying the final results using Power BI Embedded.

## Architecture

![Data Architecture](https://github.com/lkolebka/tokyo-olympics-data-engineering/blob/0878974e28b7599c20e60118f4b2c7a672bcf40c/architecture.drawio.png)

## Steps

### 1. Data Ingestion
- **Azure Data Factory:** Ingests raw data from a CSV file into a Data Lake (ADLS Gen2).

### 2. Data Transformation
- **Azure Databricks:** Processes and transforms the ingested data, then stores it back in the Data Lake in a cleaner version.

### 3. Data Analytics
 **Azure Synapse Analytics:**
- Transform the clean csv into a datalake database to perform advanced analytics using SQL.
- Loop the Data Lake storage to create proper SQL table using Azure SQL 

### 4. Data Visualization
- **Power BI Embedded:** Visualizes the final data for insights.

This project serves as a practical exercise to understand how different Azure services can be integrated to create a comprehensive data engineering solution.
