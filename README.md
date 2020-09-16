# AzureFundamental
This file describes the basic understanding info relating to azure architecture
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


## References:
- Microsoft Learning Docs: https://docs.microsoft.com/en-us/learn