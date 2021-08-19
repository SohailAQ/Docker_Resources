# Docker Resources

### Dockerfile usage

To check the dockerfile, just copy the dockerfile without docker-compose and travis and execute

```docker build -t docker_id/crud .```

> Replace ```docker_id``` with your own docker_id.

> Do not forget trailing period.

To check if the files are copied to the correct folder and all the requirements are installed execute

```docker ps```
> Copy the container_id

```docker exec -it container_id sh```

The ```sh``` starts your container with working_directory.