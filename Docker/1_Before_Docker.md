


# **Before Docker**: 

 Before Docker, one major issue was that traditional server setups often involved running one application per server.
This setup had several implications:

1. # Dedicated Resources: 
A server was allocated to run just one application or service, which meant that the server's resources (CPU, memory, etc.) were used only for that application.

2. # Underutilization:
 If the application didn’t use all of the server’s resources, those resources were wasted. For example, if a server had 8 GB of RAM but the application only needed 2 GB, the remaining 6 GB of RAM wasn’t used efficiently.

3. # Deployment Challenges: 
Updating or deploying a new version of the application required either modifying the existing server or creating a new server. This process could be complex and resource-intensive.

4. # Isolation Issues: 
Running multiple applications on the same server without isolation could lead to conflicts between applications, especially if they had different dependencies or configurations. traditionally, each physical or virtual server was often dedicated to running a single application. 

**Note:** A code is work on our systems and doesn't work on our friends . There may be any installation problems or any dependencies problem which will be solved by docker



# ** Virtual Machines (VMs)**:

VMs helped address some of these issues by allowing multiple isolated environments on a single physical server. Each VM runs its own operating system and can host one or more applications. This approach provided:

- Isolation: Each VM is isolated from others, preventing conflicts between applications.
- Resource Efficiency: Better resource utilization compared to running a single application per server.
- Easier Deployment: VMs can be cloned or deployed to create new instances quickly.

 However, VMs have their own overhead because each VM includes a full operating system. This can lead to resource inefficiencies and longer boot times.




 ## What is a Server?
A server is a computer or software that provides services, resources, or data to other computers (clients) over a network. Servers can be physical machines or virtual environments.

1. **Physical Servers**
Example:

Server 1: A physical computer with its own CPU, RAM, disk storage, and network connections. It might be a dedicated machine in a data centre running a web server application.
Server 2: Another physical computer, similar to Server 1, but it might be running a database server or another type of service.

2. **Virtual Servers**
Virtual servers are created using virtualization technology and run on a single physical server. They share the physical server’s resources but operate as if they were separate, independent servers.

Example:

Physical Server:

CPU: 8 cores,RAM: 32 GB,Disk: 500 GB
On this physical server, you can create multiple virtual servers (VMs) using virtualization software (hypervisor).
- VM 1:
Operating System: Ubuntu Server
Resources Allocated: 4 CPU cores, 8 GB RAM, 100 GB disk
Purpose: Might be running a web server application.
-VM 2:
Operating System: Windows Server
Resources Allocated: 4 CPU cores, 8 GB RAM, 100 GB disk
Purpose: Might be running a database application.

*Characteristics*:

Isolation: Each VM is isolated from others, so applications running in VM 1 don’t affect those in VM 2.
Shared Resources: VMs share the physical server’s resources (CPU, RAM, disk) but are allocated specific portions.


## Summary
# Physical Servers: Standalone machines that run applications or services.(One application per physical server)
# Virtual Servers (VMs): Virtual instances created on a physical server, sharing its resources but operating independently.
(Multiple VMs can run on a single physical server, each with its own OS and isolated environment.)

# By using virtualization, you can maximize the use of physical hardware and run multiple applications or services efficiently on a single physical machine.

## But VMs need separate OS,separate hardware , for that we r having Docker which uses Containers 


**Docker Containers**: Multiple containers can run on a single host OS, sharing resources more efficiently and starting up quickly.