# Covid-19 Cases Data Analysis in Europe

## Overview
This project focuses on analyzing the spread and impact of COVID-19 across European countries using publicly available datasets. 
The goal is to uncover insights from the pandemic data through data preprocessing, visualization, and time-series analysis.

## Table of contents

## Architecture

<img src="images/7.covid19_architecture_prj.png"/>

## Project Structure

- 📂 **PhoenixPhungNguyen-covid19-adf/**
  - 📄 README.md
  - 📄 publish_config.json
  - 📂 images/
  - 📂 dataflow/   
  - 📂 dataset/    
  - 📂 factory/
  - 📂 linkedService/
  - 📂 pipeline/
  - 📂 trigger/

## Data Source
Covid 19 Data in Europe from website https://www.ecdc.europa.eu/en

## Tech Stack
**1. Azure Data Factory**

<img src="images/azure_datafactory_pipeline.png" width="400"/>

-    Linked Service
Create linked service to connect ADF with Azure Data Lake Storage Gen2

<img src="images/covid19_dataset_lookup_linkservice_datalake.png" width="600"/>
<img src="images/covid19_dataset_process_linkservice_datalake.png" width="600"/>
<img src="images/covid19_dataset_raw_linkservice_datalake.png" width="600"/>

Create linked service to connect ADF with Azure Blob Storage

<img src="images/covid19_dataset_source_linkservice_blob.png" width="600"/>

Create linked service to connect ADF with Azure SQL Database

<img src="images/covid19_dataset_source_linkservice_blob.png" width="600"/>

-  Create new dataset

<img src="images/covid19_dataset.png" width="400"/>

-    Pipelines : ingest population, load case deaths, hospital admissions, testing, process population,case deaths, hospital admission, testing data
  
<p align="left">
      <img src="images/copydata_caseDeath.png" width="300"/>
      <img src="images/copydata_hospitalAdmissionsDaily.png" width="300"/>
      <img src="images/copydata_testing.png" width="300"/>
</p>
 <img src="images/pipeline_caseDeaths.png"/>
 <img src="images/pipeline_hospitalAdmissions.png"/>
 <img src="images/pipeline_testing.png"/>
 <img src="images/copydata_population.png"/>
  
-    Data flows : Transform case dealths, hospital admissions and testing data
  
<p align="left">   
      <img src="images/dataflow_caseDeaths.png" width="300"/>
      <img src="images/dataflow_hospitalAdmission.png" width="300"/>
      <img src="images/dataflow_testing.png" width="300"/>
      <img src="images/databrick_population.png" width="300"/>
</p>

- Trigger:

  <img src="images/covid19_trigger.png" width="700"/>
  
**2. Azure Databricks** 

- Workspace:
  
   <img src="images/databrick_workspace.png" width="700"/>
- Compute:
  
   <img src="images/databrick_compute.png" width="700"/>

**3. Azure Data Lake Gen 2**

- resource group
  
  <img src="images/azure_resourcegroup.png" width="700"/>
- raw
 
<img src="images/azure_raw_ecdc.png" width="700"/>
<img src="images/azure_raw_population.png" width="700"/>

-lookup

<img src="images/azure_lookup.png" width="700"/>
- process
  
<img src="images/azure_process_ecdc.png" width="700"/>
<img src="images/azure_process_population.png" width="700"/>

**4. Azure SQL DB**
- Create access control (IAM) and add role assignment
  
<img src="images/covid19-reporting-app.png" width="700"/>

<img src="images/azure_sqldb.png" width="700"/>

**5. Power BI**

- **Covid trends by country**
  
<img src="images/covid19_dashboard1.png"/>
<img src="images/covid19_dashboard2.png"/>

- **Covid testing cases**
  
<img src="images/covid19_dashboard3.png"/>
 

