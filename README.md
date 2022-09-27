# Docker
Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. 

## Containers
A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

## Docker-commands
* List running container               :
 ```
 docker ps
 ```
* List all container even exited one   :
```
docker ps -a
```
* Stop Container use Id/conatiner name : 
```
docker stop container name/container Id
```
* List all docker Images               : 
```
docker images
```
* Remove docker images                 : 
```
docker rmi image-name
```
* Run Docker Image                     : 
```
docker run image-name
```
* Pull image from docker hub           : 
```
docker pull image-name
```
* Execute command in docker container  : 
```
docker exec image-name cat /etc/os-release
```
* Run image in detach mode             : 
```
docker run -d image-name
```
* Run image in attach mode             : 
```
docker attach id
```
* Run particular version of an image   : 
```
docker run image-name:tag
```
* Run image in interactive mode        : 
```
docker run -i image-name
```
* Remove container                     : 
```
docker rm container-id
```
* Volume mapping                       :
```
docker run -v /opt/backup_dir:/var/lib/jenkins jenkins
```
* Inspect container                    : 
```
docker inspect container-name
```
* Container logs                       : 
```
docker logs container-name
```

## Create your own image
- We can create our image using Dockerfile
- Define steps
- Build image docker build 
```
Dockerfile build -t docker_hub_username/application-name
```
- Push image  
```
docker push docker_hub_username/application-name 
```
