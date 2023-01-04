# AZ900

### Cloud Computing?
A.  _The practice of using a network of remote servers hosted on the internet to store, manage and process data, rather a local server or personal computer._

Service delivery model over the internet (cloud). This includes but is not limited to

* **compute power** meaning servers such as windows, linux, hosting environments, etc.
* **storage** like files and/or databases
* **networking** in azure but also outside when connecting to your company network
* **analytics** services for visualization and telemetry data


**Benefits of Cloud Computing**
1. Cost effective
2. Global
3. Secure
4. Reliable
5. Scalable
6. Elastic
7. Current

- **scalability** is the ability to scale, so allocate and deallocate resources at any time
- **elasticity** is the ability to scale dynamically
- **agility** is the ability to react fast (scale quickly)
- **fault tolerance** is the ability to maintain system uptime while physical and service component failures happen
- **disaster recovery** is the process and design principle which allows a system to recovers from natural or human induced disasters
- **high availability** is the agreed level of operational uptime for the system. It is a simple calculation of system uptime versus whole lifetime of the system.
 **availability = uptime/(uptime + downtime)**
<hr>

**Economies of Scale**<br>
The principle of economies of scale states that as the companies grow they become more effective at managing shared operations. Be that HR and hiring, taxes, accounting, internal operations, marketing, big purchases via contracts meaning better discounts, etc. etc.

Because of those, companies can save/earn more which in return allows for reduction in cost of their services to their customers. This is so called ‘price per unit’.

It’s not possible to go to 0 because in the end some underlying infrastructure needs to run to provide the services. But the larger the scale the more benefits can be passed to customers.

In fact, in the current scale, Microsoft can already offer multiple services for free due to how small a fraction of the cost it is for them.

<hr>

**CapEx vs OpEx**
Differences between Capital Expenditure and Operational Expenditure

|                  |   Capital Expenditure      |    Operational Expenditure     |
| ---------------- | -------------------------- | ------------------------------ |
| Up front cost    |        Significant         |             None               |
| Ongoing cost     |            Low             |           Based on usage       |
| Tax Deduction	   |         Over time	        |            Same year           |
|Early Termination |	          No	        |             Anytime            |
|Maintenance	   |          Significant	|               Low              |
|Value over time   |            Lowers	        |             No change          |

<hr>

### What is a consumption-based model?
The consumption-based model is a pricing model used in the cloud so that customers are only charged based on their resource usage.

This model is characterized by-

* **No associated upfront cost**
* **No wasted resources as such no charges are incurred for unused resources**. Unused in this case is different per service. For instance, blob storage that stores any data is considered to be used, as it consumes the storage space. Virtual Machines that are running consume CPU, memory and other resources even if there isn’t any traffic. Hence they are considered to be used and will incur charges.
* **Pay for what you need**
* **Stop paying when you don’t**

Consumption is the virtual metric used to calculate how much each resource (service) in Azure was used. Each service has many smaller metrics that track its consumption to offer best possible pricing model. Those metrics are tracked on very granular level.

<hr>

**Service Models responsibilities**
As a service means which party will manage the particular layer and all the layers below.

* **Software layer** consists the application (application code and set) & the application data
* **Platform layer** means all the supporting software and the operating system required to host the application
* **Infrastructure layer** consists hardware the infrastructure and virtualization required to host the platform

|      Layer	   |     Layer     |
| ---------------- | ------------- |
|    Application   |    Software   |
|       Data	   |    Software   |
|     Runtime	   |    Platform   |
|    Middleware    |    Platform   |
| Operating System |	Platform   |
|  Virtualization  | Infrastructure|
|     Servers	   | Infrastructure|
|    Networking	   | Infrastructure|
|     Storage	   | Infrastructure|
|  Responsibility  |     Matrix    |

As such following table represents responsibilities-

