# Microsoft Azure Interview/Academic Questions

1. [Cloud Computing](#cloud_computing)
      * [Azure Models](#azure_models)
3. [Azure Services](#azure_services)
      * [General](#general)
      * [Storage Account](#storage_account)
      * [Key Vault]($key_vault)

<a name="cloud_computing"></a>
## Cloud Computing
<a name="azure_models"></a>
### Azure Models
#### Q: What's the differences between different cloud models: PaaS, IaaS, SaaS?
A:<br/>
**1) PaaS: Platform As A Service** - in that model user doesn't have to care about platform settings, access to OS, OS configuration, Web Service configuration etc. Such information are totally transparent to him. Only what he needs to know is how to deploy an application to the particular "platform". In Azure PaaS examples are: Azure CDN, Azure Search, App Service<br/>
**2) IaaS: Infrastructure As A Service** - IaaS "hide" internal communications betwen objects as: Network, Antivirus, Operating System, Clusters etc. Examples: Virtual Machines, Azure Kubernetes Service<br/>
**3) SaaS: Software As A Service** - delivers full software platform and/or SDK Suite for developers. Only what the user needs to do is to make a configuration. Scalability & platform is transparent. Example: Office 356, Azure IoT Suite
<a name="azure_services"></a>
## Azure Services
<a name="general"></a>
### General
#### Q: Describe most popular Azure Services 
A:
| Service | Description |
| --- | --- |
|Virtual Machine | Dedicated image of OS system |
|Azure Virtual Scale Set | Feature that supports autoscaling between VMs. Load Balancer is created automatically |
|Azure Functions | Serverless "container" for development code (C# Java Script, Python, Java) | 
|AKS, Azure Container Service | Container orchestrator (Kubernetes, DC/OS, Swarm) |
|Azure Container Instances | Containers for Windows and Linux | 
|Azure Container Registry | Container repo (like Docker Hub) |
|Azure Batch | Job scheduling and in automatically scaling and managing virtual machines running those jobs|
|Azure Service Fabric | Distributed framework for microservice/container development and lifecycle management|
|Azure Virtual Network |Service that allows to close object into safety virtual network |
|Azure Load Balancer | Smart traffic manager for distributing load between VMs |
|Azure Application Gateway |Round robin load balancer for HTTP traffic |
|Azure VPN Gateway|VPN for Virtual Networks |
|Azure DNS|DNS Server for Azure objects|
|Azure Content Delivery Network|Content delivery network bundle capable of handling most content delivery network workloads|
|Azure Traffic Manager|High-availability ensurement for endpoint monitoring and automatic reconnection after failure|
|Azure Express Route|Dynamic routing between on-prem network and Azure|
|Azure DDOS Protection|Cost-free Azure protection against Distributed Denial Of Services attacks|
|Azure Network Watcher|Monitoring and diagnisis of the Azure network resources|
|Azure Storage|Storage for BLOBS, structured data (tables), file sharing and queues|
|Azure Data Lake Storage|Storage for Big Data solutions|
|Azure Storsimple|Synchronization between on-prem and Azure Storage|
|Azure Site Recovery |Replication of application running on VMs and/or physical machines from the master localization to backup|
|Azure App Service|Serverless App container|
|Azure Web App|Serverless Web Application hosted on IIS|
|Azure Mobile Apps|Simple service for Mobile App backend development|
|Azure Logic App|PaaS for workflow and business logic modelling|
|Azure API Apps|Web API services, integrated part of Web Apps|
|Azure Search|Content searcher based on Elasticsearch|
|Azure Notification Hub|Service for sending Push Notification. Can be integrated with iOS, Android and Windows|
|Azure SQL Database|Database based on SQL Server engine. User has a possibility to choose also MySQL and PostgreSQL engine|
|Azure SQL Data Warehouse|Enterprise data warehouse in PaaS model|
|Azure Cosmos DB|NoSQL database in PaaS model|
|Azure Redis Cache|Service for fast and save cache memory|
|Azure Database Migration Service|Service supports migration process from on-premis to cloud database|
|Azure HDInsight|Managed platform for Big Data analysis|
|Azure Data Bricks|Analytical platform based on Azure Spark|
|Azure Stream Analytics|Data Stream processing with ML|
|Azure Bot Service|Virtual Partner Implementation in Azure|
|Azure Data Lake Analytics|Job-based service for Big Data Analysis|
|Azure Data Factory|Data Set factory between different data sources|
|Azure Data Catalog|Registry for different type of Data (SQL, NoSQL)|
|Azure Log Analytics|Service for logging and monitoring Azure objects|
|Azure Analysis Service|Paas for well known SQL Server Analysis Services|
|Azure Maps|Mapping service based on Bing engine|
|Azure Custom Speech Service|Azure AI text to speech|
|Azure Event Hub|Service designed for streaming huge amount of data|
|Azure IOT Hub|Platform for IoT Device management|
|Azure DPS|IoT Device Provisioning Service|
|Azure Active Directory|Identity and access management center|
|Azure KeyVault|Secure database for storing secrets|

<a name="storage_account"></a>
### Storage Account
#### Q: How many different Storage Accounts Azure offer?
A: There's 4 types of Storage Accounts:<br/>  
**1) BLOB Storage** - designed for storing images, files with distributed access, logs etc.<br/>
**2) Table Storage** - designed for storing structured NoSQL data.<br/>
**3) Queue Storage** - designerd for storing large number of messages (access via HTTPS).<br/> 
**4) (Shared) File Storage** - designed for storing fully managed file shares.<br/>
#### Q: What's Shared Access Signature?
A: SAS is a hash key including into Storage Account/Container/Blob URI that guaarantees restricted access to that objects. SAS can be generated with validity period (for example for 1 month only)
#### Q: How much storage VM can use?
A: Data Disk contains up to 1 TB free space, however it's possible to link more than one disk to the VM

<a name="key_vault"></a>
### Key Vault
#### Q: What kind of secrets Azure Key Vault can protect?
A: Keys, Certificates and Secrets
