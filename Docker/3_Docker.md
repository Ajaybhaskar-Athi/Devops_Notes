# What is Docker?

Docker is a container platform that allows you to build, test and deploy applications quickly.
A developer defines all the applications and it's dependencies in a Docker file which is then used to build Docker images that defines a Docker container.
Doing this ensures that your application will run in any environment.

# Why use Docker?

- Using Docker can help you ship your code faster, gives you control over your applications. You can deploy applications on containers that make it easier for them to be deployed, scaled, perform rollbacks and identify issues.

- It also helps in saving money by utilizing resources. Docker-based applications can be seamlessly moved
  from local development machines to production deployments.
- You can use Docker for Microservices, Data Processing, Continuous Integration and Delivery, Containers as a Service.

# **Kubernetes** : (often abbreviated as K8s) is an open-source platform designed to automate the deployment, scaling, and management of containerized applications. Developed by Google and now maintained by the Cloud Native Computing Foundation (CNCF), Kubernetes helps manage clusters of containers at scale across multiple hosts.

# Why Use Kubernetes?

Kubernetes is widely used to manage containerized applications because it simplifies the complex tasks of scaling, networking, and deployment, making it an ideal solution for running cloud-native applications and managing microservices architectures. It’s platform-agnostic and can run on any infrastructure, from on-premises data centres to public clouds.

**The Docker runtime** is the software component responsible for running containers in Docker. It provides the low-level functionality needed to create, start, manage, and stop containers.
The runtime acts as an intermediary between the Docker Engine (which provides higher-level container management functions) and the underlying operating system, enabling the execution of containerized applications.

# Types of Docker Runtime :

1. Default Runtime (runc): The standard runtime for Docker, compliant with the OCI specification, and responsible for creating and running containers. It is lightweight and provides the core functionality for container execution.
2. Containerd : 
containerd is designed to handle the lifecycle of containers, including pulling container images, managing storage, networking, and running containers.
