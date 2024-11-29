# Essential Docker Commands

## Basic Docker Commands

- **Check Docker Version**  
  `docker --version`

- **List Docker Commands**  
  `docker`

- **Display Docker System Information**  
  `docker info`

- **Check Running Docker Containers**  
  `docker ps`

- **List All Docker Containers (Including Stopped)**  
  `docker ps -a`

## Managing Containers

- **Run a Container**  
  `docker run <options> <image>`

  Example: `docker run -it ubuntu bash`

- <span style="color:green">**Start a Container**</sapn>  
  `docker start <container_id_or_name>`

- <span style="color:yellow">**Stop a Running Container**</span>  
  `docker stop <container_id_or_name>`

- **Restart a Container**  
  `docker restart <container_id_or_name>`

- <span style="color:red">**Remove a Stopped Container**</span>  
  `docker rm <container_id_or_name>`

- **View Container Logs**  
  `docker logs <container_id_or_name>`

- **Execute a Command in a Running Container**  
  `docker exec -it <container_id_or_name> <command>`

  Example: `docker exec -it <container_id> bash`

## Images and Repositories

- **List Docker Images**  
  `docker images`

- **Pull an Image from Docker Hub**  
  `docker pull <image_name>`

- **Build an Image from a Dockerfile**  
  `docker build -t <image_name> <path>`

- <span style="color:red">**Remove an Image**</span>  
  `docker rmi <image_id_or_name>`

- **Tag an Image**  
  `docker tag <source_image> <target_image>`

- **Push an Image to Docker Hub**  
  `docker push <repository>/<image_name>`

## Docker Networking

- **List Docker Networks**  
  `docker network ls`

- **Create a New Network**  
  `docker network create <network_name>`

- **Connect a Container to a Network**  
  `docker network connect <network_name> <container_name>`

- **Disconnect a Container from a Network**  
  `docker network disconnect <network_name> <container_name>`

## Docker Volumes

- **List Volumes**  
  `docker volume ls`

- **Create a Volume**  
  `docker volume create <volume_name>`

- <span style="color:red">**Remove a Volume**</span>  
  `docker volume rm <volume_name>`

- **Inspect a Volume**  
  `docker volume inspect <volume_name>`

- **Use a Volume with a Container**  
  `docker run -v <volume_name>:/path/in/container <image>`
"""