|     Layer	   | On-Premises  |     IaaS	   |     PaaS       |	  SaaS       |
| ---------------- | ------------ | -------------- | -------------- | -------------- |
| Application	   |     You	  |      You	   |      You	    | Cloud provider |
|     Data	   |     You	  |      You	   |      You	    | Cloud provider |
|    Runtime	   |     You	  |      You	   | Cloud provider | Cloud provider |
| Middleware	   |     You	  |      You	   | Cloud provider | Cloud provider |
| Operating System |     You	  |      You	   | Cloud provider | Cloud provider |
| Virtualization   |     You	  | Cloud provider | Cloud provider | Cloud provider |
|     Servers	   |     You	  | Cloud provider | Cloud provider | Cloud provider |
|   Networking	   |     You	  | Cloud provider | Cloud provider | Cloud provider |
|    Storage	   |     You	  | Cloud provider | Cloud provider | Cloud provider |

<hr>

**Cloud Deployment Model**
Cloud Deployment Model is simple a separation which describes where are the company resources deployed. Whenever this is in public cloud provider environment or private datacenter.

Below table presents high level deployment model separation

|   Layer	 |     Cloud Provider	|  Own Datacenter |
| -------------- | -------------------- | ----------------|
|    Public	 |         ✅	      |        ✖        |
|    Hybrid	 |        ✅	      |        ✅       |
|    Private	 |         ✖	       |        ✅       |

**Public Cloud**
|      Cloud Provider   |      Own Datacenter     |
| --------------------- | ----------------------- |
|         ✅	       |            ✖           |

_Key Characteristics_

* Everything runs on cloud provider hardware
* No local hardware
* Some services share hardware with other customers

_Advantages_

* No CapEx (No initial investment)
* High Availability
* Agility
* Pay as you Go (PAYG) pricing
* No hardware maintenance
* No deep technical skills required

_Disadvantages_

* Not all security and compliance policies can be met
* No ownership over the physical infrastructure
* Rare specific scenarios can’t be done

**Private Cloud**
|      Cloud Provider      |     Own Datacenter     |
| ------------------------ | ---------------------- |
|           ✖              |    	✅         |

_Key Characteristics_

* Everything runs on your own datacenter
* Self-service should be provided
* You maintain the hardware

_Advantages_

* Can support any scenario
* Total control over security and infrastructure
* Can meet any security and compliance policy

_Disadvantages_

* Initial investment is required (CapEx)
* Limited agility constrained by server capacity and team skills
* Very dependent on IT skills & expertise

**Hybrid Cloud**
|      Cloud Provider	|       Own Datacenter     |
| --------------------- | ------------------------ |
|          ✅           |        ✅               |

_Key Characteristics_

* Combines both Public & Private cloud

_Advantages_

* Great flexibility
* You can run any legacy apps in private cloud
* Can utilize existing infrastructure
* Meet any security& compliance requirements
* Can take advantage of all public cloud benefits

_Disadvantages_

* Can be more expensive
* Complicated to manage due to larger landscape
* Most dependent on IT skills & expertise from all three models

<hr>
### Types of Cloud Computing
1. SaaS - A product that is run and managed by service provider.  _Don't worry about how the service is maintained. It just works and remains available._
        Example - Salesforce, Gmail, Office 365. ~For Customers
2. PaaS - Focus on the deployment and management of your apps. _Don't worry about provisioning, configuring and understanding the Hardware or OS._
          Example - Beanstalk, AWS Heroku, Google App Engine. ~For Developers
3. IaaS - Provides access to networking features, computers and data storage space.  _Don't worry about IT staff, data centres and hardware._
          Example - Microsoft Azure, AWS, Oracle Cloud. ~For Administrators
          
<hr>

### Types of Cloud Computing Services
A.

<img src="https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg" alt="Visual representation">

**You’ll always be responsible for:**
<ul>
<li>The information and data stored in the cloud</li>
<li>Devices that are allowed to connect to your cloud (cell phones, computers, and so on)</li>
<li>The accounts and identities of the people, services, and devices within your organization</li>
</ul>

