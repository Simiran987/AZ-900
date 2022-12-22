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
*Dedicated* => *Cons*<br>
              Wholly utilized by a single customer<br>
              *Pros*<br>
              Guarantee of security, privacy and full utility of underlying resources<br>
              
*VMs* => mutliple virtual machines on one machine through - Hypervisor<br>
         *Cons*<br>
         Multiple apps on a single virtual machine can result in conflicts in resource sharing.<br>
         
*Containers* =>  Virtual machines running on multiple containers using Docker Daemon<br>
                 *Pros*<br>
                 Maximum utilization of the available capacity so cost-effective<br>
                 Containers are more efficient than multiple VMs, as they share the same underlying OS<br>
                 Multiple apps can run side by side and will not cause conflicts in resource sharing<br>
              
*Functions* => A managed VM running managed containers, known as Serverless Compute<br>
               *Pros*<br>
               Ver cost-effective<br>
               *Cons*<br>
               Cold Starts are a side-effect of this setup<br>
           
<hr>

### Global Infrastructure - Regions and Geographies
         
