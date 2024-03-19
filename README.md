#Basic commands of docker

1.  docker run <image name> [ubuntu,linux,redhat] -> it pull + build + create container // it create your docker container
    e.g.    docker run ubuntu -> to run ubuntu
            (using this command your terminal goes into the foregorund state, your unable to run commands)

2.  docker run -d <image name> -> run your image  in detached mode (your image runs in background)

3.  docker ps -> it shows your running containers

4.  docker ps -a -> it shows your all containers (exited running)

5.  docker ps -q -> it shows running containers id

6.  docker ps -qa -> it shows all containers id (exited running)

7.  docker run --name <name you want to set> <image name> -> it gives name to your container while  running 
    e.g.    docker run --name shashank httpd

8.  docker image -> it shows container image

9.  docker rename <container name> <container id> -> rename to container (to rename exiting container)
    e.g.    docker rename b24 809

10. ps -elf | grep "docker" -> all info.

11. docker start <container id> -> to start container

12. docker rm <container id> -> to remove container

13. docker stop <container id> -> to stop container

14. docker run -d <image> -> to run in background

15. if config -> docker network 

16. docker inspect <container id> -> container info

17. docker exec -it <image_id/container_id> /bin/bash -> get access during container is running

18. docker run -d -P <image> -> random port number assign to the container while creating container

19. docker run -d -p <port no.> <container id> <image> -> attaching port number to the container after creating the container