**The cloud provider is always responsible for:**
<ul>
<li>The physical datacenter</li>
<li>The physical network</li>
<li>The physical hosts</li>
</ul>

**Your service model will determine responsibility for things like:**
<ul>
<li>Operating systems</li>
<li>Network controls</li>
<li>Applications</li>
<li>Identity and infrastructure</li>
</ul>

<hr>

### Azure's Deployment Models
The cloud models define the deployment type of cloud resources. The three main cloud models are: private, public, and hybrid.

#### Private Cloud: 
Everything built on company's datacenters. Also known as On-Premise. The cloud could be OpenStack.
  1. Used by a single entity
  2. Much greater control for the company and its IT departmen
  3. Greater cost and fewer of the benefits of a public cloud deployment
  4. May be hosted from your on site datacenter or  be hosted in a dedicated datacenter offsite,
               potentially even by a third party that has dedicated that datacenter to your company

#### Public Cloud: 
Everything is built on the cloud provider. Also known as Cloud-Native. 
  1. Built, controlled, and maintained by a third-party cloud provider
  2. Anyone that wants to purchase cloud services can access and use resources
              
#### Hybrid Cloud: 
Using both On-Premise and a Cloud Service Provider. 
  1. Uses both public and private clouds in an inter-connected environment
  2. Can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources
  3. Hybrid cloud can be used to provide an extra layer of security.
        For example, users can flexibly choose which services to keep in public cloud and which to deploy to their private 
              cloud infrastructure
             
#### Cross-Cloud / Multi-cloud
Azure Arc is a set of technologies that helps manage your cloud environment as it extends the user's control plane.

<hr>

### Azure VMware Solution
A. What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.

<hr>

### Total Cost of Ownership


### Consumption based model
This consumption-based model has many benefits, including:

* No upfront costs.
* No need to purchase and manage costly infrastructure that users might not use to its fullest potential.
* The ability to pay for more resources when they're needed.
* The ability to stop paying for resources that are no longer needed.

### Compare cloud pricing models
Cloud computing is the delivery of computing services over the internet by using a pay-as-you-go pricing model. You typically pay only for the cloud services you use, which helps you:
* Plan and manage your operating costs.
* Run your infrastructure more efficiently.
* Scale as your business needs change.

To put it another way, cloud computing is a way to rent compute power and storage from someone else’s datacenter. You can treat cloud resources like you would resources in your own datacenter. However, unlike in your own datacenter, when you're done using cloud resources, you give them back. You’re billed only for what you use.

Instead of maintaining CPUs and storage in your datacenter, you rent them for the time that you need them. The cloud provider takes care of maintaining the underlying infrastructure for you. The cloud enables you to quickly solve your toughest business challenges and bring cutting-edge solutions to your users.

<hr>

### Cloud Architecture Terminologies
* Availability - Your ability to ensure service remains available **Highly Available (HA)**
* Scalability - Your ability to grow rapidly or unimpeded
* Elasticity - Your ability to shrinnk and grow to meet the demand
* Fault Tolerance - Your ability to prevent a failure
* Disaster Recovery - Your ability to recover from a failure **Highly Durable (HD)**
* Agility

#### High Availability -
Multiple Datacenters and multiple servers<br>
 **Azure Load Balancer**<br>
  A load balancer would evenly distribute traffic to multiple servers in one or more datacenters and if a datacenter or server becomes unavailable (unhealthy), it will route to only available datacenters with servers to ensure availability.

#### High Scalability -
1. Vertical Scaling - (Scaling Up) Upgrade to a bigger server.
2. Horizontal Scaling - (Scaling Out) Add more servers of the same size.

#### High Elasticity -
Automatically adding or removing servers to increase or decrease capacity based on the current demand of traffic, memory and computing power.<br>
_Horizontal Scaling_ <br>
- Scaling Out- Add more servers of the same size<br>
-  Scaling In- Remove more servers of the same size<br>
 **Azure VM Scale Sets**<br>
