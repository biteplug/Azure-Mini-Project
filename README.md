# Azure-Mini-Project
My first task for 3MTT program - setting up Azure management account

Azure Mini Project: Summary Report
Date: May 11, 2026
Prepared by: Nnenna Ewa
Project: Cloud Fundamentals & Azure Governance


1. Selected Region and Availability
Selected Region: East US (or North Europe)
Geographic Rationale:
For this deployment, I selected the East US region. While there are closer geographical regions such as South Africa North, East US often provides the widest array of Free Tier services and highly stable latency for users in West Africa. To ensure high availability, I reviewed the availability zones within this region, which provide physically separate data center locations to protect applications from local data center failures.

2. Resource Deployment Summary
Resource Type: Storage Account (PaaS)
Configuration:
•	Performance: Standard
•	Replication: Locally-Redundant Storage (LRS)
•	Logical Container: Created within a dedicated Resource Group for lifecycle management.

3. The Shared Responsibility Model
The Shared Responsibility Model defines the security and operational obligations between Microsoft Azure and the customer. For the Storage Account (Platform as a Service - PaaS) deployed in this project, the responsibilities are divided as follows:
•	Microsoft’s Responsibility: Microsoft is responsible for the physical security of the data centers, the underlying hardware (servers and drives), the virtualization layer, and the maintenance of the storage software/API. They ensure the "security of the cloud."
•	My (The Customer’s) Responsibility: I am responsible for the security "in" the cloud. This includes:
•	Data Governance: Managing the information stored within the account. 
•	Identity & Access Management: Configuring Shared Access Signatures (SAS), managing access keys, and setting up Role-Based Access Control (RBAC). 
•	Network Security: Configuring the storage firewall to restrict access to specific IP addresses. 
•	Data Protection: Enabling features like versioning or soft-delete to protect against accidental deletion.

4. Cost Management Strategy
To ensure the project remains within the Azure Free Tier limits, I implemented a Budget Alert set at a threshold of $1.00. I configured both Actual and Forecasted alerts. The forecasted alert acts as a proactive trigger, notifying me via email if my current usage patterns suggest I will exceed the budget by the end of the month, allowing for immediate remediation of resources.


