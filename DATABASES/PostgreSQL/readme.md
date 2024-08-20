# PostgreSQL using docker

## Navigate to the PostgreSQL Directory

```sh
    cd PostgreSQL
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

## Access the PostgreSQL shell

```sh
    psql -U shreyash -d DB
```

## Stop and remove the running container

```sh
    docker compose down
```
