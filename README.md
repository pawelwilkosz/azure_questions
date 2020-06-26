# Microsoft Azure Interview/Academic Questions

1. [Cloud Computing](#cloud_computing)
      * [Azure Models](#azure_models)
3. [Azure Services](#azure_services)
      * [General](#general)
      * [Storage Account](#storage_account)
      * [Key Vault](#key_vault)
4. [Troubleshooting](#troubleshooting)
     * [Health Check](#health_check)
5. [Security](#security)
     * [Identity](#identity)

<a name="cloud_computing"></a>
## Cloud Computing
<a name="azure_models"></a>
### Azure Models
#### Q: What's the differences between different cloud models: PaaS, IaaS, SaaS?
A:<br/>
**1) PaaS: Platform As A Service** - in that model user doesn't have to care about platform settings, access to OS, OS configuration, Web Service configuration etc. Such information are totally transparent to him. Only what he needs to know is how to deploy an application to the particular "platform". In Azure PaaS examples are: Azure CDN, Azure Search, App Service. In PaaS model:
- Client is responsible on: Data, Application
- Cloud provider is responsible on: Runtime, Middleware, OS, Servers, Virtualizations, Storage, Networking<br/>
**2) IaaS: Infrastructure As A Service** - IaaS "hide" internal communications betwen objects as: Network, Antivirus, Operating System, Clusters etc. Examples: Virtual Machines, Azure Kubernetes Service. User doesn't have influence how network looks like and which HW/SW components are choosen to build infrastructure<br/>
In IaaS model:
- Client is responsible on: Data, Application, Runtime, Middleware, OS
- Cloud provider is responsible on: Virtualization, Servers, Storage, Networking
**3) SaaS: Software As A Service** - delivers full software platform and/or SDK Suite for developers. Only what the user needs to do is to make a configuration. Scalability & platform is transparent. Example: Office 356, Azure IoT Suite
In SaaS model client is responsible on Data only, the rest of Cloud Stack is in Cloud provider's responsibility
<a name="azure_services"></a>
#### Q: What's Azure Resource Group?
A: Resource group is a logical group collector for Azure objects/assets
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
#### Q: Is there any limit of file count on BLOB Storage?
A: There's no limit on file count however there's a limit on storage size (500TB). 
#### Q: What's Storage Account Soft Delete?
A: Soft delete protects file against accidentially deletion. When the option is enabled and user performs delete on particular object, Azure marked it as "Deleted" without phisically removal

<a name="key_vault"></a>
### Key Vault
#### Q: What kind of secrets Azure Key Vault can protect?
A: Keys, Certificates and Secrets

#### Q: How can you grant access to e.g. list secrets/certificates?
A: Access is configured per secret type, separate for: Keys, Certificates and Secrets. 

#### Q: What's a differences between keys and secrets?
A: Info abput Keys: https://docs.microsoft.com/pl-pl/azure/key-vault/keys/about-keys
Info about Secrets: https://docs.microsoft.com/pl-pl/azure/key-vault/secrets/about-secrets

###Virtual Machines
####Q: What's Virtual Machine Scale Set?
A: Service for creating load balancing VMs.

<a name="troubleshooting"></a>
## Troubleshooting
<a name="health_check"></a>
### Health Check
#### Q: How to check maintenance scheduled by Microsoft by itself?
A: Go to the Azure Portal -> Service Health -> Planned Maintenance

<a name="security"></a>
## Security
<a name="identity"></a>
### Identity
#### Q: What's Identity As A Service in Microsoft Azure?
A: It's SaaS-based Identity Access Management (IAM) that allows to use Single Sign-On authentication from your organization (on-premises AD) and access control

#### Q: What's a different way to create identity in Azure AD?
A: It can be: adding user in Azure AD, invite user via Azure AD (hardening), Synchronization with on-prem AD, Azure AD Bulk create/Bulk invite (group of users defined in *.csv file),  
