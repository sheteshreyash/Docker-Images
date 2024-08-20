# MySQL using docker

## Navigate to the MySQL Directory

```sh
    cd MySQL
```

## Start the Docker Service (if not already running)

```sh
    sudo systemctl start docker
```

## start the docker container

```sh
docker compose up -d
```

## check the running containers

```sh
    sudo docker ps
```

## Get shell access to the container

(replace cont_id with the actual container ID)

```sh
    sudo docker exec -it cont_id bash
```

## Access the MySQL shell

```sh
    mysql -u root -p
```

## exit from MySQL command shell

```sh
    exit
```

## to stop and remove the running container

```sh
docker stop cont_id
docker rm cont_id
```

## Down

```sh
    docker compose down
```
