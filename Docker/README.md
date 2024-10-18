# Devops
Dcoker Engine:  It comprises two main components - Docker Daemon (dockerd) & Docker Client  
Docker Images:  Docker images are created from Dockerfiles, which are text files containing instructions for building the image layer by layer.  
Docker Containers:   
Docker Registry: Docker Registry is a centralized repository for storing and sharing Docker images. The default public registry is Docker Hub, where users can find a vast collection of images. 
## Docker Compose:  
 Dockerfile  Only defines how to build a single container , while Docker Compose Defines how to run multiple containers together, including the configurations and interactions between them.
Centralized Configuration:

Dockerfile: Focuses on one container at a time.
Docker Compose: Centralizes all configurations for multiple services, making it easier to manage complex environments.
Networking and Links Simplified:

Dockerfile: You would have to manually set up networking between containers.
Docker Compose: Automatically sets up a network where services can communicate by their names (e.g., a web service can connect to db without IP addresses).
Automated Orchestration:

Dockerfile: You would need to run commands like docker run or docker network for each container and manage them separately.
Docker Compose: Automatically brings up all services, sets up networking, and handles dependencies between services with just one command (docker-compose up).
Multi-Stage Environment Support:

Docker Compose: Offers different profiles for running the application in different environments (e.g., development vs production) with the same file or minimal changes.
Simplified Data Persistence:

Docker Compose: Easily defines shared volumes for data persistence across containers, which can be cumbersome to manage manually with docker run commands.

