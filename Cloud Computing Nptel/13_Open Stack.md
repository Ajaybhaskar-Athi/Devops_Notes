OpenStack is an open-source cloud computing platform that enables users to build and manage both public and private cloud environments. It provides infrastructure-as-a-service (IaaS), meaning it allows users to create and manage virtualized resources such as compute, storage, and networking through a web interface, command-line tools, or REST APIs.


OpenStack is modular, so each major functionality (like compute, networking, storage) is handled by a separate "project." Each project has its own codebase, documentation, and community that focuses on that area.
Ex: `The Compute Service functionality in OpenStack is fulfilled by the Nova project.`

### OpenStack Capabilities
OpenStack supports various cloud service models:
- **Software as a Service (SaaS)**: Offers applications via a browser or thin client.
- **Platform as a Service (PaaS)**: Allows platform services on top of infrastructure, such as Cloud Foundry.
- **Infrastructure as a Service (IaaS)**: Provides virtualized compute, storage, and network resources, allowing users to provision and manage them directly.

### Key Features
- **Virtual Machines (VMs)** on demand, enabling users to quickly access virtualized computing resources.
- **Provisioning**: Automates the setup of compute, network, and storage resources.
- **Snapshotting**: Allows capturing a VM's state for recovery or backup.
- **Network Management**: Manages virtual networks for seamless connectivity.
- **Multi-tenancy**: Enables secure isolation between different users and projects.
- **Quotas**: Sets limits for resources to ensure fair usage across projects and users.
- **User Association**: Users can work across multiple projects, offering flexibility.

### OpenStack Major Components

1. **Compute Services ,Ephemeral storage**  
   - **Project: Nova**
   - Manages the lifecycle of VMs, including starting, stopping, and scheduling them in an OpenStack environment.

2. **Networking Service**
   - **Project: Neutron**
   - Provides Network-Connectivity-as-a-Service, allowing users to define networks and manage connectivity.
   - Offers a pluggable architecture to integrate with different networking technologies.

3. **Object Storage Service**
   - **Project: Swift**
   - Manages and stores large amounts of unstructured data with replication across servers for high fault tolerance.
   - Accessible via a RESTful API and is scalable across a server cluster.

4. **Block Storage Service**
   - **Project: Cinder**
   - Provides persistent storage that can be attached to VMs, functioning like virtual hard drives.
   - Features a driver architecture that supports multiple storage backends.

5. **Identity Service**
   - **Project: Keystone**
   - Handles authentication, authorization, and access control across OpenStack services.
   - Offers a catalogue listing all available OpenStack services and their endpoints.

6. **Image Service**
   - **Project: Glance**
   - Stores and manages virtual machine disk images, which can be used when launching VMs.

7. **Telemetry Service**
   - **Project: Ceilometer**
   - Collects and monitors data on resource usage for billing, capacity planning, and performance analysis.
    - images. Ceilometer provides telemetry services, which allow the cloud to `provide billing services` to individual users of the cloud.
8. **Dashboard**
   - **Project: Horizon**
   - Provides a user-friendly web interface to manage OpenStack resources, such as launching VMs and configuring networks.

---

Each of these components works together to provide a comprehensive cloud management platform, allowing users to efficiently set up and manage scalable virtualized environments across large-scale data centres.


# Summary


▪ Users log into Horizon and initiates VM creation
▪ Keystone authorizes
▪ Nova initiates provisioning and saves state to DB
▪ Nova Scheduler finds appropriate host
▪ Neutron configures networking
▪ Cinder provides block device
▪ Image URI is looked up through Glance
▪ Image is retrieved via Swift
▪ VM is rendered by Hypervisor




`Ephemeral Storage` refers to temporary storage that is not persistent across reboots or failures. It is typically used for data that is only needed for the duration of a session or instance lifecycle, making it suitable for certain types of applications and workloads.

-Ephemeral storage is used to run operating system and/or scratch space
-In ephemeral storage, the stored objects persist until the VM is terminated.
-Ephemeral storage is managed by NOVA in OpenStack.