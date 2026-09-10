# Microsoft Azure Research

## Brief Overview
Microsoft Azure is Microsoft's cloud computing platform. It started out as "Windows Azure," first previewed to developers in October 2008 and made commercially available on February 1, 2010. It was renamed "Microsoft Azure" in 2014 as it grew beyond just Windows-based workloads. Azure is especially popular with organizations that already use Microsoft products like Windows Server, Active Directory, and Microsoft 365, because it integrates closely with them.

## Global Infrastructure
Azure's infrastructure is also built around **Regions** and **Availability Zones**:
- An **Azure Region** is a set of data centers within a defined latency perimeter, connected through a dedicated low-latency network.
- Regions are grouped into **Geographies** (e.g., United States, Europe, Asia Pacific), which matter for data residency and compliance.
- **Availability Zones** are physically separate data centers within a Region, each with independent power, cooling, and networking.
- Azure also uses **Region Pairs** — two Regions in the same geography, at least 300 miles apart, used for disaster recovery replication.
- Azure currently operates in 60+ Regions, which Microsoft states is more than any other cloud provider.

## Cloud Management Console
Azure resources are managed through the **Azure Portal**, a web-based dashboard. Azure also provides **Azure CLI**, **Azure PowerShell**, and **Azure Resource Manager (ARM) templates** for automation and infrastructure-as-code.

## Four Core Services
1. **Azure Virtual Machines** – Azure's main compute service, equivalent to AWS EC2, letting you run Windows or Linux VMs on demand.
2. **Azure Blob Storage** – Object storage for unstructured data such as files, images, and backups.
3. **Azure Virtual Network (VNet)** – Lets you build your own private network within Azure, including subnets and network security groups.
4. **Microsoft Entra ID (formerly Azure Active Directory)** – Azure's identity and access management service, used to manage users, groups, and permissions.

## Three Advantages
1. **Deep integration with Microsoft products** – Azure works smoothly with Windows Server, Active Directory, Microsoft 365, and .NET, which makes migration easier for organizations already using these tools.
2. **Largest Region footprint** – With 60+ Regions, Azure gives organizations a lot of flexibility to place resources close to their users or to meet local compliance rules.
3. **Strong hybrid cloud support** – Services like Azure Arc let companies manage on-premises servers and cloud resources from a single place, which is helpful for businesses that aren't ready to move everything to the cloud.

## Typical Enterprise Use Cases
- Migrating on-premises Windows Server and Active Directory environments to the cloud.
- Running enterprise line-of-business applications built on .NET.
- Hybrid cloud setups where some systems stay on-premises and others move to Azure.
- Business intelligence and analytics through Microsoft's ecosystem (e.g., Power BI integration).

## References
- Azure Global Infrastructure and Geographies – https://azure.microsoft.com/en-us/explore/global-infrastructure/geographies
- Azure Regions List – https://learn.microsoft.com/en-us/azure/reliability/regions-list
- What is Microsoft Azure – https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-azure
