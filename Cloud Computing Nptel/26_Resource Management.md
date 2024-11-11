# Resource Management Approaches
• Architectures ‐ the architectures used for resource management in fog/edge computing are classified on the basis of data flow, control, and tenancy.
• Infrastructure ‐ The infrastructure for fog/edge computing provides facilities composed of hardware and software to manage the
computation, network, and storage resources for applications utilizing the fog/edge.
• Algorithms ‐ There are several underlying algorithms used to facilitate fog/edge computing.



### Architectures
Architectures in fog and edge computing vary based on:
  - **Data Flow**: Determines how data is transmitted between devices and the cloud, often in real-time or near-real-time to support applications like IoT.
  - **Control**: Can be centralized or decentralized, impacting how decisions are made and resources managed across the network.
  - **Tenancy**: Refers to the sharing of resources between multiple tenants (single or multi-tenant models), affecting security, isolation, and resource allocation. 
   Tenancy is correctly described as the support for hosting multiple applications
or a single application on an edge node.

### Infrastructure
Infrastructure in fog and edge computing consists of:
  - **Hardware**: This includes devices such as routers, gateways, sensors, and edge servers to handle computing closer to the source of data.
  - **Software**: Middleware and frameworks that enable management, virtualization, and orchestration of resources (e.g., Kubernetes, OpenStack).
  - **Middleware**:Acts as a bridge between the hardware and applications, managing communication, data integration, and           interoperability across devices.
    Examples include data analytics platforms, cloud management tools, and IoT frameworks that handle resource orchestration and service provisioning.


### Algorithms
1. **Discovery**:
   - Algorithms that identify and connect edge devices and resources within the network, ensuring seamless device integration and communication.
   - Discovery algorithms are essential for dynamically adding or removing devices in a fog/edge environment.

2. **Benchmarking**:
   - Evaluates the performance of devices and resources in real-time, helping determine their suitability for specific tasks.
   - Benchmarking can involve measuring processing speed, latency, energy efficiency, and storage capacity to match workloads with available resources.

3. **Load Balancing**:
   - Distributes workloads across multiple devices or servers to avoid overloading any single resource, ensuring high availability and optimal resource utilization.
   - Load balancing algorithms in edge computing often consider network proximity, device capacity, and energy constraints to minimize latency.

4. **Placement**:
   - Determines the optimal location for deploying applications or tasks, whether on edge devices, local servers, or in the cloud.
   - Placement algorithms take into account factors like latency, bandwidth, and data security, ensuring that applications are positioned to meet performance and efficiency requirements.

Each of these elements within the **Infrastructure** and **Algorithms** categories is tailored to support the unique demands of fog and edge computing, enabling rapid, reliable, and efficient processing close to data sources.


• Algorithms used to facilitate fog/edge computing. Four major
algorithms.
• Discovery: identifying edge resources within the network that can be
used for distributed computation
• Benchmarking: capturing the performance of resources for decision‐
making to maximize the performance of deployments
• Load‐balancing: distributing workloads across resources based on
different criteria such as priorities, fairness etc.
• Placement: identifying resources appropriate for deploying a
workload.
