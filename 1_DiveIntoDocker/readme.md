# Docker

### Why do we use docker?

> Docker makes it easy to install and run softwares without having to worry about setups or dependencies.

### What is docker?

> Docker is a platform or ecosystem around creating and running containers.

### Docker ecosystem

- Docker Client (Docker cli): tool that we use to issue docker commands.
- Docker Server (Docker daemon): tools that is responsabilities for creating images, running containers, etc.
- Docker Machine
- Docker Images
- Docker Hub
- Docker Compose

### Important terminology

> **Image:** single file with all deps and configs required to run a specific program. **Container:** instance of an image (running program)

#### Container & Images

> Think a containers as set of processes that have a grouping of resources specifically assigned to it.

> An image is like a filesystem snapshot a long with the specific start up comand, consider to be a copy and paste of a directory containing files needed to run a container. When we run an image it copies the image to our OS container creating a namespace in order to run it.

### How does docker works

When we install docker we are installing a Linux VM and all the our containers are created in that Linux VM, it uses Linux Kernel to hust and running the processes giving access to the OS resources.

The linux kernel laverages the use of **Namespacing** and **Control groups** to alocate memory space and access to the OS in order to run the containers.
