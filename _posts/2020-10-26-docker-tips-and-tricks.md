---
title: Docker Tips and Tricks
tags: [Docker, Software Development]
style: fill
color: dark
description: Some tips and tricks about Docker.
---

The purpose of this blog post is to collect the commands that I use the most on a daily basis. Besides
some advice and/or trick to improve the operation of Docker.

## Tricks

### .dockerignore

Before the docker CLI sends the context to the docker daemon, it looks for a file named `.dockerignore`
in the root directory of the context. If this file exists, the CLI modifies the context to exclude files
and directories that match patterns in it.

### Example for Python

```
_env
.git
```

### Example for React

```
node_modules
deploy
build
.git
```

[Docker Documentation about .dockerignore](https://docs.docker.com/engine/reference/builder/#dockerignore-file)

## CLI related

### Stop all containers

`docker stop $(docker ps -a -q);`

### Remove all containers

`docker rm $(docker ps -a -q);`

### Remove all images

`docker rmi $(docker images -q);`

## Shell-alias related

### Get container process

`alias dps="docker ps"`

### Get container IP

{% raw %}
`alias dip="docker inspect --format '{{ .NetworkSettings.IPAddress }}'"`
{% endraw %}

### Stop all containers

`dst() { docker stop $(docker ps -a -q); }`

### Remove all containers

`drm() { docker rm $(docker ps -a -q); }`

### Remove all images

`dri() { docker rmi $(docker images -q); }`

### Log a container

Should pass the name, e.g.: _dlog container_1_

`alias dlog="docker logs $1"`

### Log and follow a container

Should pass the name, e.g.: _dlogf container_1_

`alias dlogf="docker logs -f $1"`

### Sh into running container

Should pass the name, e.g.: _dsh container_1_

`dsh() { docker exec -it $(docker ps -aqf "name=$1") sh; }`

### Bash into running container

Should pass the name, e.g.: _dbash container_1_

`dbash() { docker exec -it $(docker ps -aqf "name=$1") bash; }`

## Troubleshooting

### UnixHTTPConnectionPool(host='localhost', port=None): Read timed out. (read timeout=60)

[Original answer](https://github.com/docker/compose/issues/3927)
```
export DOCKER_CLIENT_TIMEOUT=120
export COMPOSE_HTTP_TIMEOUT=120
```

Source: [Github - LaQuay / docker-utils](https://github.com/LaQuay/docker-utils)