Automatically increase or decrease in response to demand or a defined schedule.
**SQL Server Stretch Database**<br>

#### High Durability -
<hr>

### Evolution of Computing
*Dedicated* =><br>
              **_Cons_**<br>
              Wholly utilized by a single customer<br>
              **_Pros_**<br>
              Guarantee of security, privacy and full utility of underlying resources<br>
              
*VMs* => mutliple virtual machines on one machine through - Hypervisor<br>
         **_Cons_**<br>
         Multiple apps on a single virtual machine can result in conflicts in resource sharing.<br>
         
*Containers* =>  Virtual machines running on multiple containers using Docker Daemon<br>
                 **_Pros_**<br>
                 Maximum utilization of the available capacity so cost-effective<br>
                 Containers are more efficient than multiple VMs, as they share the same underlying OS<br>
                 Multiple apps can run side by side and will not cause conflicts in resource sharing<br>
              
*Functions* => A managed VM running managed containers, known as Serverless Compute<br>
               **_Pros_**<br>
               Ver cost-effective<br>
               **_Cons_**<br>
               Cold Starts are a side-effect of this setup<br>
           
<hr>

### Global Infrastructure - Regions and Geographies
A **region** is a grouping of multiple datacenters. (Availability zones)<br>
=> Azure has 58 regions available across 140 countries<br>

A **Geography** is discreet market of two or more regions that preserves **data residency** and **compliance boundaries** .<br>

**Paired Regions** => Each region is paired with another region 300 miles away.<br>

Only one region is updated at a time to ensure no outages.<br>

Some Azure services rely on Paired Regions for Disaster Recovery.<br>
**E.g. Azure Geo-redundant Storage (GRS)**

#### Region Types and Service Availability
1. Recommended Regions
2. Alternate (other) regions<br>

*General availability (GA)* is when a service is considered ready to be used publicly by everyone.<br>
Azure cloud services are grouped into three categories-
* Foundational - When GA immediately or in 12 months in Recommended or Alternate regions.
* Mainstream - When GA immediately or in 12 months in Recommended regions. May become available in Alternate region based on customer demand.
* Specialized - Available in Recommeded or Alternate region based on customer demand.

#### Special Regions
Azure has specialized regions to meet compliance or legal regions.

#### Availability Zones
An Availability Zone is physical location made up of one or more datacenter.
* A region will generally contain 3 availability zones.

#### AZ Supported Regions

#### Availability Sets Fault and Update Domains
An Availability Zone (AZ) in an Azure region is a combination of a fault domain and an update domain.<br>
**Fault Domain** - A logical grouping of hardware to avoid a single point of failure within an AZ. Group of virtual machines that share a common power source and network switch.<br>
**Update Domain** - Azure may need to apply updates to the underlying hardware and software. Update domains ensure your resources do not go offline.<br>
**Availability Set** - A logical grouping that you can use in Azure to ensure that the VMs you place in the Availability Set are different fault/update domains to avoid downtime.<br>

<hr>

### Computing Services
* Azure Virtual Machines (VMs)
* Azure Container Instances - _Docker as a Service_
* Azure Kubernetes Services (AKS) - _Kubernetes as a Service_
* Azure Service Fabric - _Tier-1 Enterprise Containers as a Service_
* Azure Functions 
* Azure Batch

<hr>

### Storage Services
* Azure Blob Storage - _Object Serverless Storage_
* Azure Disk Storage
* Azure File Storage
* *Azure Queue Storage _Messaging Queue_
* *Azure Table Storage _Wide-Column No-SQL Database_
* Azure Data box/ Azure Databox Heavy
* Azure Archive Storage
* Azure Data Lake Storage

<hr>

