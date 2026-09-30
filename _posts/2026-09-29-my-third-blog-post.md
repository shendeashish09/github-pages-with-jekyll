

![Alt Text](https://github.com/shendeashish09/github-pages-with-jekyll/blob/805909c07ad7fd33aef4d843d9818ab9a4cf6f38/assets/Tech_stack.png)

### **Campaign performance Overview **

An integrated reporting platform, featuring visualization dashboards and an array of data management tools to help streamline processes, ensure data quality and compliance. It enables basic reporting at scale in order to realign resources to higher value tasks and outputs. 


### **Project Overview** 

- The Baseline product is deployed on Microsoft Azure and is built using various Azure services, including Azure Data Factory (ADF), Azure SQL Database, Azure Blob Storage, Azure Logic Apps, and Azure Key Vault. 

- The product ingests delivery data from multiple advertising and media platforms through the Adverity API, including: 

   - Google Campaign Manager, Google Ads, DV360, SA360. 

   - Amazon, The Trade Desk (TTD). 

   - Facebook, LinkedIn, Snapchat, TikTok, Reddit, Pinterest, Twitter/X. 

   - IAS, DoubleVerify (DV), MOAT, and other platforms. 

- The product also supports data ingestion from Google Cloud Storage (GCS) and email, with the data initially stored in Azure Blob Storage and subsequently loaded into the corresponding Azure SQL Database tables. 

- Planned data (Prisma) is ingested from the GroupM Data Warehouse (Mediaocean). 

- Once delivery and planned data are ingested, the Business Rules (BR) pipeline performs data transformations, joins delivery and planned data, and applies the required business logic and validations. 

- Final reporting tables are prepared for Power BI visualization and reporting. 

- The product also supports exporting reporting data to external destinations, including Google Cloud Storage (GCS), Amazon S3 via SFTP. 

**6** 

 

### **Numerous data connections available in Baseline** 






 

### **Baseline | Product Map** 

###### Delivery Data Sources 

###### Planned Data 

- Universal ADF pipeline for all the delivery data sources. 

   - Planned data (Prisma) is ingested from the GroupM Data Warehouse (Mediaocean). 

- Adverity data streams for all the API platforms. 

   - ADF pipeline on boards prisma data from 6 different agencies across US,UK, and Canada. 

- Monitoring and alerts for platform data ingestion. 

- Data Validation and QA with platforms. 

      - Connected with offline data. 

   - Site serve data ingestion via web portal. 

- Supports Display, search, social and verification data sources. 

###### Business Rules 

###### Web Portal 

- The Business Rules (BR)  Web portal provides pipeline performs data following capabilities: transformations, joins  Site serve process. 

- delivery and planned data,  Data classifications. 

- and applies the required business logic and  Orphan transitions. validations.  

      - Site serve process. 

      - Data classifications. 

      - Orphan transitions. 

      - Placement merging. 

   - Data Sourcing & Normalization. 

      - Run reports. 

      - Custom reports. 

   - Orphan Identification 

   - Units Decisioning 

   - Creative Reallocation 

- Site serve process. 

- Spend Calculations 





###### Power BI Reports 

   - Power BI Report has following Dashboards. 

      - Cross Channel View 

      - Campaign Performance 

      - Facebook/Instagram 

      - Conversion Performance 

      - Search Campaign Performance 

      - Placement and Creative Performance 

      - Pacing Analysis. 

      - Programmatic In-Depth 

      - Advertiser Overview 

      - Other Social platforms. 

- Final Reporting. 

>  **8** 

### **Business Rules Description** 

|**#**||**Baseline Table Name**|**Description**|
|---|---|---|---|
|0||Orphan Identification|Ensures all data is pulled in|
|1|**rcing &**<br>**zation**|Units Decisioning|Determine Units source of truth|
|2|**ata Sou**<br>**Normali**|Creative Reallocation|Combine with metrics of different granularity|
|3|**D**<br>|Placement Merging|Mapping to combine placements|
|4|**ns**|Final Billable Units|Assign metric to use in calculating cost|
|5|**lculatio**|Calculated Spend|Mathematical calculation on delivered spend|
|6|**end Ca**|Spend Decisioning|Determine spend source of truth|
|7|**Sp**|Delivered Units and Spend|Logic for determining spend in case of under/over-<br>delivery and reconciliation|
|8|**ting**|Final BR Output|Puts together all the units and spend logic along<br>with Prisma metadata|
|9|**al Repor**|Final Conversion|Includes conversions/custom actions needed for<br>reporting|
|10|**Fin**|Final Reporting|Combines BR Output and Final Conversion data|







- **Multi-step process to define source of truth for units-delivery, spend and conversion for digital buys** 

- **Broken up into smaller steps to prevent computing one massive calculation in one go** 

- **If any step of the calculation fails, Data Ops can rerun from that step rather than restarting from the beginning** 



 

### **Baseline Ecosystem** 





|**Ongoing data processing workflow**<br>|||
|---|---|---|
|Data<br>Processing<br>Final Table<br>Aggregation<br>**Prisma**validation, naming<br>checks and decisioning<br>Automated<br>Data<br>Collection<br>Raw<br>Input QA<br>**API & FTPs**<br>Raw Data<br>Streams<br>a<br>|Final Data<br>QA<br>Data exports<br>|Reports &<br>Visuals<br>Release to<br>Client<br>Insights<br>and Visuals<br>|
|Baseline Process<br>Quality<br>Control<br>Quality<br>Control<br>Revise data that<br>falls outside of 2%<br>margin of<br>discrepancy<br>**Managed by Client Team**<br>Manual Data<br>Collection<br>|Quality<br>Control<br>Resolve all<br>surfaced<br>discrepancies<br>Baseline<br>|Planning<br>QA<br>Planning<br>Feedback<br>Align on<br>comments,<br>questions &<br>concerns<br>|
|Baseline Process<br>|Copyright © 2026 Cybage Soft       i<br>Final Tables<br>|**11**<br>ware Pvt. Ltd. All Rights Reserved. Cybage Confidential.<br>11<br>|



### **Tools and Technologies** 







#### Baseline Tech Stack 




 

### **Cybage Footprint | Service Offerings** 

#### Brand Onboarding & Ownership 

#### Monitoring & Alerts 

- New brand onboarding and end-to-end responsibility for setting up all required resources. 

   - Adverity Monitoring 

      - Monitor data streams and ingestion status. 

      - Identify failed or delayed data loads. 

- Integration of planned and delivery data into pipelines and activation of the baseline process. 

   - Track missing campaigns and data issues. 

- Data validation and QA across platforms. 

   - ADF Monitoring 

      - Monitor pipeline and trigger execution. 

- Streamlining the site-served and orphan processes. 

   - Identify and troubleshoot pipeline failures. 

- Setting up and maintaining data classification and taxonomy processes. 

- Management of reporting pipeline schedules to minimize delays. 

#### Data Classification & Custom Reporting 

- Provide engineering support for custom reports, custom transformations, and reporting integrations. 

- Build and maintain custom data classifications. 

- Setup of offline data streams. 

- Support the development of features that improve campaign management efficiency and automation. 

- Pipeline and query optimization for time- and cost-efficient data processing. 




#### Product Engineering 

- Product support through dedicated Data Engineering and Support teams. 

- Enhancement of product capabilities for monitoring and optimization. 

- Implementation of robust pipeline management for complex workflows and data handling. 

- Design and development of data pipelines. 

   - Monitoring of Adverity data streams. 

   - Materialization of reporting views. 

   - Development and maintenance of generic Prisma pipelines. 



### **Screenshot | Campaign Performance Dashboard** 


### **Screenshot | Pacing Analysis** 



- The Pacing Analysis view was designed with our planning teams in mind. This page contains clean and simple visuals that provide users with an understanding of their media delivery versus their planned media. 












