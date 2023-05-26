# Docker

## Basics

```bash
docker
```

## Docker version

```bash
docker --version
```

## Pull image

```bash
docker pull image
```

## Remove image

```bash
docker rmi image
```

## List images

```bash
docker images
```

## Run container from image

```bash
docker run image:tag
```

## Run container from image in detached mode

```bash
docker run -d image:tag
```

## Run container with name

```bash
docker run --name container_name image:tag
```

## Stop container

```bash
docker stop container_id
```

## Start container

```bash
docker start container_id
```

## Remove container

```bash
docker rm container_id
```

## Remove all containers

```bash
docker rm $(docker ps -aq)
```

## Force remove container

```bash
docker rm -f container_id
```

## Force remove all containers

```bash
docker rm -f $(docker ps -aq)
```

## List running containers

```bash
docker ps
```

## List all containers

```bash
docker ps -a
```

## List with format

```bash
docker ps --format="ID\t{{.ID}}\nNAME\t{{.Names}}\nImage\t{{.Image}}\nPORTS\t{{.Ports}}\nCOMMAND\t{{.Command}}\nCREATED\t{{.CreatedAt}}\nSTATUS\t{{.Status}}\n"
```

## Expose port in detached mode

```bash
docker run -d -p host_port:container_port image:tag
```

## Expose multiple ports in detached mode

```bash
docker run -d -p host_port:container_port -p host_port:container_port image:tag
```

## Volumes

### Mount present working directory inside container

mode: ro (read only), rw (read write).

```bash
docker run -d -p host_port:container_port --name container_name -v $(pwd):container_folder:mode image:tag
```

### Share volumes between containers

```bash
docker run -d -p host_port:container_port --name container_name --volumes-from container_name image:tag
```

## Enter container

```bash
docker exec -it container_id bash
```
