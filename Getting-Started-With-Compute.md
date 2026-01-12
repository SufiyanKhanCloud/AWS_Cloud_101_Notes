# AWS Educate: Getting Started with Compute – Comprehensive Notes

These notes document my learning from the **AWS Educate “Getting Started with Compute”** course.  
They cover core computing fundamentals, AWS compute services, Amazon EC2 deep-dive concepts, instance configuration, scaling, and assessment preparation.

---

## 1. Fundamentals of Computing

Core components involved in computing:

- **CPU (Central Processing Unit):** Executes instructions (the “brain” of the system).
- **RAM (Random Access Memory):** Temporary memory for active tasks.
- **Storage (Hard Drive):** Long-term data storage (OS, applications, files).
- **Networking:**
  - **Bandwidth:** Amount of data transferred over time.
  - **Latency:** Time taken for data to travel between systems.

---

## 2. Why Cloud Compute?

Key benefits of using compute resources in the cloud:

- **Cost Efficiency:** Pay only for what you use; no upfront infrastructure costs.
- **Scalability:** Instantly scale resources up or down.
- **Reliability:** Built-in fault tolerance and high availability.

---

## 3. AWS Compute Service Categories

AWS provides multiple compute options based on workload requirements:

| Category | Description | AWS Services |
|-------|------------|-------------|
| **Virtual Machines** | Traditional servers with full OS control | Amazon EC2 |
| **Containers** | Package apps with dependencies in isolated environments | Amazon ECS, Amazon EKS |
| **Serverless** | Run code without managing servers | AWS Lambda, AWS Fargate |
| **PaaS / Web Hosting** | Simplified app deployment | AWS Elastic Beanstalk |

**Hybrid deployments** combine on-premises infrastructure with AWS cloud services.

---

## 4. Amazon EC2 (Elastic Compute Cloud)

### Key Benefits
- Elastic scaling in minutes
- Full OS-level control
- Multiple instance types and OS choices
- Integrated with AWS services (S3, RDS, VPC)
- Pay-as-you-go pricing
- Secure networking using VPC and Security Groups

---

## 5. EC2 Architecture Components

- **Region:** Geographic area containing AWS infrastructure.
- **Availability Zones (AZs):** Isolated data centers within a region.
- **VPC:** Logically isolated virtual network.
- **Subnets:** Network segments inside a VPC.
  - Public Subnet → Internet access
  - Private Subnet → No direct internet access

Best practice: Deploy instances across multiple AZs for fault tolerance.

---

## 6. EC2 Instance Lifecycle

1. Pending (not billed)
2. Running (billed)
3. Stopping
4. Stopped (storage billed)
5. Shutting-down
6. Terminated (deleted)

---

## 7. EC2 Pricing & Purchasing Options

| Option | Use Case |
|-----|---------|
| **On-Demand** | Short-term, unpredictable workloads |
| **Reserved Instances** | Long-term, steady workloads |
| **Savings Plans** | Flexible long-term compute usage |
| **Spot Instances** | Fault-tolerant workloads with flexible timing |

---

## 8. EC2 Tenancy Models

- **Shared (Default):** Lowest cost
- **Dedicated Instances:** Dedicated hardware
- **Dedicated Hosts:** Required for compliance and licensing needs

---

## 9. Launching an EC2 Instance – 7 Key Steps

1. **Name & Tags:** Resource organization and cost tracking  
2. **AMI:** OS and application template  
3. **Instance Type:** CPU, memory, and network capacity  
4. **Key Pair:** Secure access (SSH/RDP)  
5. **Network Settings:** VPC, Subnet, Security Groups  
6. **Storage Configuration:** EBS or Instance Store  
7. **Advanced Settings:** User data, IAM roles, monitoring

---

## 10. Storage Options for EC2

### Amazon EBS
- Persistent, AZ-specific block storage
- Supports snapshots and encryption

### Instance Store
- Ephemeral storage
- Data lost on stop/termination
- Ideal for temporary data (cache, buffers)

---

## 11. Scaling & Load Balancing

### Scaling Types
- **Vertical Scaling:** Resize instance (downtime required)
- **Horizontal Scaling:** Add/remove instances (no downtime)

### Auto Scaling
- Dynamic
- Predictive
- Scheduled

### Elastic Load Balancing
- **Application Load Balancer (ALB):** Layer 7
- **Network Load Balancer (NLB):** Layer 4
- **Gateway Load Balancer:** Layer 3

---

## 12. Connecting to EC2 Instances

- EC2 Instance Connect
- Session Manager
- SSH Client
- EC2 Serial Console

---

## 13. Assessment & Exam Quick Reference

- Serverless workloads → **AWS Lambda**
- Container orchestration → **Amazon EKS**
- Cost-efficient flexible workloads → **Spot Instances**
- Persistent storage → **Amazon EBS**
- Traffic distribution → **Elastic Load Balancing**
- Auto Scaling → **Horizontal Scaling**

---

## Key Takeaways

- AWS offers multiple compute models for different workloads.
- Amazon EC2 provides full control and flexibility.
- Scaling and load balancing are essential for reliability and performance.
- Cost optimization depends on selecting the right purchasing model.

---

*These notes are part of my AWS Educate learning journey and are maintained for revision, documentation, and portfolio purposes.*
