# Client Recommendations

## Client A – Startup Company
**Scenario:** A startup company wants to launch a new mobile application. Their budget is limited, but they expect rapid growth within the next few years.

**Recommended Platform: AWS**

AWS is a good fit here because it has a generous free tier and pay-as-you-go pricing, so the startup doesn't need to invest heavily upfront. It also offers serverless options that scale automatically as the app grows, so the team won't need to redesign their infrastructure later when usage increases. Because AWS has the largest ecosystem, it's also easier to hire developers who already know the platform.

Suggested services:
- **Amazon EC2** or **AWS Lambda** – to run the backend, with Lambda being useful if they want to avoid managing servers directly.
- **Amazon S3** – to store app assets like images and user uploads.
- **Amazon RDS** – for a managed relational database as their user data grows.

## Client B – University
**Scenario:** A university already uses Windows Server, Microsoft 365, and Active Directory, and wants to migrate some services to the cloud.

**Recommended Platform: Microsoft Azure**

Azure is the clear choice here because the university's existing systems are all Microsoft products. Azure integrates directly with Active Directory through Microsoft Entra ID, which means user accounts and permissions can carry over without having to rebuild everything from scratch. This makes the migration smoother and reduces the risk of disrupting staff and student access during the move.

Suggested services:
- **Microsoft Entra ID** – to extend the university's existing Active Directory into the cloud.
- **Azure Virtual Machines** – to migrate existing Windows Server workloads.
- **Azure Virtual Desktop** or **Azure Files** – for shared storage and remote access for staff and students.

## Client C – AI Research Company
**Scenario:** A research company develops Artificial Intelligence and Machine Learning applications that require high-performance computing.

**Recommended Platform: Google Cloud Platform**

GCP is the strongest option for AI/ML-heavy workloads. Google built much of the underlying technology used in modern machine learning, and GCP's tools are designed to work well together for training and deploying models at scale. GCP also gives easy access to high-performance computing hardware needed for large training jobs.

Suggested services:
- **Vertex AI** – to build, train, and deploy machine learning models.
- **Compute Engine** with GPU/TPU support – for high-performance model training.
- **BigQuery** – to store and analyze the large datasets used for training.

## Client D – Global E-Commerce Company
**Scenario:** A multinational online shopping company serves customers around the world and requires highly available infrastructure with automatic scaling.

**Recommended Platform: AWS**

AWS is well suited for a global e-commerce platform because of its large number of Regions and Availability Zones, which allow the company to place resources closer to customers around the world and keep the site available even if one data center has an issue. AWS also has mature auto-scaling and load-balancing tools that are proven at a very large scale, which matters for handling traffic spikes like seasonal sales.

Suggested services:
- **Amazon EC2 Auto Scaling** – to automatically add or remove servers based on traffic.
- **Amazon CloudFront** – as a content delivery network (CDN) to speed up load times for customers worldwide.
- **Amazon RDS (Multi-AZ)** or **Amazon DynamoDB** – for a highly available database layer.

---

## Multi-Cloud Decision Matrix (Checkpoint 6)

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | AWS | Low-cost entry, pay-as-you-go pricing, and serverless options that scale with growth. |
| Enterprise Organization | AWS | Broadest service catalog and proven track record for large, complex workloads. |
| Microsoft Environment | Microsoft Azure | Native integration with Active Directory, Microsoft 365, and Windows Server. |
| AI / Machine Learning | Google Cloud Platform | Strong AI/ML tooling (Vertex AI) built on Google's own research infrastructure. |
| Kubernetes Deployment | Google Cloud Platform | Google created Kubernetes; GKE is one of the most mature managed Kubernetes services. |
| Global Web Application | AWS | Largest number of Regions/Availability Zones and mature global CDN and auto-scaling tools. |

## References
- AWS Free Tier – https://aws.amazon.com/free/
- Microsoft Entra ID overview – https://learn.microsoft.com/en-us/entra/fundamentals/whatis
- Vertex AI overview – https://cloud.google.com/vertex-ai/docs/start/introduction-unified-platform
