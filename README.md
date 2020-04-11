# Microsoft Azure Interview/Academic Questions

1. [Cloud Computing](#cloud_computing)
      * [Azure Models](#azure_models)
3. [Azure Services](#azure_services)
      * [General](#general)
      * [Storage Account](#storage_account)

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
|Azure Storsimple|SYnchronization between on-prem and Azure Storage|
<a name="storage_account"></a>
### Storage Account
#### Q: How many different Storage Accounts Azure offer?
A: There's 4 types of Storage Accounts:<br/>  
**1) BLOB Storage** - designed for storing images, files with distributed access, logs etc.<br/>
**2) Table Storage** - designed for storing structured NoSQL data.<br/>
**3) Queue Storage** - designerd for storing large number of messages (access via HTTPS).<br/> 
**4) (Shared) File Storage** - designed for storing fully managed file shares.<br/>
