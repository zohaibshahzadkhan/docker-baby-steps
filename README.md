# docker-baby-steps
Whats is docker ?

Docker is an advance form of virtualization and it's job is to do containerization. Container is like a virtual machine where as docker is a tool helps creating these virtual machines. 

### Virtual Machine VS Docker Containers 
\
![VM VS Containers](images/VM%20vs%20Docker.png)

### Problems with virtualization
1. Once the resources are allocated to VM it will remain allocated to the VM.
i.e If a host machine has 16GB of RAM in total and you wish to create three different VM's  with the following resources. 
    - VM-1 (2GB RAM) 
    - VM-2 (6GB RAM)
    - VM-3 (8GB RAM)

    Onces VM-1 and VM-2 is created VM-3 can not be created ( despite of the fact either VM-1 or VM-2 is in running state or not ) as VM-3 need 8GB of RAM and there not enough memory is left. 

2. OS need to be installed on each VM with it self need space and resource 

### Advantages of Docker

1. No pre-allocation of RAM
2. Light weight
3. Less cost in terms of resources 
4. Reuse Images

### Disadvantage of Docker
Docker doest not provide cross-platform compatibility if an application is design to run in a docker container on windows than it can not run on linux docker container. 

### Image  vs Container

Container in stop state is refer to an Image however Image in running state is known as container.

### What is Docker Hub ?
Docker Hub is a hosted repository service provided by Docker for finding and sharing container images. Container pulls it's dependencies from docker hub.

### Docker Architecture  
\
![docker architecture](images/Docker%20Architecture.png)

### Docker Eco-system  
\
![docker eco-system](images/docker%20ecosystem.png)

1. **Docker Daemon**: Runs on Host OS and it is responsible for running containers.

2. **Docker Client**: Docker user can interact with docker daemon through client (it is a tool to communicate with docker daemon)
    Docker client uses CLI and REST API for communication to docker daemon
    
3. **Docker Hub**: It is a registry that manage and store docker images. There are two type of registries in docker.
    - Public Registry: also called docker hub (available to all)
    - Private Registry: It is used to share a registry with in an enterprise
    
4. **Docker Images**: Docker images are read only binary templates used to create docker containers. Different ways to create docker images
    - Take image from docker hub
    - Create image from docker file
    - Create image from existing running container
    
5. **Docker Images**: Docker container holds the entire package that is needed to run the application.

