<div align="center">

# 🎯 Cloud Platform Recommendations

</div>

---

## 📑 Table of Contents
- [Cloud Platform Recommendation Challenge](#-cloud-platform-recommendation-challenge)
  - [Client A — Startup Company](#client-a--startup-company)
  - [Client B — University](#client-b--university)
  - [Client C — AI Research Company](#client-c--ai-research-company)
  - [Client D — Global E-Commerce Company](#client-d--global-e-commerce-company)
  - [Summary](#-summary)
- [Multi-Cloud Decision Matrix](#-multi-cloud-decision-matrix)

---

## 🎯 Cloud Platform Recommendation Challenge

### Client A — Startup Company
*Scenario: Limited budget, launching a mobile app, expects rapid growth.*

**Recommended Platform:** 🟧 **AWS**

AWS is a good choice for a startup because it offers flexible, pay-as-you-go services that can help control costs while the company is growing. AWS also provides many services that can easily scale as the mobile application gains more users. The startup could use Amazon EC2 for computing, Amazon S3 for storing files and images, and Amazon RDS for its database. It could also use AWS Lambda to run application functions without managing servers.

**Services:**
- Amazon EC2
- Amazon S3
- Amazon RDS
- AWS Lambda

---

### Client B — University
*Scenario: Already uses Windows Server, Microsoft 365, Active Directory. Wants to migrate some services to the cloud.*

**Recommended Platform:** 🔵 **Microsoft Azure**

Microsoft Azure is the best choice because the university already uses Windows Server, Microsoft 365, and Active Directory. Azure provides strong integration with Microsoft's existing technologies, making the migration easier and more convenient. The university could use Azure Virtual Machines for Windows workloads, Microsoft Entra ID for identity management, and Azure SQL Database for databases. Azure also supports hybrid-cloud environments, allowing the university to gradually move services to the cloud.

**Services:**
- Azure Virtual Machines
- Microsoft Entra ID
- Azure SQL Database
- Azure Blob Storage

---

### Client C — AI Research Company
*Scenario: Develops AI/ML applications requiring high-performance computing.*

**Recommended Platform:** 🔴 **Google Cloud Platform (GCP)**

Google Cloud is a strong choice for an AI research company because it provides powerful artificial intelligence and machine-learning tools. Google Cloud offers infrastructure designed for high-performance computing and specialized workloads such as machine learning. The company could use Vertex AI for developing and deploying AI models, Compute Engine for high-performance computing, and Google Kubernetes Engine (GKE) for managing containerized AI applications. Cloud Storage could also be used to store large datasets and research files.

**Services:**
- Vertex AI
- Compute Engine
- Google Kubernetes Engine (GKE)
- Cloud Storage

---

### Client D — Global E-Commerce Company
*Scenario: Multinational, requires high availability and automatic scaling.*

**Recommended Platform:** 🟧 **AWS**

AWS is a suitable choice for a global e-commerce company because it has a large global infrastructure and provides services designed for high availability and automatic scaling. The company can deploy applications across multiple regions and Availability Zones to improve reliability. It could use Amazon EC2 Auto Scaling for automatically adjusting computing capacity, Amazon S3 for storing product images and files, and Amazon RDS for managing its database. Amazon CloudFront could also improve the delivery speed of website content to customers around the world.

**Services:**
- Amazon EC2 Auto Scaling
- Amazon S3
- Amazon RDS
- Amazon CloudFront

---

### 📋 Summary

| Client | Recommended Platform | Main Reason |
|---|---|---|
| **Client A** – Startup | 🟧 AWS | Flexible costs and easy scalability |
| **Client B** – University | 🔵 Microsoft Azure | Strong Microsoft technology integration |
| **Client C** – AI Research | 🔴 Google Cloud | Strong AI/ML and high-performance computing capabilities |
| **Client D** – Global E-Commerce | 🟧 AWS | Global infrastructure, high availability, and automatic scaling |

---

## 🧩 Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| **Startup Company** | 🟧 AWS | AWS offers flexible, scalable services that allow startups to begin with small resources and expand as they grow. |
| **Enterprise Organization** | 🟧 AWS | AWS provides a wide range of services, strong security, and global infrastructure suitable for large organizations. |
| **Microsoft Environment** | 🔵 Microsoft Azure | Azure integrates closely with Microsoft products such as Windows Server, Microsoft 365, SQL Server, and Microsoft Entra ID. |
| **AI / Machine Learning** | 🔴 Google Cloud | Google Cloud provides powerful AI and machine-learning services such as Vertex AI and supports high-performance computing workloads. |
| **Kubernetes Deployment** | 🔴 Google Cloud | Google Kubernetes Engine (GKE) provides a managed Kubernetes environment for deploying and managing containerized applications. |
| **Global Web Application** | 🟧 AWS | AWS provides a large global infrastructure and services such as EC2, CloudFront, and Auto Scaling to support highly available and scalable web applications. |

---