### Database Services
* Azure Cosmos DB - _No SQL Databases_
* Azure SQL Database - _Fully Managed MS SQL Databases_
* Azure Database for MySQL/PQL/MariaDB - _MySQL/PostgreSQL/Maria DB Database_
* SQL Server on VMs
* Azure Synapse Analytics (Azure SQL Data Warehouse) - _Data Warehouse_
* Azure Database Migration Service
* Azure Cache for Redis - _Caches
* *Azure Table Storage - _Wide Column NoSQL Database_

<hr>

### Application Integration
* Azure Notifications Hub - _Pub/Sub_
* Azure API Apps - _API Gateway_
* Azure Service Bus - _Service Bus_
* Azure Stream Analytics - _Real-time analytics_
* Azure logic Apps
* Azure API Management
* *Azure Queue Storage _Messaging Queue_

<hr>

### Developer and Mobile Tools
* Azure SignalR Service - _Real-time Messaging_
* Azure App Service - Heroku like version for Azure
* Visual Studio (Microsoft-owned) - _Code Editor_
* Xamarin (Microsoft-owned) - _Mobile App Framework_

<hr>

### Azure DevOps Service
* Azure Boards - _Kanban_
* Azure Pipelines - _CI/CD_
* Azure Repos - _Git repos_
* Azure Test Plans - _manual and exploratory testing tools_
* Azure Artifacts 
* Azure DevTest Labs

<hr>

### Azure Resource Manager
* What is Infrastructure as Code (IaC)?<br>
     Process of managing and provisioning computer data centers through machine readable definition files<br>
     
#### Azure Resource Manager (ARM) allows you to programmatically create Azure resource via JSON template.

<hr>

### Azure QuickStart Templates
It is a library of pre-made Azure templates provided by the community and partners to help you quickly launch new projects for a variety of stack scenarios.

<hr>

### vNets and Subnets
**Virtual Network (vNet)** is a logically isolated section of the Azure network where you launch youre Azure resources. _You choose a range of IPs using CIDR range._<br>
**Subnets** is a logically partition of an IP network into multiple smaller network segments. _You are breaking up your IP range for vNet into smaller networks._<br>

* A Public Subnet is one that can reach the internet<br>
* A Private Subnet is one that can not reach the internet<br>

<hr>

### Cloud-Native Networking Services
* Azure DNS
* Azure Virtual Network (vNet)
* Azure Load Balancer
* Azure Application Gateway
* Network Security Groups

<hr>

### Enterprise/Hybrid Networking Services
* Azure Front Door
* Azure Express Route
* Virtual WAN
* Azure Connection
* Virtual Network Gateway

<hr>

### Azure Traffic Manager - operates at the DNS layer to quickly and efficiently direct incoming DNS requests based on the routing method of your choice.

<hr>

### Azure DNS - allows you to host your domain names on Azure. You can create your DNS zones and manage your DNS records.
** Azure DNS does not allow you to purchase domains. Only the ability to manage DNS records.

<hr>

### Azure Load Balancer - is used for evenly distributing incoming network traffic across a group of backend resources or servers.<br>
* Azure Load Balancer operates on OSI Layer 4 (Transport)<br>
* You can create a : <br>
  1) Public Load Balancer incoming traffic from the internet to public-facing servers (Public IPs)<br>
  2) Internal (Private Load Balancer) incoming internal network traffic to private-facing servers (Private IPs)<br>
                  
<hr>

### Scale Sets
** Allows you to group identical virtual machines (VMs) and automatically increase or decrease amount of servers based on :
* change in CPU, memory, disk and network performance
* On a predefined schedule

<hr>

### IoT Services
* IoT Central
* IoT Hub
* IoT Edge
* Windows 10 IOT Core Services

<hr>

### Big Data and Analytics Services
* Azure Synapse Analytics - _Data Warehousing and Big Data analytics_ **run SQL queries**
* HDInsight - _open-souce analytics software such as Hadoop, Kafka and Spark_
* Azure Databricks
* Data Lake Analytics

