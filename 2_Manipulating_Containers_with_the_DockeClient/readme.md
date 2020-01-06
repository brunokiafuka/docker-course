# Docker client

### Create and running container from an image

> docker run = docker create + docker start. Docker run combines two commands to create and start the container. We can create a container without having to start it.

`docker run <image name>`

#### Default commands

We can override the default run command by passing an extra command:

`docker run <image name> command!`

### Docker list containers

`docker ps` - We use it to see running containers.

`docker ps --all` - shows all the containers that ever being created on our machine.

### Docker create & start

`docker create <image name>` - returns id of the container.

`docker start -a <container id>` - `-a` attach to container and append to terminal. If we don't use `-a` it will not return the container logs.

### Removing stopped containers

`docker system prune`

### Docker logs

`docker logs <container id>`

### Docker stop container

`docker stop <container id>` or `docker kill <container id>`

### Running multi-commands containers

`docker exec -it <container id> <command>` - the `-it` flag allow us to add an input.

### Execute shell

`docker exec -it <container id> sh`
