
#               Types of Cloud (Deployment Models)


# Public cloud
The cloud infrastructure is made available to the general public

Examples of Public Cloud:
Google App Engine
Microsoft Windows Azure
IBM Smart Cloud
Amazon EC2,Google Doc, Spreadsheet,


# Private cloud
The cloud infrastructure is operated solely for an organization.
•
Examples of Private Cloud:
— Eucalyptus
Ubuntu Enterprise Cloud - I-JEC
— Amazon VPC (Virtual Private Cloud)
— VMware Cloud Infrastructure Suite
— Microsoft ECl data center.
-Window Server 'Hyper-V'.

# Community cloud
The cloud infrastructure is shared by several organizations and supports a specific goal.
• Examples of Community Cloud:
• Google Apps for Government
• Microsoft Government Community Cloud


# Hybrid cloud
The cloud infrastructure is a composition of two or more clouds (private,
e.g Cloud Bursting for load balancing between clouds.
community, or public)

Examples of Hybrid Cloud:
— Windows Azure (capable of Hybrid Cloud)
— VMware vCloud (Hybrid Cloud Services)





Let’s break down the terms you mentioned — **Cloud Manager**, **Cluster Manager**, and **Computer Manager** — to clarify their meanings and roles in computing.

---

### **1. Cloud Manager**

A **Cloud Manager** is a platform or tool that helps organizations manage their cloud infrastructure and resources efficiently. It allows users to deploy, monitor, and control cloud-based services across private, public, or hybrid cloud environments.



Cloud Manager is the public access point to the cloud where subscribers sign up for accounts, manage the resources they rent
from the cloud, and access data stored in the cloud.

Cloud Manager has mechanism for:
— Authenticating subscribers
— Generating or validating access credentials that subscriber uses when
communicating with VMs.
— Top-level resource management.
For a subscriber's request cloud manager determines if the cloud has enough free resources to satisfy the request



#### **Key Functions:**
- **Resource Provisioning:** Launching virtual machines (VMs), containers, and storage resources in the cloud.
- **Cost Management:** Monitoring and optimizing cloud usage to control costs.
- **Monitoring and Alerts:** Tracking the health and performance of cloud applications and infrastructure.
- **Security Management:** Managing permissions, encryption, and identity access control.
- **Automation:** Automating tasks like backups, scaling, or deployment using scripts or tools.


#### **Examples:**
- AWS Management Console (for Amazon Web Services)
- Microsoft Azure Portal
- Google Cloud Console
- VMware vRealize for hybrid cloud management  






---

### **2. Cluster Manager**

 A **Cluster Manager** is software responsible for coordinating and managing a **cluster**—a group of interconnected computers or nodes that work together as a single system to provide higher availability, performance, and scalability.

 Each Cluster Manager is responsible for the operation of a collection of computers that are connected via high speed local area networks
  `Cluster Manager receives resource allocation commands and queries from the Cloud Manager`, and calculates whether part or all of a
command can be satisfied using the resources of the computers in the cluster.
Cluster Manager queries the Computer Managers for the computers in the cluster to determine resource availability, and returns messages to the Cloud Manager



#### **Key Functions:**
- **Resource Allocation:** Assigning resources (like CPU, memory, storage) to applications running on the cluster.
- **Job Scheduling:** Distributing workloads across the nodes to ensure efficiency and balance.
- **Fault Tolerance:** Detecting and managing node failures to maintain the cluster’s availability.
- **Scaling:** Adding or removing nodes dynamically based on workload requirements.
  
#### **Examples:**
- **Kubernetes:** Manages clusters of containers.
- **Apache Mesos:** Schedules tasks across large-scale clusters.
- **Hadoop YARN:** Manages clusters for big data applications.
- **SLURM:** Used for scheduling tasks in high-performance computing (HPC) clusters.






---

### **3. Computer Manager**  

A **Computer Manager** refers to a more general role, tool, or software responsible for managing individual computers or systems. This term is usually used in the context of system administration or IT management.


At the lowest level in the hierarchy computer manger runs on each computer system and uses the concept of virtualization to provide Virtual Machines to subscribers
Computer Manger maintains status information including how many virtual machines are running and how many can still be started
Computer Manager uses the command interface of its hypervisor to start, stop, suspend, and reconfigure virtual machines

#### **Examples:**
- Microsoft System Center Configuration Manager (SCCM)
- Remote Desktop Management Tools
- Linux-based system management utilities (e.g., `top`, `htop`)





### **Conclusion**

Each of these managers serves a distinct purpose within IT infrastructure. **Cloud Managers** are concerned with cloud resources, **Cluster Managers** focus on coordinating multiple nodes to work together, and **Computer Managers** deal with individual machine operations. Understanding these tools helps organizations choose the right technology to fit their operational needs, whether they’re working with cloud platforms, distributed systems, or local devices.










# Data Object Storage (DOS)

• DOS generally stores the subscriber's metadata like user credentials,
operating system images.
•DOS service is (usually) single for a cloud.
