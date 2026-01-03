# ☁️ AWS Cloud 101: Ultimate Revision Sheet

A comprehensive revision guide based on the AWS Educate "Introduction to Cloud 101" course.

---

## 📚 MODULE 1: Introduction to Cloud Computing

### • Client-Server Model
* **What it is:** The fundamental model of modern computing where a client (device/app) makes a request, and a server (computer/service) fulfills it.
* **Why it is used:** To enable interaction with applications and websites over the internet.
* **Key points:**
    * **Client:** Web browser or desktop application.
    * **Server:** Computers or services like Amazon EC2 that evaluate and fulfill requests.
* **Real-world example:** Clicking a link for a news article (Client request) and the website sending the text/images back to you (Server response).
* **Keywords:** Request, Response, Amazon EC2.

### • Cloud Computing
* **What it is:** The on-demand delivery of IT resources (compute, database, storage) via the internet with pay-as-you-go pricing.
* **Why it is used:** To access resources dynamically without owning physical hardware.
* **Key points:**
    * **Programmable:** Quickly set up and tear down resources.
    * **Dynamic:** Access resources instantly to meet customer needs.
    * **Pay-as-you-go:** Test systems without full commitment.
* **Real-world example:** Instead of buying a server to host a website, you rent one from AWS for a few hours and pay only for that time.
* **Keywords:** On-demand, Pay-as-you-go, Agility.

### • Six Benefits of Cloud Computing
* **What it is:** The strategic advantages of using cloud over traditional data centers.
* **Key points:**
    * **Trade upfront expense for variable expense:** Pay only for what you use instead of investing heavily first.
    * **Stop spending money on data centers:** Eliminate costs of running and maintaining physical infrastructure.
    * **Stop guessing capacity:** Scale automatically instead of over-provisioning.
    * **Economies of scale:** Benefit from AWS's massive scale to get lower prices.
    * **Increase speed and agility:** Launch resources in minutes.
    * **Go global in minutes:** Deploy apps worldwide quickly.
* **Real-world example:** A startup can launch a global video app without building a single data center.
* **Keywords:** Variable Expense, Agility, Global Reach.

### • Deployment Models (Cloud Service Models)
* **What it is:** Categories defining the level of control and management you have over the infrastructure.
* **Key points:**
    * **IaaS (Infrastructure as a Service):** You manage the OS and apps; AWS provides the hardware (e.g., EC2).
    * **PaaS (Platform as a Service):** AWS manages the OS/hardware; you focus on code/deployment.
    * **SaaS (Software as a Service):** You use the completed software; AWS manages everything (e.g., Gmail).
* **Real-world example:**
    * **IaaS:** Renting a car (you drive/maintain fuel).
    * **SaaS:** Taking a bus (you just ride).
* **Keywords:** IaaS, PaaS, SaaS, Control.

### • Deployment Strategies
* **What it is:** Where the infrastructure physically resides.
* **Key points:**
    * **Cloud:** All parts of the application run in the cloud.
    * **Hybrid:** Connects cloud resources with on-premises infrastructure.
    * **On-premises:** Resources are deployed in your own data center (Private Cloud).
* **Real-world example:** A bank keeps legacy data in its own building (On-premises) but runs its mobile app on AWS (Cloud), connecting the two (Hybrid).
* **Keywords:** Hybrid, Migration, Connectivity.

---

## 🏗️ MODULE 2: Introduction to AWS Infrastructure

### • AWS Global Infrastructure
* **What it is:** The physical arrangement of AWS data centers worldwide.
* **Key points:**
    * **Region:** A physical geographic location containing multiple Availability Zones.
    * **Availability Zone (AZ):** One or more discrete data centers with redundant power and networking.
    * **Edge Location:** Sites used to cache content closer to users for lower latency.
* **Real-world example:** Storing data in the "Ohio Region" inside "Availability Zone A".
* **Keywords:** Region, AZ, Edge Location, Reliability.

### • Shared Responsibility Model
* **What it is:** A framework defining security obligations for AWS and the customer.
* **Key points:**
    * **Security OF the Cloud (AWS):** Physical hardware, global infrastructure, networking, and facilities.
    * **Security IN the Cloud (Customer):** Customer data, encryption, OS patching, firewall configuration.
