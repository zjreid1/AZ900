# AZ900
AZ900 Notes 


https://learn.microsoft.com/en-us/training/paths/microsoft-azure-fundamentals-describe-cloud-concepts/


### Describe Cloud Concepts

AZ-900 Domain Area	Weight
Describe cloud concepts	25-30%
Describe Azure architecture and services	35-40%
Describe Azure management and governance	30-35%

### Intro to Cloud Computing

Objectives:
Define cloud computing.
Describe the shared responsibility model.
Define cloud models, including public, private, and hybrid.
Identify appropriate use cases for each cloud model.
Describe the consumption-based model.
Compare cloud pricing models.


- Cloud computing is the delivery of computing services over the internet including VMs, storage, DBs, and networking which allows for rapid horizontal scaling (adding more servers to handle workload)
- W/ the shared responsibility model the responsibiltieis of who is responsible for what get split between provider and consumer (i.e. provider is responsible for data center, consumer is responsible for data/info in the cloud, and access security)

<img width="885" height="528" alt="image" src="https://github.com/user-attachments/assets/e2741136-2e8b-430a-8026-b1a3622b8949" />


When using a cloud provider, you’ll always be responsible for:

- The information and data stored in the cloud
- Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
- The accounts and identities of the people, services, and devices within your organization

The cloud provider is always responsible for:

- The physical datacenter
- The physical network
- The physical hosts

Your service model will determine responsibility for things like:

- Operating systems
- Network controls
- Applications
- Identity and infrastructure

### Cloud Models

- Private cloud: Used by a single corp/entity/  Allows for greatest control and can be hosted from corp/entitys data center(or pontially 3rd parties).  Also comes with greatest cost/fewer benfits of public cloud
- Public cloud: Built, controlled, and maintained by 3rd part cloud provider.  Anyone that wants to purchase cloud services can access/use the resources.
- Hybrid cloud:  Users can choose which services are public and which to deploy to priv cloud infra.  Can be used to allow priv cloud to surge for increased/temp demand via deploying public cloud resources
- Multi cloud: Use multiple public cloud providers (potientially using differeant features from each, or possibly migrating from one to another)

Azure Arc: Set of tech that manages cloud enviro regardless of the above scenarios



### Consumption Based Model

- CapEx vs OpEx
- CapEx: One time up front expediture to purchase a resource (i.e a building, a datacenter, or company vehicle)
- Opex: Spending money on recurring services/services over time (renting a con center, leasing a vehicle, or using cloud services)
- Cloud computing is Opex
- Benefits of cloud computing/consumption based model: No upfront costs, no need to purchase/manage infra, pay for resources as needed, stop paying for resources you don't need
- Building a priv data center = costly w/ potential overruns, cloud based model you can scale as you need
- Cloud is usually PAYGO, and someone else handles the infra


1. What is cloud computing?

Delivery of computing services over the internet.
Correct

Delivery of storage services over the internet.

Delivery of websites accessible via the internet.
2. Which cloud model uses some datacenters focused on providing cloud services to anyone that wants them, and some data centers that are focused on a single customer?

Public cloud

Hybrid cloud
Correct

Multicloud
3. According to the shared responsibility model, which cloud service type places the most responsibility on the customer?

Infrastructure as a Service (IaaS)
Correct

Software as a Service (SaaS)

Platform as a Service (PaaS)


---

Upon completion of this module, you will be able to:

Describe the benefits of high availability and scalability in the cloud.

Describe the benefits of reliability and predictability in the cloud.

Describe the benefits of security and governance in the cloud.

Describe the benefits of manageability in the cloud.

### Describe Benefits of Cloud Services

- Azure SLAs are %ages in uptime, more uptime = more $$$
- 99% uptime can be down 1.6 hours per week, but 99.9% can be down 10 mins per week max
- Highly available = uptime

- Scalability = ability to adjust resources to meet demand (elasticity to scale up/scale down as needed to avoid overpaying)
- Vertical scaling = Increase CPU/RAM available on a VM
- Horizontal scaling = add additional VMs/containers (throw more servers at the problem instead of beefing up one server)

### Benefits of relability/predictability in the cloud

- Relability is the ability to recover from failures and continue to function and is part of the Azure Well-Architected Franework.  Being decentralized the system can shift/recover as needed even to other geographic zones
- Predictability allows focus on performance and cost predictability (MS WAF)
- Performance: Focuses on providing known resources needed to deliver the end product depending on needs from scaling to HA, to load balancing, etc...
- Cost predictibility focuses on forecasting cost of cloud spend and being able to track resource utilization and cost in real time, and use tools like Total Cost Ownership or the Pricing Claculator to get an estimate of cloud spend


### Describe benefits of security/governance in the cloud

- Governance/compliance templates can help meet corp standars/regulatory requirements
- Cloud based audititing can flag resources out of compliance and mitigate impacts
- Security can include easy patches and maintenance automation or various service/software deployments

### Cloud Managability

- Cloud management allows for scaling, deploying resources based on templates, monitoring/telmetry, and automatic alerts
- Cloud management can take the form of web portal, CLI, API, or Powershell
