# Service Level Agrement

- A formal contract between a Service Provider (SP) and a Service Consumer
- **SLA**: foundation of the consumer's trust in the provider
- **Purpose** : to define a formal basis for performance and availability the SP guarantees to deliver
- SLA contains Service Level Objectives (SLOs)
  . Objectively measurable conditions for the service
  . SLA & SLO: basis of selection of cloud provider




#  a simple breakdown of **Web Service SLA** and the differences between **Cloud SLA** and **Web Service SLA**:

### **Web Service SLA**

- **Definition**: A Web Service SLA is an agreement that outlines the expected performance and quality levels for a specific web service provided to clients.
  
- **Key Features**:
  - **Service Availability**: Specifies uptime guarantees (e.g., 99.9% availability).
  - **Response Times**: Details expected response times for requests.
  - **Support Levels**: Outlines support availability and response times for issues.
  - **Penalties**: Defines penalties for not meeting agreed performance metrics (e.g., service credits).

### **Cloud SLA vs. Web Service SLA**

| Aspect                | Cloud SLA                                          | Web Service SLA                                   |
|-----------------------|---------------------------------------------------|---------------------------------------------------|
| **Scope**             | Covers a broad range of cloud services (IaaS, PaaS, SaaS) | Focuses specifically on the performance of individual web services. |
| **Services Included** | May include infrastructure, storage, and applications hosted in the cloud | Pertains to APIs and services that enable communication over the web. |
| **Performance Metrics**| May include metrics related to overall cloud platform performance (e.g., compute resources, storage availability) | Specifically focuses on service-related metrics (e.g., API response time, service uptime) |
| **Complexity**        | Generally more complex due to the variety of services offered | More straightforward, focusing on specific service performance. |
| **Customization**     | Often includes customizable service levels based on user needs | Typically predefined, but may have some flexibility for specific services. |

### **Conclusion**

- **Web Service SLA**  focuses on the specific performance and reliability of web services, ensuring clients know what to expect. 
- **Cloud SLA**, on the other hand, encompasses a wider range of services within a cloud environment, addressing overall cloud service performance and resource management.

This simple comparison can help clarify the differences between these two types of service agreements!



**QoS Parameters** :
- Traditional Web Service : response time, SIA violation rate for reliability, availability, cost Of service. etc.
- Cloud computing : QoS related to security. privacy, trust. management, etc.
**Automation** :
- Traditional Web Service : SLA negotiation, provisioning. service delivery, monitoring are not automated.
- Cloud computing : SLA automation is required for highly dynamic and scalable service consumption
**Resource Allocation** :
- Traditional Web Service : UDDt (Universal Description Discovery ond Integration) for advertising and discovering between web services
- Cloud computing : resources are allocated and distributed globally without any central  directory













 a simplified explanation of **Service Level Objectives (SLOs)** and **Key Performance Indicators (KPIs)**:

### **Service Level Objectives (SLOs)**

**Definition**: SLOs are specific targets set by a service provider to measure the expected level of service. They help ensure that a service meets certain performance standards.

**Examples**:
- **Availability**: 99.9% uptime for the service each month.
- **Response Time**: 95% of requests should be answered in under 200 milliseconds.
- **Throughput**: The system should handle at least 1000 transactions per second.

### **Key Performance Indicators (KPIs)**

**Definition**: KPIs are measurable values that show how effectively a company is achieving its key business objectives. They provide insights into overall performance.

low- level resource metrics
Multiple KPIs are composed, aggregated, or converted to for high-level SLOs.
Example :
— downtime, uptime, inbytes, outbytes, packet size, etc.
Possible mapping : `Availability (A)= 1 — (downtime/uptime)`

**Examples**:
- **Customer Satisfaction Score (CSAT)**: Measures how happy customers are with a service.
- **Net Promoter Score (NPS)**: Gauges customer loyalty and likelihood of recommending the service.
- **Throughput**: Measures the total number of transactions processed over a specific time frame.

In summary, SLOs focus on specific service performance targets, while KPIs assess broader business performance.



# KPI -> SLO ->SLA
