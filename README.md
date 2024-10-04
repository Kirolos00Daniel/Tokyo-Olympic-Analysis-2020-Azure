# Tokoyo-Olympic-Analysis-2020-Azure
Tokyo Olympics Analysis Using AZURE platform

# Azure Data Pipeline Project

## Overview

This project demonstrates an end-to-end data pipeline using Azure services for data ingestion, transformation, and analytics. The pipeline is designed to facilitate data flow from various sources into a data lake, transform the data, and finally visualize it through dashboards using Power BI.

<img width="566" alt="Azure" src="https://github.com/user-attachments/assets/5f8ff2ff-29ec-42a2-ba6c-b252e9c74ba2">


## Architecture

### 1. Data Source
- **Description:** The data source can be any structured or unstructured data, such as databases, files, or external APIs.
- **Role:** It serves as the initial point of data entry into the pipeline.

### 2. Data Ingestion with Azure Data Factory
- **Azure Data Factory:** A cloud-based data integration service used to create data-driven workflows for orchestrating and automating data movement and transformation.
- **Raw Data Store:** The ingested data is stored in its raw format in the Data Lake Gen 2.

### 3. Raw Data Store (Data Lake Gen 2)
- **Description:** Azure Data Lake Storage Gen 2 provides a highly scalable and secure data lake for big data analytics.
- **Role:** It stores the ingested raw data, serving as a staging area before transformation.

### 4. Data Transformation with Azure Databricks
- **Azure Databricks:** An Apache Spark-based analytics platform optimized for Azure. It is used for large-scale data processing and machine learning.
- **Role:** It performs data transformations, cleaning, and enrichment before loading the transformed data back into the Data Lake.

### 5. Transformed Data Store (Data Lake Gen 2)
- **Description:** After transformation, the clean and structured data is stored back in Data Lake Gen 2.
- **Role:** This data serves as the source for further analytics and reporting.

### 6. Analytics with Azure Synapse Analytics
- **Azure Synapse Analytics:** An integrated analytics service that accelerates time to insight across data warehouses and big data systems.
- **Role:** It provides data exploration and analytics capabilities, enabling complex queries and insights on the transformed data.

### 7. Dashboards and Reporting
- **Tools:** Power BI, Looker Studio, Tableau.
- **Role:** These tools are used to create interactive dashboards and reports for data visualization and business insights.

## How It Works

1. **Data Ingestion:**
   - Data from various sources is ingested using Azure Data Factory and stored in a raw format in Data Lake Gen 2.


![Ingestion using APIs](https://github.com/user-attachments/assets/a342b1db-5ccb-4c78-9d35-3cc5cc8b5fec)

2. **Data Transformation:**
   - Azure Databricks processes the raw data, performing transformations such as filtering, aggregation, and data enrichment.


![Databriks 1](https://github.com/user-attachments/assets/4c0ee840-53ee-4b10-acd4-4dbbeba8d4ac)


3. **Data Storage:**
   - Transformed data is stored in Data Lake Gen 2, making it ready for analytics and reporting.


![Screenshot 2024-10-04 093918](https://github.com/user-attachments/assets/9c9fe14e-fbd9-45cb-8abd-5f785ee81a27)


4. **Data Analytics:**
   - Azure Synapse Analytics is used for querying and analyzing the transformed data, creating a bridge between big data and data warehousing.


![synapse2](https://github.com/user-attachments/assets/653a0f51-f598-4652-9031-c1f8b8f074f5)


5. **Data Visualization:**
   - Visualization tools such as Power BI, Looker Studio, and Tableau connect to Azure Synapse Analytics for creating dashboards that provide insights into the data.


![Screenshot 2024-10-04 093631](https://github.com/user-attachments/assets/f2ed867c-92b4-4bb5-af8f-c92dec6ac08c)


## Prerequisites

- **Azure Subscription:** Required for accessing Azure services like Data Factory, Databricks, and Synapse Analytics.
- **Data Sources:** Identify and configure the data sources for ingestion.
- **Visualization Tools:** Power BI, Looker Studio, or Tableau installed and configured.

## Setup and Deployment

1. **Provision Azure Services:**
   - Set up Azure Data Factory, Data Lake Gen 2, Databricks, and Synapse Analytics within your Azure subscription.

2. **Configure Data Ingestion:**
   - Create pipelines in Azure Data Factory to ingest data from the source to the Data Lake.

3. **Create Databricks Notebooks:**
   - Develop Databricks notebooks for data transformation processes and connect them to the raw data stored in Data Lake.

4. **Setup Synapse Analytics:**
   - Configure Azure Synapse Analytics to connect with the transformed data in Data Lake for querying and analysis.

5. **Build Dashboards:**
   - Use visualization tools to connect to Synapse Analytics and create interactive dashboards and reports.

## Conclusion

This project outlines a scalable and efficient data pipeline using Azure's suite of tools. It allows for seamless data ingestion, transformation, and visualization, enabling businesses to gain valuable insights from their data.
