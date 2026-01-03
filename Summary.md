# ☁️ AWS Cloud 101: Ultimate Revision Sheet

A comprehensive revision guide based on the AWS Educate "Introduction to Cloud 101" course.

---

## 📚 MODULE 1: Introduction to Cloud Computing

### • Client-Server Model
* [cite_start]**What it is:** The fundamental model of modern computing where a client (device/app) makes a request, and a server (computer/service) fulfills it[cite: 3].
* [cite_start]**Why it is used:** To enable interaction with applications and websites over the internet[cite: 3].
* **Key points:**
    * [cite_start]**Client:** Web browser or desktop application[cite: 3].
    * [cite_start]**Server:** Computers or services like Amazon EC2 that evaluate and fulfill requests[cite: 3].
* [cite_start]**Real-world example:** Clicking a link for a news article (Client request) and the website sending the text/images back to you (Server response)[cite: 3].
* **Keywords:** Request, Response, Amazon EC2.

### • Cloud Computing
* [cite_start]**What it is:** The on-demand delivery of IT resources (compute, database, storage) via the internet with pay-as-you-go pricing[cite: 2].
* [cite_start]**Why it is used:** To access resources dynamically without owning physical hardware[cite: 2].
* **Key points:**
    * [cite_start]**Programmable:** Quickly set up and tear down resources[cite: 2].
    * [cite_start]**Dynamic:** Access resources instantly to meet customer needs[cite: 2].
    * [cite_start]**Pay-as-you-go:** Test systems without full commitment[cite: 2].
* **Real-world example:** Instead of buying a server to host a website, you rent one from AWS for a few hours and pay only for that time.
* **Keywords:** On-demand, Pay-as-you-go, Agility.

### • Six Benefits of Cloud Computing
* [cite_start]**What it is:** The strategic advantages of using cloud over traditional data centers[cite: 4].
* **Key points:**
    * [cite_start]**Trade upfront expense for variable expense:** Pay only for what you use instead of investing heavily first[cite: 4].
    * [cite_start]**Stop spending money on data centers:** Eliminate costs of running and maintaining physical infrastructure[cite: 4].
    * [cite_start]**Stop guessing capacity:** Scale automatically instead of over-provisioning[cite: 4].
    * [cite_start]**Economies of scale:** Benefit from AWS's massive scale to get lower prices[cite: 4].
    * [cite_start]**Increase speed and agility:** Launch resources in minutes[cite: 4].
    * [cite_start]**Go global in minutes:** Deploy apps worldwide quickly[cite: 4].
* **Real-world example:** A startup can launch a global video app without building a single data center.
* **Keywords:** Variable Expense, Agility, Global Reach.

### • Deployment Models (Cloud Service Models)
* [cite_start]**What it is:** Categories defining the level of control and management you have over the infrastructure[cite: 5].
* **Key points:**
    * **IaaS (Infrastructure as a Service):** You manage the OS and apps; [cite_start]AWS provides the hardware (e.g., EC2)[cite: 5].
    * [cite_start]**PaaS (Platform as a Service):** AWS manages the OS/hardware; you focus on code/deployment[cite: 5].
    * **SaaS (Software as a Service):** You use the completed software; [cite_start]AWS manages everything (e.g., Gmail)[cite: 5].
* **Real-world example:**
    * **IaaS:** Renting a car (you drive/maintain fuel).
    * **SaaS:** Taking a bus (you just ride).
* **Keywords:** IaaS, PaaS, SaaS, Control.

### • Deployment Strategies
* [cite_start]**What it is:** Where the infrastructure physically resides[cite: 5].
* **Key points:**
    * [cite_start]**Cloud:** All parts of the application run in the cloud[cite: 5].
    * [cite_start]**Hybrid:** Connects cloud resources with on-premises infrastructure[cite: 5].
    * [cite_start]**On-premises:** Resources are deployed in your own data center (Private Cloud)[cite: 5].
