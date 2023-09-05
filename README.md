# Docker

| Feature  | Option Code |
| :------------- | :------------- |
|Check whether docker is already installed|`docker info`|
|Building docker container in the current folder|`docker build .`|
|Building docker container with a tag name 'mosaic-docker' [example](https://github.com/ide3a/mosaic#2-build-docker-image)|`docker build . -t mosaic-docker`|
|Check docker images already was built in local machine|`docker images`|
|Check the container is running|`docker ps`|
|Remove an image on local machine, 123456: docker image id, NOTE: If there is runnning container, you need to stop them|`docker image rm 123456`|
|Get docker image information|`docker image ls`|
|Get only docker image ids|`docker image ls -q`|
|Execute a docker container, -d:Run container in background and print container ID ,-p:Publish a container's port(s) to the host, 80:80:expose on the port, 6a75..:image id|`docker run -d -p 80:80 6a7576ddd211`|
|Or alternatively to execute -v:Bind mount a volume, --rm:Automatically remove the container when it exits, |`docker run -v %cd%:/home/mosaic/mosaic --rm -it mosaic-docker`|
|Run docker-compose.yml file, -d is detach mode|`docker-compose up -d`|
|Run docker-compose.yml file by forcing rebuild, -d is detach mode|`docker-compose up -d --build`|
|Connect a running container named flcav|`docker exec -it flcav bash`|


| Feature  | Option Code |
| :------------- | :------------- |
|Start a run container with the names|`docker start ContainerName`|
|Stop a run container with the names or IDS|`docker stop ContainerName`|
|Remove container with names or IDs|`docker stop ContainerName`|
|Remove build cache by force|`docker builder prune -f`|