<hr>

### AI/ML Services Introduction
* Azure Mchine Learning Service
* Azure Mchine Learning Studio (classic)
* Personalizer
* Translator
* Anomaly Detector
* Azure Bot Service
* Form Recogniser
* Computer Vision
* Language Understanding
* QnA Maker
* Text Analytics
* Content Moderator
* Face
* Ink Recogniser

<hr>

### Serverless Services
* Azure Functions
* Blog Storage
* Logic Apps
* Event Grid

<hr>

### Azure Portal
Web-based unified console

### Azure Preview Portal - Preview, Beta,Other pre-release
_test preview features_

<hr>

### Azure Powershell
** command -line shell and a scripting language

<hr>

### Visual Studio Code
free source-code editor

<hr>

### Azure Cloud Shell
browser-accessible shell _either Bash or PowerShell_

<hr>

### Azure CLI
** Command Line Interface (CLI) processes commands to a computer program in the form of lines of text.

 <hr>
 ### Follow Along
 
 #### Create a Resource Group
** Azure Portal => Resource Group => Click on Add => Select subscription, name and region => Click on Review + Create/ Create

#### Create a vNet

** Azure Portal => Virtual Network (vNet) => Click on Add => Select subscription, resource group, virtual network name and region => Other options like IP Addresses, Security and Tags can be explored => Click on Review + Create/ Create

#### Launching a Server

** Azure Portal => Virtual Machine (VM) => Click on Add => Select subscription, resource group, virtual machine name, region, availability options, Image, size, authentication options, public inbound ports- none  => Other options like Disks, Networking, Management and Advanced can be explored => Click on Review + Create/ Create

#### Creating Azure Function

** Azure Portal => Function App => Click on Add => Select subscription, resource group, Function app name, publish, runtime stack, version, region => Other options like Hosting, Monitoring and Tags can be explored => Click on Review + Create/ Create => After deployment, click functions on left side of dashboard => Create Function => Code + Test

#### Storing files in Blob Storage

** Azure Portal => Storage accounts => Click on Add => Selection subscription, resource group, storage account name, location, performance, account kind, replication and access tier => Other options like Networking, Advanced and Tags can be explored => Click on Review + Create/ Create => Go to containers => Click on container => Add name and public access level => Now we can access the container and upload files

#### Exploring Azure Cloud Shell

** Azure Portal => Click on Cloud Shell => Select Bash or Powershell => Create Storage method => Cloud shell commands can be used

#### Azure Trust Center

** A public facing website portal providing easy access to privacy, security and regulatory compliance information.

#### Azure Security - Compliance Programs
* NIST 800 - 53
* PIPEDA Compliant
* HIPPA Compliant
* FIPS-140-2 Compliant

1) Criminal Iustice Information Services (CJIS)
2) Cloud Security Alliance (CSA) STAR Certification
3) General Data Protection Regulation (GDPR)
4) EU Model Clauses
5) Health Insurance Portability and Accountability Act (HIPAA)
6) International Organization for Standardization (ISO) and the International Electrotechnical Commission (IEC) 27018
7) Multi-Tier Cloud Security (MTCS) Singapore
8) Service Organization Controls (SOC) 1,2, and 3
9) National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF)
10) UK Government G-Cloud
11) Federal Information Processing Standard (FIPS) 140-2

<hr>

### Azure Active Directory<br>
Azure Active Directory (Azure AD) is Microsoft's cloud-based identity and access management service, which helps your employees sign in and access resources.<br>
**External Resources**<br>
-Microsoft Office 365<br>
-Azure Portal<br>
-SaaS applications<br>
**Internal Resources**<br>
-Applications within your internal networking<br>
-Access to workstations on-premise<br>

Use Azure AD to implement **Single-Sign-On (SSO)**<br>