* **Real-world example:** A bank keeps legacy data in its own building (On-premises) but runs its mobile app on AWS (Cloud), connecting the two (Hybrid).
* **Keywords:** Hybrid, Migration, Connectivity.

---

## 🏗️ MODULE 2: Introduction to AWS Infrastructure

### • AWS Global Infrastructure
* [cite_start]**What it is:** The physical arrangement of AWS data centers worldwide[cite: 13].
* **Key points:**
    * [cite_start]**Region:** A physical geographic location containing multiple Availability Zones[cite: 13].
    * [cite_start]**Availability Zone (AZ):** One or more discrete data centers with redundant power and networking[cite: 13, 14].
    * [cite_start]**Edge Location:** Sites used to cache content closer to users for lower latency[cite: 13].
* [cite_start]**Real-world example:** Storing data in the "Ohio Region" inside "Availability Zone A"[cite: 14].
* **Keywords:** Region, AZ, Edge Location, Reliability.

### • Shared Responsibility Model
* [cite_start]**What it is:** A framework defining security obligations for AWS and the customer[cite: 15].
* **Key points:**
    * [cite_start]**Security OF the Cloud (AWS):** Physical hardware, global infrastructure, networking, and facilities[cite: 16].
    * [cite_start]**Security IN the Cloud (Customer):** Customer data, encryption, OS patching, firewall configuration[cite: 16].
* [cite_start]**Real-world example:** AWS locks the data center doors (Physical security); you set a password for your database (Data security)[cite: 16].
* **Keywords:** Of the Cloud, In the Cloud, Patching, Encryption.

### • AWS Well-Architected Framework
* [cite_start]**What it is:** A set of best practices for designing high-quality systems[cite: 17].
* **Key points (The 6 Pillars):**
    * [cite_start]**Operational Excellence:** Running and monitoring systems to deliver business value[cite: 18].
    * [cite_start]**Security:** Protecting information and systems[cite: 21].
    * [cite_start]**Reliability:** Recovering from disruptions and acquiring resources dynamically[cite: 24].
    * [cite_start]**Performance Efficiency:** Using resources efficiently as demand changes[cite: 25].
    * [cite_start]**Cost Optimization:** Delivering value at the lowest price point[cite: 27].
    * [cite_start]**Sustainability:** Minimizing environmental impact[cite: 30].
* **Real-world example:** Designing a system that automatically heals after a crash (Reliability) and shuts down at night to save money (Cost Optimization).
* **Keywords:** Pillars, Design Principles, Efficiency.

### • Total Cost of Ownership (TCO)
* [cite_start]**What it is:** A metric to estimate direct and indirect costs of a product/service[cite: 34].
* [cite_start]**Why it is used:** To compare the cost of on-premises infrastructure vs. Cloud[cite: 34].
* **Key points:**
    * [cite_start]Includes costs like procurement, management, maintenance, and decommissioning[cite: 34].
    * [cite_start]**AWS Pricing Calculator:** Tool to estimate costs for AWS products[cite: 36].
* **Real-world example:** Calculating not just the server purchase price, but the electricity and IT staff salary required to run it.
* **Keywords:** Calculator, Estimate, Indirect Costs.

### • AWS Pricing Models
* [cite_start]**What it is:** Flexible payment options for using AWS services[cite: 38].
* **Key points:**
    * [cite_start]**Pay-as-you-go:** No upfront cost; adapt to changing needs without over-committing[cite: 39].
    * [cite_start]**Save when you reserve:** Commit to a 1 or 3-year term (Savings Plans) for a discount[cite: 42, 43].
    * [cite_start]**Pay less by using more:** Volume-based discounts (e.g., S3 storage gets cheaper as you store more)[cite: 47].
* **Real-world example:** Paying a monthly electric bill (Pay-as-you-go) vs. signing a year-long gym contract for a lower rate (Reserved).
* **Keywords:** On-Demand, Reservations, Volume Discounts.

