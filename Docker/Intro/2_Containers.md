**Hypervisor** is used to create multiple machines on a host operating system and
it manages virtual machines. These virtual machines have their own operating
system and do not use the host's operating system. They have some space

**Containers** in Docker are lightweight, standalone, and executable software packages that include everything needed to run a piece of software, such as code, runtime, system tools, libraries, and settings. They are based on Docker images and provide a consistent environment across different stages of development and deployment. Containers are isolated from each other and the host system, making them portable and easy to manage.

**Containerization** is the process of packaging an application and its dependencies into a container. This approach ensures that the application runs consistently across different computing


**Containers** are lightweight, portable units that package an application along with its dependencies, ensuring it runs consistently across different environments.

**Virtual Machines (VMs)** are isolated environments that run an entire operating system along with the application and its dependencies.

## Comparison:

Resource Usage: Containers share the host OS kernel and are more efficient, while VMs include a full OS and are heavier on resources.
Isolation: Containers offer process-level isolation, while VMs provide full OS-level isolation.
Start up Time: Containers start up quickly, often in seconds, while VMs can take minutes due to the need to boot up the entire OS.
Portability: Containers are more portable because they encapsulate only the application and its dependencies, whereas VMs package an entire OS and can be less portable.


## **Note:**:
 *containers* typically run on top of virtual machines (VMs) in many environments, especially in cloud and data centre setups. Here's how they relate:

Containers: Operate on top of a host OS (or sometimes directly on VMs), sharing the OS kernel while providing process-level isolation.

VMs: Provide full OS-level isolation and can host multiple containers. VMs include their own OS, which allows running different OS versions and configurations on the same physical hardware.


## When we say that containers typically run on top of virtual machines (VMs), it means:

- VMs as Hosts: Containers are often deployed within VMs. Each VM runs its own operating system and provides an environment where containers can be executed.

- Layered Architecture: In this setup, you have a layered architecture:

Physical Host: The actual hardware.
Hypervisor: Software that creates and manages VMs.
VMs: Each VM runs its own Guest OS.
Containers: Within each VM, containers run and share the VM's OS kernel but are isolated from each other.

- Resource Management: VMs manage resources and provide isolation, while containers offer lightweight, efficient application environments within those VMs.