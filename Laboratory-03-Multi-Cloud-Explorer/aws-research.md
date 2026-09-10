# AWS Research

## Brief Overview
Amazon Web Services (AWS) is the cloud platform run by Amazon. It started in 2006 with three services — Amazon S3, Amazon SQS, and Amazon EC2 — and has since grown into the largest and most widely used public cloud provider, with hundreds of services covering compute, storage, databases, networking, AI/ML, and more. AWS is generally seen as the "market leader" because it has been around the longest and has the widest range of services.

## Global Infrastructure
AWS organizes its physical infrastructure into **Regions** and **Availability Zones (AZs)**:
- A **Region** is a separate geographic area (for example, `us-east-1` in Northern Virginia or `ap-southeast-1` in Singapore).
- Each Region has multiple **Availability Zones**, which are one or more discrete data centers with their own power, cooling, and networking. Most Regions have at least 3 AZs.
- AWS also has **Local Zones** and **Wavelength Zones**, which place compute and storage closer to end users or to 5G networks for very low latency use cases.

Spreading resources across AZs (instead of putting everything in one data center) is how AWS customers build highly available, fault-tolerant applications.

## Cloud Management Console
AWS is managed through the **AWS Management Console**, a web-based dashboard where you can create and monitor resources visually. For automation or scripting, AWS also provides the **AWS CLI** (command-line interface) and **SDKs** for languages like Python, Java, and JavaScript.

## Four Core Services
1. **Amazon EC2 (Elastic Compute Cloud)** – Virtual servers ("instances") that you can resize and scale on demand. This is AWS's main compute service.
2. **Amazon S3 (Simple Storage Service)** – Object storage for files, backups, images, and static websites. It is one of AWS's oldest and most-used services.
3. **Amazon VPC (Virtual Private Cloud)** – Lets you create your own isolated network inside AWS, with subnets, route tables, and firewalls (security groups).
4. **AWS IAM (Identity and Access Management)** – Controls who (or what) can access your AWS resources, and what they're allowed to do.

## Three Advantages
1. **Widest range of services** – AWS has the largest service catalog of any provider, so almost any workload has a matching service.
2. **Mature global infrastructure** – Because AWS has been operating the longest, it has the most Regions and Availability Zones, which helps with performance and disaster recovery.
3. **Strong ecosystem and community** – Because so many companies use AWS, there's a huge amount of documentation, tutorials, third-party tools, and hiring pool of AWS-skilled engineers.

## Typical Enterprise Use Cases
- Hosting large-scale web and mobile applications that need to scale automatically.
- Running big data analytics and data lakes (using services like S3 and Amazon Redshift).
- Disaster recovery and backup, since resources can be replicated across Regions.
- Machine learning workloads using services like Amazon SageMaker.

## Screenshot
See `screenshots/aws-homepage.png` for a screenshot of the official AWS homepage/console.

## References
- AWS Regions and Availability Zones – https://docs.aws.amazon.com/global-infrastructure/latest/regions/aws-regions-availability-zones.html
- AWS Global Infrastructure – https://aws.amazon.com/about-aws/global-infrastructure/
- About AWS – https://aws.amazon.com/about-aws/
