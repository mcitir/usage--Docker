# Docker

| Feature  | Option Code |
| :------------- | :------------- |
|Check whether docker is already installed|`docker info`|
|Building docker container in the current folder|`docker build .`|
|Building docker container with a tag name 'mosaic-docker' [example](https://github.com/ide3a/mosaic#2-build-docker-image)|`docker build . -t mosaic-docker`|
|Check docker images already was built|`docker images`|
|Execute a docker container, -d:Run container in background and print container ID ,-p:Publish a container's port(s) to the host, 80:80:expose on the port, 6a75..:image id|'docker run -d -p 80:80 6a7576ddd211'|
|Or alternatively to execute -v:Bind mount a volume, --rm:Automatically remove the container when it exits, |`docker run -v %cd%:/home/mosaic/mosaic --rm -it mosaic-docker`|
|Check the container is running|`docker ps`|
