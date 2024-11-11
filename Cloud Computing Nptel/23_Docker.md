**Docker Overview**

- **Docker** is a container management service (initial release: March 2013).
- **Main Features**: Develop, ship, and run anywhere.
- **Purpose**: Facilitates developers in developing applications, packaging them in containers, and deploying them universally.
- **Popularity**: Widely used in modern development, especially in Agile projects.

---

**Docker Components**

- **Docker for Mac**: Runs Docker containers on Mac OS.
- **Docker for Linux**: Runs Docker containers on Linux OS.
- **Docker for Windows**: Runs Docker containers on Windows OS.
- **Docker Engine**: Builds Docker images and creates Docker containers.
- **Docker Hub**: A registry for hosting Docker images.
- **Docker Compose**: Defines applications with multiple Docker containers.


---

**Docker Architecture**

- **Server**: The physical server hosting multiple virtual machines.
- **Host OS**: The underlying operating system, such as Linux or Windows.
- **Docker Engine**: Runs the OS, which now runs Docker containers instead of traditional virtual machines.
- **Applications**: All applications are run as Docker containers.


**Terminology - Image**

- *Persisted snapshot* that can be run.
- **images**: List all local images.
- **run**: Create a container from an image and execute a command in it.
- **tag**: Tag an image.
- **pull**: Download an image from a repository.
- **rmi**: Delete a local image (removes intermediate images if no longer used).

---


**Terminology - Container**

- *Runnable instance* of an image.
- **ps**: List all running containers.
- **ps -a**: List all containers (including stopped ones).
- **top**: Display processes within a container.
- **start**: Start a stopped container.
- **stop**: Stop a running container.
- **pause**: Pause all processes within a container.
- **rm**: Delete a container.
- **commit**: Create an image from a container container.



`Solution::Container is a run time instance of an image.`