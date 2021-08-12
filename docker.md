## Intro

This cheatsheet for docker provides some common docker commands, plus links to various online resources.   

### Docs
https://docs.docker.com/

### Install
https://docs.docker.com/get-docker/

### Help
```docker help```

## Working with containers

### Launch a new container and run a command 
```docker container run --rm busybox:latest /bin/echo "Hello World"```

or

```docker run --rm busybox:latest /bin/echo "Hello World"```


```--rm``` option removes container automatically when it exits

### Launch a new container and run an interactive shell 
```docker container run -it --rm busybox:latest```

or 

```docker run -it --rm busybox:latest```

```-i``` interactive (adds a stdin stream)
```-t``` Allocate a psuedo tty (adds a terminal driver allowing interaction)

### List all containers
```docker container ls -a```

or

```docker ps -a```

```-a``` list all containers (default is to list only running containers)

### Stop a container
```docker container stop {container id / name}```

or 

```docker stop {container id / name}```

### Start a container
```docker container start {container id / name}```

or 

```docker start {container id / name}```

### Remove a container
```docker container rm {container id / name}```

or 

```docker rm {container_id / name}```


## Working with images

### List images
```docker image ls```

or

```docker images```

### Pull an image from a registry
```docker image pull busybox:latest```

or

```docker pull busybox:latest```



## Working with registries

Docker Hub - https://hub.docker.com
Amazon Elastic Container Registry - https://aws.amazon.com/ecr/