### • AWS Free Tier
* [cite_start]**What it is:** Offers that allow users to try AWS services for free[cite: 45].
* **Key points:**
    * [cite_start]**Always Free:** Offers that never expire (e.g., Lambda 1M requests/month)[cite: 49].
    * [cite_start]**12 Months Free:** Free for the first year after sign-up (e.g., EC2 t2.micro)[cite: 51, 52].
    * [cite_start]**Trials:** Short-term free trials starting from activation (e.g., SageMaker for 2 months)[cite: 54, 56].
* **Real-world example:** A 30-day free trial for a streaming service.
* **Keywords:** Always Free, 12 Months, Trials.

---

## 🛠️ MODULE 4: AWS Core Services

### • Amazon VPC (Virtual Private Cloud)
* [cite_start]**What it is:** A logically isolated virtual network where you launch resources[cite: 78].
* [cite_start]**Why it is used:** To control network configuration, IP ranges, and security[cite: 79].
* **Key points:**
    * [cite_start]**Subnets:** Segments of the VPC (Public for web servers, Private for backend systems)[cite: 80, 81].
    * [cite_start]**Security:** Uses security groups and network ACLs[cite: 81].
    * [cite_start]**Cost:** The VPC itself is free; you pay for resources inside it[cite: 93].
* **Real-world example:** A secure office building (VPC) with a public lobby (Public Subnet) and restricted employee-only zones (Private Subnet).
* **Keywords:** Network, Isolation, Subnets, Public/Private.

### • Amazon EC2 (Elastic Compute Cloud)
* [cite_start]**What it is:** A web service providing resizable compute capacity (virtual servers) in the cloud[cite: 95].
* [cite_start]**Why it is used:** To host applications without buying hardware[cite: 96].
* **Key points:**
    * [cite_start]**Control:** Gives full control over computing resources[cite: 97].
    * [cite_start]**Flexible:** Scale up or down as needed[cite: 99].
    * [cite_start]**Instance Types:** Various configurations (CPU, Memory) for different needs[cite: 101].
    * [cite_start]**Pricing:** On-Demand, Spot Instances, Reserved Instances[cite: 111].
* **Real-world example:** Renting a powerful computer remotely to process large data files because your laptop is too slow.
* **Keywords:** Virtual Server, Compute, Instances, Resizable.

### • Amazon RDS (Relational Database Service)
* [cite_start]**What it is:** A managed distributed relational database service[cite: 112].
* [cite_start]**Why it is used:** To set up, operate, and scale databases without managing administrative tasks[cite: 112].
* **Key points:**
    * [cite_start]**Managed:** AWS handles patching, backups, and recovery automatically[cite: 112, 124].
    * [cite_start]**Scalable:** Resize capacity as needed[cite: 116].
    * [cite_start]**High Availability:** Multi-AZ deployments for disaster recovery[cite: 119].
* **Real-world example:** Using a service that automatically organizes and backs up your filing cabinet (RDS) vs. doing it manually (EC2 Database).
* **Keywords:** Managed, SQL, Patching, Multi-AZ.

### • Amazon S3 (Simple Storage Service)
* [cite_start]**What it is:** Object storage built to store and retrieve any amount of data[cite: 185].
* [cite_start]**Why it is used:** For durability, availability, and virtually unlimited scalability at low cost[cite: 185].
* **Key points:**
    * [cite_start]**Objects:** Files are stored as objects in buckets[cite: 185].
    * [cite_start]**Durability:** Data is replicated across multiple Availability Zones[cite: 187].
    * [cite_start]**Use Cases:** Backup, archiving, static website hosting[cite: 191].
* **Real-world example:** Storing millions of user-uploaded photos for a social media app.
* **Keywords:** Buckets, Objects, Unlimited Storage, Static Web Hosting.

### • AWS Lambda
* [cite_start]**What it is:** A serverless compute service that runs code in response to events[cite: 203].
* [cite_start]**Why it is used:** To run code without provisioning or managing servers[cite: 203].
* **Key points:**
    * [cite_start]**No Servers:** AWS manages all infrastructure[cite: 205].
    * [cite_start]**Event-Driven:** Triggered by changes in data (e.g., S3 upload)[cite: 205].
    * [cite_start]**Pay-per-use:** Pay only for the compute time used (milliseconds)[cite: 218].
    * [cite_start]**Limit:** 15-minute max runtime per function[cite: 216].
