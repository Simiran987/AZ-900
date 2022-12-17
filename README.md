# AZ900

## Microsoft Azure Fundamentals: Describe cloud concepts
### Name of temporary Azure portal environment available in the exercises?
A. Sandbox
### What is Cloud Computing?
A.Cloud computing is the delivery of computing services over the internet. Computing services include common IT infrastructure such as virtual machines, storage, databases, and networking.Cloud services also expand the traditional IT offerings to include things like Internet of Things (IoT), machine learning (ML), and artificial intelligence (AI).
            Mainly, every cloud provider provides a) Compute Power and b) Storage
### What is shared responsibility?
A. With the shared responsibility model, the responsibilities earlier only available to a traditional datacenter, now get shared between the cloud provider and the consumer. Physical security, power, cooling, and network connectivity are the responsibility of the cloud provider. The consumer isn’t collocated with the datacenter, so it wouldn’t make sense for the consumer to have any of those responsibilities.

At the same time, the consumer is responsible for the data and information stored in the cloud. (You wouldn’t want the cloud provider to be able to read your information.) The consumer is also responsible for access security, meaning you only give access to those who need it.
Then, for some things, the responsibility depends on the situation.
### Extra
cloud service types (covered later in this learning path): infrastructure as a service (IaaS), platform as a service (PaaS), and software as a service (SaaS). IaaS places the most responsibility on the consumer, with the cloud provider being responsible for the basics of physical security, power, and connectivity. On the other end of the spectrum, SaaS places most of the responsibility with the cloud provider. PaaS, being a middle ground between IaaS and SaaS, rests somewhere in the middle and evenly distributes responsibility between the cloud provider and the consumer.

<img src="https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg" alt="Visual representation">

You’ll always be responsible for:

The information and data stored in the cloud
Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
The accounts and identities of the people, services, and devices within your organization
The cloud provider is always responsible for:

The physical datacenter
The physical network
The physical hosts
Your service model will determine responsibility for things like:

Operating systems
Network controls
Applications
Identity and infrastructure

### What are cloud models?
What are cloud models? The cloud models define the deployment type of cloud resources. The three main cloud models are: private, public, and hybrid.

Private Cloud: 1) used by a single entity
               2) much greater control for the company and its IT departmen
               3) greater cost and fewer of the benefits of a public cloud deployment
               4) may be hosted from your on site datacenter or  be hosted in a dedicated datacenter offsite, potentially even by a third party that has dedicated that datacenter to your company

Public Cloud: 1) Built, controlled, and maintained by a third-party cloud provider
              2) anyone that wants to purchase cloud services can access and use resources
              
Hybrid Cloud: 1) uses both public and private clouds in an inter-connected environment
              2) can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources
              3) Hybrid cloud can be used to provide an extra layer of security. For example, users can flexibly choose which services to keep in public cloud and which to deploy to their private cloud infrastructure
             
Multi-cloud

### What is Azure Arc ?
A. Azure Arc is a set of technologies that helps manage your cloud environment. 

### Azure VMware Solution
A. What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.

