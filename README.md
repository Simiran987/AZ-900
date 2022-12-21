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

### Types of Cloud Computing
1. SaaS - A product that is run and managed by service provider.  _Don't worry about how the service is maintained. It just works and remains available._
        Example - Salesforce, Gmail, Office 365. ~For Customers~
2. PaaS - Focus on the deployment and management of your apps. _Don't worry about provisioning, configuring and understanding the Hardware or OS._
          Example - Beanstalk, AWS Heroku, Google App Engine. ~For Developers~
3. IaaS - Provides access to networking features, computers and data storage space.  _Don't worry about IT staff, data centres and hardware._
          Example - Microsoft Azure, AWS, Oracle Cloud. ~For Administrators~

### Types of Cloud Computing Services
A.

<img src="https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg" alt="Visual representation">

**You’ll always be responsible for:**

The information and data stored in the cloud
Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
The accounts and identities of the people, services, and devices within your organization
The cloud provider is always responsible for:

The physical datacenter
The physical network
The physical hosts

**Your service model will determine responsibility for things like:**

Operating systems
Network controls
Applications
Identity and infrastructure

### Azure's Deployment Models
The cloud models define the deployment type of cloud resources. The three main cloud models are: private, public, and hybrid.

#### Private Cloud: 
               1) used by a single entity
               2) much greater control for the company and its IT departmen
               3) greater cost and fewer of the benefits of a public cloud deployment
               4) may be hosted from your on site datacenter or  be hosted in a dedicated datacenter offsite,
               potentially even by a third party that has dedicated that datacenter to your company

#### Public Cloud: 
              1) Built, controlled, and maintained by a third-party cloud provider
              2) anyone that wants to purchase cloud services can access and use resources
              
#### Hybrid Cloud: 
              1) uses both public and private clouds in an inter-connected environment
              2) can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources
              3) Hybrid cloud can be used to provide an extra layer of security.
              For example, users can flexibly choose which services to keep in public cloud and which to deploy to their private 
              cloud infrastructure
             
#### Multi-cloud

### What is Azure Arc ?
A. Azure Arc is a set of technologies that helps manage your cloud environment. 

### Azure VMware Solution
A. What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.

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
