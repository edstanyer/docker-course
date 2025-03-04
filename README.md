# Docker Course

## Part 1
Simple Alpine Httpd image with Apache showing a webpage.

## Commands


## Images

Get a list od docker images

`docker` `images`

## Containers

List running containers

`docker` `ps` 

List all containers

`docker` `ps` `-a`



## Build
<p>Build the docker image: </p>

`docker` `build` `-t` *image-name* `:` *version* **source_path**

Example:  
> docker build -t my-docker-image:1.0.0 **.**

## Run

Build & run the container:</p>

`docker` `run` `--name` *container-name* `-p` *external port*`:` *internal port* *image-name* `:` *version*

Example:
> docker run --name my-docker-container -p 5150:80 my-docker-image:1.0.0 


## Start, Stop, Restart
<p>Restart an existing docker container</p>

`docker` `stop` / `start` / `restart`  *container-name* or *container-id*

## Piping

<p>Chain commands together</p>

List all ids of containers.

`docker` `ps` `-a` `-q` 

Example usage

Stop all containers:

`docker` `stop` $(`docker` `ps` `-a` `-q`)




## Exec

`docker` `exec` `-it` *my-docker-container* `sh`

See: [docker container execs](https://docs.docker.com/reference/cli/docker/container/exec/)