* **Real-world example:** AWS locks the data center doors (Physical security); you set a password for your database (Data security).
* **Keywords:** Of the Cloud, In the Cloud, Patching, Encryption.

### • AWS Well-Architected Framework
* **What it is:** A set of best practices for designing high-quality systems.
* **Key points (The 6 Pillars):**
    * **Operational Excellence:** Running and monitoring systems to deliver business value.
    * **Security:** Protecting information and systems.
    * **Reliability:** Recovering from disruptions and acquiring resources dynamically.
    * **Performance Efficiency:** Using resources efficiently as demand changes.
    * **Cost Optimization:** Delivering value at the lowest price point.
    * **Sustainability:** Minimizing environmental impact.
* **Real-world example:** Designing a system that automatically heals after a crash (Reliability) and shuts down at night to save money (Cost Optimization).
* **Keywords:** Pillars, Design Principles, Efficiency.

### • Total Cost of Ownership (TCO)
* **What it is:** A metric to estimate direct and indirect costs of a product/service.
* **Why it is used:** To compare the cost of on-premises infrastructure vs. Cloud.
* **Key points:**
    * Includes costs like procurement, management, maintenance, and decommissioning.
    * **AWS Pricing Calculator:** Tool to estimate costs for AWS products.
* **Real-world example:** Calculating not just the server purchase price, but the electricity and IT staff salary required to run it.
* **Keywords:** Calculator, Estimate, Indirect Costs.

### • AWS Pricing Models
* **What it is:** Flexible payment options for using AWS services.
* **Key points:**
    * **Pay-as-you-go:** No upfront cost; adapt to changing needs without over-committing.
    * **Save when you reserve:** Commit to a 1 or 3-year term (Savings Plans) for a discount.
    * **Pay less by using more:** Volume-based discounts (e.g., S3 storage gets cheaper as you store more).
* **Real-world example:** Paying a monthly electric bill (Pay-as-you-go) vs. signing a year-long gym contract for a lower rate (Reserved).
* **Keywords:** On-Demand, Reservations, Volume Discounts.

### • AWS Free Tier
* **What it is:** Offers that allow users to try AWS services for free.
* **Key points:**
    * **Always Free:** Offers that never expire (e.g., Lambda 1M requests/month).
    * **12 Months Free:** Free for the first year after sign-up (e.g., EC2 t2.micro).
    * **Trials:** Short-term free trials starting from activation (e.g., SageMaker for 2 months).
* **Real-world example:** A 30-day free trial for a streaming service.
* **Keywords:** Always Free, 12 Months, Trials.

---

## 🛠️ MODULE 4: AWS Core Services

### • Amazon VPC (Virtual Private Cloud)
* **What it is:** A logically isolated virtual network where you launch resources.
* **Why it is used:** To control network configuration, IP ranges, and security.
* **Key points:**
    * **Subnets:** Segments of the VPC (Public for web servers, Private for backend systems).
    * **Security:** Uses security groups and network ACLs.
    * **Cost:** The VPC itself is free; you pay for resources inside it.
* **Real-world example:** A secure office building (VPC) with a public lobby (Public Subnet) and restricted employee-only zones (Private Subnet).
* **Keywords:** Network, Isolation, Subnets, Public/Private.

### • Amazon EC2 (Elastic Compute Cloud)
* **What it is:** A web service providing resizable compute capacity (virtual servers) in the cloud.
* **Why it is used:** To host applications without buying hardware.
* **Key points:**
    * **Control:** Gives full control over computing resources.
    * **Flexible:** Scale up or down as needed.
    * **Instance Types:** Various configurations (CPU, Memory) for different needs.
    * **Pricing:** On-Demand, Spot Instances, Reserved Instances.
* **Real-world example:** Renting a powerful computer remotely to process large data files because your laptop is too slow.
* **Keywords:** Virtual Server, Compute, Instances, Resizable.

### • Amazon RDS (Relational Database Service)
* **What it is:** A managed distributed relational database service.
* **Why it is used:** To set up, operate, and scale databases without managing administrative tasks.
* **Key points:**
    * **Managed:** AWS handles patching, backups, and recovery automatically.
    * **Scalable:** Resize capacity as needed.
    * **High Availability:** Multi-AZ deployments for disaster recovery.
