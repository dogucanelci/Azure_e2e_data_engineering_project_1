![image](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/bf084dc4-c403-4b3e-a1c4-f67bdc339f6b)

<h1 style="display: inline-block;">🔧 Analyzing Sales of AdventureWorks 🔌</h1>

<p>On-prem DB to Azure Cloud Pipeline with Data Factory, Lake Storage, Spark, Databricks, Synapse, PowerBI</p>


## 📝 Table of Contents
1. [Project Overview](#introduction)
2. [Project Architecture](#project-architecture)  
  2.1. [Data Ingestion](#data-ingestion)  
  2.2. [Data Transformation](#data-transformation)  
  2.3. [Data Loading](#data-loading)  
  2.4. [Data Reporting](#data-reporting)
3. [Credits](#credits)
4. [Contact](#contact)

<a name="introduction"></a>
## 🔬 Project Overview 

This an end-to-end data engineering project on the Azure cloud. Where I did data ingestion from a on-premise SQL Server to Azure Data Lake using Data Factory to transformation using Databricks and Spark, loading to Synapse, and reporting using PowerBI. Also, I used Azure Active Directory (AAD) and Azure Key Vault for the data monitoring and governance purpose. 

<a name="project-architecture"></a>
## 📝 Project Architecture

You can find the detailed information on the diagram below:

![1_project_str](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/f0fdf9eb-5b61-4f18-806f-2d8f5d2cef13)


<a name="data-ingestion"></a>
### 📤 Data Ingestion
- Connected the on-premise SQL Server with Azure using Microsoft Integration Runtime.

![2_IR](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/a2e6d6ee-5b67-4e16-8c99-4c54a1488d5a)


- Setup the **Resource group** with needed services (Key Vault, Storage Account, Data Factory, Databricks, Synapse Analytics)

![3_resource_group](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/659df9b6-c624-4244-beed-70bd74d06bbc)

- Migrated the tables from on-premise SQL Server to Azure Data Lake Storage Gen2.

![4_containers](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/fd073c15-f09b-4bcf-97fa-4105ea033d25)

![5_pipeline_1](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/0c54279a-f1d0-4ee1-bd54-1de8a77fe913)


<a name="data-transformation"></a>
### ⚙️ Data Transformation
- Mounted Azure Blob Storage to Databricks to retrieve raw data from the Data Lake.
- Used Spark Cluster in Azure Databricks to clean and refine the raw data.
- Saved the cleaned data in a Delta format; optimized for further analysis.

![6_databricks_bronze_to_silver](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/de9fcd1a-39ec-4d6e-8c07-6520d23f1886)

![7_databricks_silver_to_gold](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/105e2c61-629d-4c96-becd-2518f7db46cc)


<a name="data-loading"></a>
### 📥 Data Loading
- Used Azure Synapse Analytics to load the refined data efficiently.
- Created SQL database and connected it to the data lake.

![8_synapse_pipeline](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/068eeb10-86e0-4122-b172-6480409f8fa4)

![9_gold_db_views](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/7b2d362a-15ce-4716-a3cc-96434156c446)

<a name="data-reporting"></a>
### 📊 Data Reporting
- Connected Microsoft Power BI to Azure Synapse, and used the Views of the DB to create interactive and insightful data visualizations.

![10_powerbi_report](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/67e3b07b-44f3-448b-b774-202b28850015)


### 🛠️ Technologies Used

- **Data Source**: SQL Server
- **Orchestration**: Azure Data Factory
- **Ingestion**: Azure Data Lake Gen2
- **Storage**: Azure Synapse Analytics
- **Authentication and Secrets Management**: Azure Active Directory and Azure Key Vault
- **Data Visualization**: PowerBI

<a name="credits"></a>
## 📋 Credits

- This Project is inspired by the video of the [YouTube Channel "Mr. K Talks Tech"](https://www.youtube.com/watch?v=iQ41WqhHglk)  

<a name="contact"></a>
## 📨 Contact Me

[LinkedIn](https://www.linkedin.com/in/elcidogucan/)
[Website](https://www.dogucanelci.com)
[Gmail](dogucanelci@gmail.com)
