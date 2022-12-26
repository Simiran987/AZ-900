# AZ900

## Microsoft Azure Fundamentals: Describe cloud concepts

### Cloud Computing?
A.  _The practice of using a network of remote servers hosted on the internet to store, manage and process data, rather a local server or personal computer._

Cloud computing is the delivery of computing services over the internet. Computing services include common IT infrastructure such as virtual machines, storage, databases, and networking.Cloud services also expand the traditional IT offerings to include things like Internet of Things (IoT), machine learning (ML), and artificial intelligence (AI).
            Mainly, every cloud provider provides a) Compute Power and b) Storage

**i. Dedicated Server, ii.Virtual Private Server, iii.Shared Hosting, iv. Cloud Hosting**

**Benefits of Cloud Computing**
1. Cost effective
2. Global
3. Secure
4. Reliable
5. Scalable
6. Elastic
7. Current

<hr>

### Types of Cloud Computing
1. SaaS - A product that is run and managed by service provider.  _Don't worry about how the service is maintained. It just works and remains available._
        Example - Salesforce, Gmail, Office 365. ~For Customers
2. PaaS - Focus on the deployment and management of your apps. _Don't worry about provisioning, configuring and understanding the Hardware or OS._
          Example - Beanstalk, AWS Heroku, Google App Engine. ~For Developers
3. IaaS - Provides access to networking features, computers and data storage space.  _Don't worry about IT staff, data centres and hardware._
          Example - Microsoft Azure, AWS, Oracle Cloud. ~For Administrators

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
**Virtual Network (vNet)** is a logically isolated section of the Azure network where you launch youre Azure resources. _You choose a range of IPs using CIDR range._
**Subnets** is a logically partition of an IP network into multiple smaller network segments. _You are breaking up your IP range for vNet into smaller networks._

* A Public Subnet is one that can reach the internet
* A Private Subnet is one that can not reach the internet

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

### Azure Load Balancer - is used for evenly distributing incoming network traffic across a group of backend resources or servers.
* Azure Load Balancer operates on OSI Layer 4 (Transport)
* You can create a : 1) Public Load Balancer incoming traffic from the internet to public-facing servers (Public IPs)
                     2) Internal (Private Load Balancer) incoming internal network traffic to private-facing servers (Private IPs)
                  
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
 
 #### Create a Resource Group
** Azure Portal => Resource Group => Click on Add => Selection subscription, name and region => Click on Review + Create/ Create

<hr>

#### Create a vNet

** Azure Portal => Virtual Network (vNet) => Click on Add => Selection subscription, resource group, virtual network name and region => Other options like IP Addresses, Security and Tags can be explored => Click on Review + Create/ Create

<hr>

#### Launching a Server

** Azure Portal => Virtual Machine (VM) => Click on Add => Selection subscription, resource group, virtual machine name, region, availability options, Image, size, authentication options, public inbound ports- none  => Other options like Disks, Networking, Management and Advanced can be explored => Click on Review + Create/ Create

<hr>