**_Azure Active Directory comes in four editions_:**<br>
1. **Free** MFA, SSO, Basic Security and Usage Reports, User Management
2. **Office 365 Apps** Company Branding, SLA, Two-Sync between On-Premise and Cloud
3. **Premium 1** Hybrid Architecture, Advanced Group Access, Conditinal Access
4. **Premium 2** Identity Protection, Identity Governance
 
<hr>

### Multi-Factor Authentication

<hr>

### Azure Security Center
unified infrastucture security management system

<hr>

### Key Vault
safeguard cryptographic keys and other secrets
* Secrets Management
* Key Management
* Certificate Management
* Hardware Security Module *Multi-tenant (FIPS 140-2 Compliant)
                           *Single-tenant (FIPS 140-3 Compliant)
                           
<hr>

### Azure DDoS Protection (DDoS = Distributed Denial of Service)
Two tiers of DDoS Protection
1. DDoS Protection Basic
* Free
* Already turned on project Azure's global network
2. DDoS Protection Standard
* Starting at $2,994/month
* Metrics, Alerts, Reporting
* DDoS Expert Support
* Application and Cost Protection SLAs

<hr>

### Azure Firewall
cloud-based network security-service
**Features**
1. Across subscriptions
2. Static public IP address
3. No additional load balancers are required
4. Span multiple AZs for increased availability
5. No additional cost for a firewall deployed in a Availability Zone
6. Additional costs for inbound and outbound data transfers

<hr>

### Azure Information Protection (AIP)
Protects sensitive information

<hr>

### Application Gateway
web traffic load balancer (Layer 7 HTTP)

<hr>

### Advanced Threat Protection (ATP)
_leverages your on-premise Active Directory_
* identify, detect and investigate advanced threats, compromised identities and malicious insider actions

<hr>

### Microsoft Security Development Lifecycle (SDL)
* industry-leading software security assurance process

<hr>

### Azure Policies
A service you can create, assign and manage policies. A policy allows you to enforce or control the properties of a resource
*JSON format known as **Policy Definitions**

<hr>

### Role-Based Access Control (RBAC)<br>
Helps you manage who has access to Azure Resources
* User - An individual who has a profile in Azure AD
* Group -  A set of users created in Azure AD
* Service Principal - A security identity used by applications or services to access specific Azure resources.
* Managed Identity - An identity in Azure AD that is automatically managed by Azure
* Scope - set of resources
* Role Definition - collection of permissions to read, grant, create, update, delete

<hr>

### Lock resources
lock a subscription, resource group or resource
* CanNotDelete
* ReadOnly

<hr>

### Azure Management Groups

<hr>

### Azure Monitor
For collecting, analyzing and acting on telemetry

<hr>

### Service Health
current and upcoming issues
1. Azure Status
2. Azure service health
3. Azure resource health

<hr>

### Azure Advisor
personalised cloud consultant
1.High Availability
2. Security
3. Performance
4. Cost
5. Operational Excellence

<hr>

### Service Level Agreements (SLAs)
uptime and connectivity
_Performance Targets => %_
(Azure does not provide SLAs for free tier or the shared tiers)

<hr>

### Service Credits
have discount applied to their Azure bill, as compensation for an underperforming Azure product or service.

<hr>

### Composite SLAs
combine SLAs<br>
**Fallback systems**

<hr>

### Total Cost of Ownership (TCO) Calculator
Estimate the cost savings

<hr>

### Azure Marketplace
apps and services made available by third party publishers

<hr>

### Azure Support Plans

<hr>

### Azure Licensing
**Windows Server licenses** - _repurpose this investment_
* Azure Hybrid Use Benefit (HUB) - Bring Your Own License (BYOL)

<hr>

### Azure Subscriptions
4 tiers
1. Free
2. Pay-As-You-Go(PAYG)
3. Enterprise Agreement
4. Student Subscription

<hr>

### Pricing Calculator

<hr>

### Azure Cost Management
_cost analysis_ , create budgets