* **Real-world example:** Automatically resizing an image the moment it is uploaded to a website.
* **Keywords:** Serverless, Event-driven, 15-min limit.

### • Amazon DynamoDB
* [cite_start]**What it is:** A fast, serverless, non-relational (NoSQL) database[cite: 221].
* [cite_start]**Why it is used:** For applications requiring single-digit millisecond latency at any scale[cite: 225].
* **Key points:**
    * [cite_start]**Key-Value:** Stores data in simple pairs rather than relational tables[cite: 221].
    * [cite_start]**Serverless:** No servers to patch or manage[cite: 225].
    * [cite_start]**Performance:** Handles millions of requests per second[cite: 223].
* **Real-world example:** A gaming leaderboard that updates scores instantly for millions of players.
* **Keywords:** NoSQL, Key-Value, Millisecond Latency.

### • Amazon CloudWatch
* [cite_start]**What it is:** A monitoring and observability service[cite: 132].
* [cite_start]**Why it is used:** To collect data and actionable insights to monitor applications[cite: 132].
* **Key points:**
    * [cite_start]**Metrics:** Collects logs and metrics (e.g., CPU usage)[cite: 134].
    * [cite_start]**Alarms:** Triggers automated actions or alerts when thresholds are met[cite: 135].
    * [cite_start]**Free Tier:** Basic monitoring (5-minute intervals) is free; detailed (1-minute) costs extra[cite: 147].
* **Real-world example:** Receiving an alert on your phone if your website's server CPU usage goes above 80%.
* **Keywords:** Monitoring, Alarms, Metrics, Logs.

### • Amazon SNS (Simple Notification Service)
* [cite_start]**What it is:** A fully managed messaging service for pub/sub communication[cite: 153].
* [cite_start]**Why it is used:** To decouple microservices and send notifications[cite: 153].
* **Key points:**
    * [cite_start]**Publish/Subscribe:** Topics distribute messages to multiple subscribers[cite: 153].
    * [cite_start]**Protocols:** Supports SMS, Email, Mobile Push, HTTP[cite: 157].
    * [cite_start]**Durability:** Messages are stored across multiple AZs[cite: 157].
* **Real-world example:** Sending a "Your Order has Shipped" text message to a customer.
* **Keywords:** Pub/Sub, Topics, Notifications, SMS.

### • AWS IAM (Identity and Access Management)
* [cite_start]**What it is:** A service to manage access to AWS resources securely[cite: 171].
* [cite_start]**Why it is used:** To control who is authenticated (signed in) and authorized (has permissions)[cite: 171].
* **Key points:**
    * [cite_start]**Users/Groups/Roles:** Entities used to manage access[cite: 171].
    * [cite_start]**Least Privilege:** Granting only the permissions necessary to perform a task[cite: 174].
    * [cite_start]**Cost:** Offered at no additional charge[cite: 182].
* **Real-world example:** Creating a specific username for an employee that only allows them to view S3 buckets but not delete them.
* **Keywords:** Permissions, Policies, Authentication, Authorization.

---

## 💼 MODULE 5: Cloud Careers

### • Cloud Career Pathways
* [cite_start]**What it is:** Diverse job roles available in the cloud computing industry[cite: 254].
* **Key Roles:**
    * [cite_start]**Solutions Architect:** Designs cloud infrastructure and applications[cite: 254].
    * [cite_start]**Cloud Support Specialist:** Provides technical support for cloud services[cite: 254].
    * [cite_start]**DevOps Engineer:** Focuses on deployment, automation, and operations[cite: 254].
* [cite_start]**Requirements:** Basic IT knowledge, scripting (Python/Java), and AWS Certifications[cite: 248].
* **Keywords:** Architect, DevOps, Certification, Roles.
