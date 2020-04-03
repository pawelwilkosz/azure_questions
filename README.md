# Microsoft Azure Interview Questions

1. [Cloud Computing](#cloud_computing)
* [Azure Models](#azure_models)
3. [Azure Services](#azure_services)
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
<a name="storage_account"></a>
### Storage Account
#### Q: How many different Storage Accounts Azure offer?
A: There's 4 types of Storage Accounts:<br/>  
**1) BLOB Storage** - designed for storing images, files with distributed access, logs etc.<br/>
**2) Table Storage** - designed for storing structured NoSQL data.<br/>
**3) Queue Storage** - designerd for storing large number of messages (access via HTTPS).<br/> 
**4) (Shared) File Storage** - designed for storing fully managed file shares.<br/>
