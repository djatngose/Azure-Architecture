# Azure Fundamental
This file describes the basic understanding info relating to azure architecture
## Cloud concepts
- Compute power - such as Linux servers or web applications used for computation and processing tasks
- Storage - such as files and databases
- Networking - such as secure connections between the cloud provider and your company
- Analytics - such as visualizing telemetry and performance data
### 1. Container (Docker)
- Containers provide a consistent, isolated execution environment for applications.
- They're similar to VMs except they don't require a guest operating system
- Instead, the application and all its dependencies is packaged into a "container" and then a standard runtime environment is used to execute the app
- This allows the container to start up in just a few seconds, because there's no OS to boot and initialize.You only need the app to launch
- Multiple containers can be run on a single machine, and containers can be moved between machines
### 2. Serverless computing
- Serverless computing lets you run application code without creating, configuring, or maintaining a server
- The core idea is that your application is broken into separate functions that run when triggered by some action
- This is ideal for automated tasks - for example, you can build a serverless process that automatically sends an email confirmation after a customer makes an online purchase.
- The serverless model differs from VMs and containers in that you only pay for the processing time used by each function as it executes
- VMs and containers are charged while they're running - even if the applications on them are idle
- This architecture doesn't work for every app - but when the app logic can be separated to independent units
- You can test them separately, update them separately, and launch them in microseconds, making this approach the fastest option for deployment.

## Azure Billing
https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/4-multiple-subscriptions
### 1. Azure subscription
- An Azure subscription is a logical container used to provision resources in Azure
- It holds the details of all your resources like virtual machines (VMs), databases,app services and more
- You might choose to create additional subscriptions to separate
  - **Environments**: When managing your resources, you can choose to create subscriptions to set up separate environments for **development and testing, security, or to isolate data** for compliance reasons. This is particularly useful because resource access control occurs at the subscription level.
  - **Organizational structures**: You can create subscriptions to reflect different organizational structures. For example, you could limit a team to lower-cost resources, while allowing the IT department a full range. This design allows you to manage and control access to the resources that users provision within each subscription.
  - **Billing**: You might want to also create additional subscriptions for billing purposes. Because costs are first aggregated at the subscription level, you might want to create subscriptions to manage and track costs based on your needs. For instance, you might want to create a subscription for your production workloads and another subscription for your development and testing workloads.
- You might also need additional subscriptions due to:
  - ****Subscription limits**:
    - Subscriptions are bound to some hard limitations.
    - For example, the maximum number of **Express Route** circuits per subscription is **10**.
    - Those limits should be considered as you create subscriptions on your account.
    - If there is a need to go over those limits in particular scenarios, then you might need additional subscriptions.
### 2. Express Route
  - ExpressRoute is an Azure service that lets you create **private** connections between Microsoft **datacenters** and **infrastructure** that's on your premises or in a colocation facility
  - They offer higher security, reliability, and speeds, with lower and consistent latencies than typical connections over the Internet.
  - In some cases, using ExpressRoute connections to transfer data between on-premises devices and Azure can yield significant cost benefits.

## Cloud Security
https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/2-shared-responsibility

## Services on Azure:
  - `Compute services` such as VMs and containers that can run your applications
  - `Database services` that provide both relational and NoSQL choices
  - `Identity` services that help you authenticate and protect your users
  - `Networking` services that connect your datacenter to the cloud, provide high availability or host your DNS domain
  - `Storage` solutions that can accommodate massive amounts of both structured and unstructured data
  - `AI and machine-learning services` can analyze data, text, images, comprehend speech, and make predictions using data — changing the world of agriculture, healthcare, and much more.

## References:
- Microsoft Learning Docs: https://docs.microsoft.com/en-us/learn