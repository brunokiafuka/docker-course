## Creating docker

> To create a custom container we need to have a DockerFile[image], which will house some configurations for our docker container.

After creating the docker file, we should pass it through the `docker cli` which will provide the file to the `docker server` in order to build a docker usable image.

#### Docker file config

Writing a docker file is equivalent to be given a new computer and be told to install specific programs.

- Specify a base image.
- Run commands to install additional programs.
- Speficy a command to run on container starup.

Example: Create an image that runs redis-server

`docker build .`

```
# Use an existing docker image as a base
FROM alpine

# Download and install dependency
RUN apk add --update redis

# Tell the image what to do when it starts a container
CMD [ "redis-server" ]

```

`[FROM | RUN | CMD]` - are instructions used to tell docker server what to do.

> A `base image` is basically a base OS the container will be using. The base image is a starting point for the image we are creating.

#### Tagging an image

`docker build -t bruno/redis:latest .`

**Convetion breakdown**

`-t bruno/redis:latest` == `dockerid/[repo|projectname]:version`
