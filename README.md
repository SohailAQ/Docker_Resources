# Docker Resources

### Dockerfile usage

To check the dockerfile, just copy the dockerfile without docker-compose and travis and execute \
```docker build -t docker_id/crud .```

* Replace `docker_id` with your own docker_id.
* Do not forget trailing period.

To check if the files are copied to the correct folder and all the requirements are installed execute \

>```docker ps```

Copy the container_id and execute \
>```docker exec -it container_id sh```

The `sh` starts your container with working_directory.

### Docker-Compose usage

* Seperate CLI that gets installed with Docker.
* Used to startup multiple Docker containers at the same time.
* Automates some of the long-winded arguments being passed to 'docker run'

To run docker-compose execute
> ```docker-compose up```

To rebuild an existing container
> ```docker-compose up --build```

To launch a container in background
> ```docker-compose up -d```

To stop Container
> ```docker-compose down```

To check container Status with docker-compose navigate to the directory where docker-compose.yml file is located and run
> ```docker-compose ps```