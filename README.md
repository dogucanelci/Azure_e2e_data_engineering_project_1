![image](https://github.com/dogucanelci/Azure_e2e_data_engineering_project_1/assets/59261856/bf084dc4-c403-4b3e-a1c4-f67bdc339f6b)

<h1 style="display: inline-block;">🔧 Analyzing Sales of AdventureWorks 🔌</h1>

<p>On-prem DB to Azure Cloud Pipeline with Data Factory, Lake Storage, Spark, Databricks, Synapse, PowerBI</p>


## 📝 Table of Contents
1. [Project Overview](#introduction)
2. [Key Insights](#key-insights)
3. [Project Architecture](#project-architecture)  
  3.1. [Data Ingestion](#data-ingestion)  
  3.2. [Data Transformation](#data-transformation)  
  3.3. [Data Loading](#data-loading)  
  3.4. [Data Reporting](#data-reporting)
4. [Credits](#credits)
5. [Contact](#contact)

<a name="introduction"></a>
## 🔬 Project Overview 

This an end-to-end data engineering project on the Azure cloud. Where I did data ingestion from a on-premise SQL Server to Azure Data Lake using Data Factory to transformation using Databricks and Spark, loading to Synapse, and reporting using PowerBI. Also, I used Azure Active Directory (AAD) and Azure Key Vault for the data monitoring and governance purpose. 

<a name="project-architecture"></a>
## 📝 Project Architecture

You can find the detailed information on the diagram below:

![AzurePipeline-Hamagistral](https://github.com/Hamagistral/Azure-AW/assets/66017329/ebb0f88b-917f-4a6a-be6b-ddf6093ad793)

<a name="data-ingestion"></a>
### 📤 Data Ingestion
- Connected the on-premise SQL Server with Azure using Microsoft Integration Runtime.

![image](https://github.com/Hamagistral/Azure-AW/assets/66017329/b57debac-28c2-4928-8640-676643e0177c)

- Setup the **Resource group** with needed services (Key Vault, Storage Account, Data Factory, Databricks, Synapse Analytics)

![ressource-group](https://github.com/Hamagistral/Azure-AW/assets/66017329/62990af9-db6e-4712-81bf-61420835bb99)

- Migrated the tables from on-premise SQL Server to Azure Data Lake Storage Gen2.

![image](https://github.com/Hamagistral/Azure-AW/assets/66017329/2b9855a9-9ad7-4ac3-8076-70762ef0f3bc)
![df-pipeline](https://github.com/Hamagistral/Azure-AW/assets/66017329/21ed74aa-8bf4-46c5-952c-4dc9f14dc9fb)

<a name="data-transformation"></a>
### ⚙️ Data Transformation
- Mounted Azure Blob Storage to Databricks to retrieve raw data from the Data Lake.
- Used Spark Cluster in Azure Databricks to clean and refine the raw data.
- Saved the cleaned data in a Delta format; optimized for further analysis.

![image](https://github.com/Hamagistral/Azure-AW/assets/66017329/11b7fb4e-0013-4a9f-a791-ab2a2789f774)

<a name="data-loading"></a>
### 📥 Data Loading
- Used Azure Synapse Analytics to load the refined data efficiently.
- Created SQL database and connected it to the data lake.

![synapse-pipeline](https://github.com/Hamagistral/Azure-AW/assets/66017329/99a8c7cd-1a6f-4ec9-b35d-2e171d3be87b)
![db-synapse](https://github.com/Hamagistral/Azure-AW/assets/66017329/b601eb00-efe1-44d9-8de6-8f001176d549)

<a name="data-reporting"></a>
### 📊 Data Reporting
- Connected Microsoft Power BI to Azure Synapse, and used the Views of the DB to create interactive and insightful data visualizations.

![PowerBI-dashboard](https://github.com/Hamagistral/Azure-AW/assets/66017329/30bb3c61-1503-42a3-8b03-cd7c3da7bb82)

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

[LinkedIn](https://www.linkedin.com/in/hamza-elbelghiti/) •
[Website](https://Hamagistral.me) •
[Gmail](hamza.lbelghiti@gmail.com)