* **Real-world example:** Using a service that automatically organizes and backs up your filing cabinet (RDS) vs. doing it manually (EC2 Database).
* **Keywords:** Managed, SQL, Patching, Multi-AZ.

### • Amazon S3 (Simple Storage Service)
* **What it is:** Object storage built to store and retrieve any amount of data.
* **Why it is used:** For durability, availability, and virtually unlimited scalability at low cost.
* **Key points:**
    * **Objects:** Files are stored as objects in buckets.
    * **Durability:** Data is replicated across multiple Availability Zones.
    * **Use Cases:** Backup, archiving, static website hosting.
* **Real-world example:** Storing millions of user-uploaded photos for a social media app.
* **Keywords:** Buckets, Objects, Unlimited Storage, Static Web Hosting.

### • AWS Lambda
* **What it is:** A serverless compute service that runs code in response to events.
* **Why it is used:** To run code without provisioning or managing servers.
* **Key points:**
    * **No Servers:** AWS manages all infrastructure.
    * **Event-Driven:** Triggered by changes in data (e.g., S3 upload).
    * **Pay-per-use:** Pay only for the compute time used (milliseconds).
    * **Limit:** 15-minute max runtime per function.
* **Real-world example:** Automatically resizing an image the moment it is uploaded to a website.
* **Keywords:** Serverless, Event-driven, 15-min limit.

### • Amazon DynamoDB
* **What it is:** A fast, serverless, non-relational (NoSQL) database.
* **Why it is used:** For applications requiring single-digit millisecond latency at any scale.
* **Key points:**
    * **Key-Value:** Stores data in simple pairs rather than relational tables.
    * **Serverless:** No servers to patch or manage.
    * **Performance:** Handles millions of requests per second.
* **Real-world example:** A gaming leaderboard that updates scores instantly for millions of players.
* **Keywords:** NoSQL, Key-Value, Millisecond Latency.

### • Amazon CloudWatch
* **What it is:** A monitoring and observability service.
* **Why it is used:** To collect data and actionable insights to monitor applications.
* **Key points:**
    * **Metrics:** Collects logs and metrics (e.g., CPU usage).
    * **Alarms:** Triggers automated actions or alerts when thresholds are met.
    * **Free Tier:** Basic monitoring (5-minute intervals) is free; detailed (1-minute) costs extra.
* **Real-world example:** Receiving an alert on your phone if your website's server CPU usage goes above 80%.
* **Keywords:** Monitoring, Alarms, Metrics, Logs.

### • Amazon SNS (Simple Notification Service)
* **What it is:** A fully managed messaging service for pub/sub communication.
* **Why it is used:** To decouple microservices and send notifications.
* **Key points:**
    * **Publish/Subscribe:** Topics distribute messages to multiple subscribers.
    * **Protocols:** Supports SMS, Email, Mobile Push, HTTP.
    * **Durability:** Messages are stored across multiple AZs.
* **Real-world example:** Sending a "Your Order has Shipped" text message to a customer.
* **Keywords:** Pub/Sub, Topics, Notifications, SMS.

### • AWS IAM (Identity and Access Management)
* **What it is:** A service to manage access to AWS resources securely.
* **Why it is used:** To control who is authenticated (signed in) and authorized (has permissions).
* **Key points:**
    * **Users/Groups/Roles:** Entities used to manage access.
    * **Least Privilege:** Granting only the permissions necessary to perform a task.
    * **Cost:** Offered at no additional charge.
* **Real-world example:** Creating a specific username for an employee that only allows them to view S3 buckets but not delete them.
* **Keywords:** Permissions, Policies, Authentication, Authorization.

---

## 💼 MODULE 5: Cloud Careers

### • Cloud Career Pathways
* **What it is:** Diverse job roles available in the cloud computing industry.
* **Key Roles:**
    * **Solutions Architect:** Designs cloud infrastructure and applications.
    * **Cloud Support Specialist:** Provides technical support for cloud services.
    * **DevOps Engineer:** Focuses on deployment, automation, and operations.
* **Requirements:** Basic IT knowledge, scripting (Python/Java), and AWS Certifications.
* **Keywords:** Architect, DevOps, Certification, Roles.
