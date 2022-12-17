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

