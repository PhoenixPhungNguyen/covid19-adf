# Covid-19 Cases Data Analysis in Europe

## Overview
(What is the project about)

## Table of contents
1. Overview []
2. Project Structure []
...

## Architecture
(High level Data flow)

## Project Structure

- 📂 **PhoenixPhungNguyen-covid19-adf/**
  - 📄 README.md
  - 📄 publish_config.json
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

![msedge_kbiNQDhTxw](https://github.com/user-attachments/assets/c364680d-2058-484e-9ba5-ed705481014b)

-    Pipelines : ingest population, load case deaths, hospital admissions, testing, process population,case deaths, hospital admission, testing data
      ![msedge_BpNFFQ0E60](https://github.com/user-attachments/assets/f4a007b8-4662-490d-aee1-fac8ec97a9c1)
     
      ![image](https://github.com/user-attachments/assets/15b3ac81-7b49-4e1b-9bea-2d9c101e73a7)
      ![msedge_o33bUlBMQk](https://github.com/user-attachments/assets/a77d887b-3373-4555-b705-5107472277a4)
      ![msedge_Byu7iPCUwM](https://github.com/user-attachments/assets/f4457f1e-608d-4ab6-a13b-6bdd083505cd)

     ![msedge_f8CvhrDHPT](https://github.com/user-attachments/assets/2d38ed63-9ae7-4045-b532-02678f1f2991)
    ![msedge_UwLhn2ZguE](https://github.com/user-attachments/assets/1caa44fd-2cde-43e3-ac9d-8ce8ae4a4485)
    ![msedge_LvAEtIWntK](https://github.com/user-attachments/assets/8e35ef77-7658-4b2b-abd1-4b02c19f4d76)
    ![msedge_w2iz4sThII](https://github.com/user-attachments/assets/06b44b1d-aeaf-4e51-9797-7de20552c9c0)

-    Data flows : Transform case dealths, hospital admissions and testing data
  ![msedge_hlbOTge8JJ](https://github.com/user-attachments/assets/c0b429ee-3841-4fa5-8e56-0a248ad2afac)
![msedge_pa9FAT6ZBa](https://github.com/user-attachments/assets/8282dec9-c4c1-4149-b6b5-3d3605ea559a)
![image](https://github.com/user-attachments/assets/2365c748-89ab-40e3-a8ed-fa681ead52fd)

**2. Azure Databricks** 
- Workspace:
  ![msedge_e2MI8ZkUDV](https://github.com/user-attachments/assets/1ca0274e-4947-4000-8fe5-60bbba9c06f7)
- Compute:
  ![msedge_DiFLZWyQaN](https://github.com/user-attachments/assets/4db60832-7482-4f6f-a221-98f77e9f7fd7)

**3. Azure Data Lake Gen 2**
![image](https://github.com/user-attachments/assets/5051c0f2-894a-4a9b-825c-3bf3aa506563)
![msedge_7VxbOb86GX](https://github.com/user-attachments/assets/45326fbc-1baa-40b8-9ef7-3f0a466d2763)
![msedge_pEkutKj1Xw](https://github.com/user-attachments/assets/02876888-b555-4048-9849-ec1f86bb088c)

![msedge_BlzgfzhaZu](https://github.com/user-attachments/assets/78a60b9e-34da-42e9-ae19-ffebcda2d30b)

![msedge_yzXnFjsOcz](https://github.com/user-attachments/assets/6de5e243-6115-433f-9867-4f456cb4d642)
![msedge_HQsKRvEuGe](https://github.com/user-attachments/assets/d96916c9-1137-45e0-b0c8-4a47e52798aa)

**4. Azure SQL DB**
![msedge_G6QaeZss5v](https://github.com/user-attachments/assets/d5d86692-946d-4bb4-95e8-dcd24b4f1618)

**5. Power BI**
- **Covid trends by country**
  ![wps_gFyf0lhUSM](https://github.com/user-attachments/assets/35febf08-6395-4b3a-b6b9-c791e374c7d9)
  ![wps_NwlMyWX6xl](https://github.com/user-attachments/assets/b69813c8-3702-4fca-859d-3593105cc6c1)

- **Covid testing cases**
  ![wps_b8Fjd6NBnM](https://github.com/user-attachments/assets/85aee825-12d8-4161-a03a-8c13bb5ade53)


