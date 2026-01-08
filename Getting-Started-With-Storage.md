# AWS Educate: Getting Started with Storage - Lab Notes

These are consolidated revision notes for the **AWS Educate "Getting Started with Storage"** lab, summarizing core concepts, key services, and assessment questions for quick reference.

---

## 1. Cloud Storage Basics

AWS provides three main categories of cloud storage:

- **Block Storage (Amazon EBS)**  
  - Stores data in fixed-size chunks (blocks) with unique identifiers.  
  - Commonly used for databases, enterprise applications, and boot drives.  

- **File Storage (Amazon EFS)**  
  - Data is stored in a hierarchical structure of directories and files.  
  - Supports shared access across multiple instances.  

- **Object Storage (Amazon S3)**  
  - Stores data as objects with metadata and a unique ID.  
  - Ideal for media hosting, backups, web content, and archives.  

**Key Benefits:** Cost-efficient, secure, scalable, accessible, managed, and backed up.

---

## 2. Amazon S3 (Simple Storage Service)

**Core Concepts:**
- **Buckets:** Containers for objects, must be globally unique, lowercase, 3–63 characters, no spaces.  
- **Objects:** Files plus metadata and a unique key.  
- **Regions:** Data can be stored in a specific AWS region based on latency or compliance needs.  

**Storage Classes:**
| Class | Use Case |
| --- | --- |
| S3 Standard | Frequently accessed data (websites, mobile apps) |
| S3 Standard-IA | Infrequently accessed, rapid retrieval (backups, DR) |
| S3 One Zone-IA | Single AZ storage, lower cost |
| S3 Glacier Flexible Retrieval | Archives, retrieval in minutes to hours |
| S3 Glacier Deep Archive | Long-term retention (7+ years), rarely accessed |
| S3 Intelligent-Tiering | Auto moves data between tiers based on usage |

**Costs & Limits:**
- **Charged for:** Storage (GB/month), outbound transfer, requests (PUT, GET, COPY, etc.)  
- **Free:** Inbound transfer and intra-region S3 transfers  
- **Object Size Limit:** 5 TB max per object  
- **Multipart Upload:** Recommended for files >100 MB  
- **Console Upload Limit:** 160 GB  

**Key Features:**
- **Versioning:** Maintain multiple versions of objects  
- **Lifecycle Rules:** Automate transitions to cheaper tiers or deletions  
- **Replication:** Cross-Region (CRR) or Same-Region (SRR) replication  
- **Security:** Block Public Access, Bucket Policies, Server-side & Client-side Encryption  
- **Data Transfer:** S3 Transfer Acceleration, Snow Family (Snowcone, Snowball, Snowmobile)

---

## 3. Amazon EBS (Elastic Block Store)

- **Type:** Block storage attached to a single EC2 instance.  
- **Characteristics:**  
  - AZ-specific, persistent, supports snapshots (incremental), AES-256 encryption.  
- **Volume Types:**  
  - SSD (General Purpose) – balanced price/performance  
  - SSD (Provisioned IOPS) – high performance for databases  
  - HDD (Throughput Optimized) – big data, logs  
  - HDD (Cold) – lowest cost, infrequently accessed data  

---

## 4. Amazon EFS (Elastic File System)

- **Type:** Fully managed file storage (NFS protocol)  
- **Features:**  
  - Shared access by multiple EC2 instances  
  - Elastic, automatically scales  
  - Regional storage across multiple AZs for durability (99.999999999%)  
- **Use Cases:** CMS, media processing, home directories  

---

## 5. Comparison Cheat Sheet

| Feature | S3 (Object) | EBS (Block) | EFS (File) |
| --- | --- | --- | --- |
| Data Structure | Objects with IDs | Blocks on a drive | File hierarchy (folders) |
| Access | Web/API | Single EC2 instance | Multiple EC2 instances |
| Storage Location | Regional | Single AZ | Regional (multi-AZ) |
| Best For | Media, backups, web | Databases, boot drives | Shared folders, CMS |

---

**End of Notes**  
These notes consolidate key AWS storage concepts, services, features, and lab exercises for quick revision and hands-on lab preparation.
