# MongoDB using docker

## to start the docker service

```sh
   sudo systemctl start docker
```

## to start docker container

```sh
   docker compose up -d
```

## to stop the docker container

```sh
   docker compose down
```

## see the running containers

```sh
   sudo docker ps
```

## to get the shell access

```sh
   sudo docker exec -it cont_id bash
```

## access the mongodb shell with authentication

```sh
   mongosh --username root --password abc123
```

## Connect to the mongo database from mongodb compass using below link (it uses local shrey database)

```sh
   mongodb://root:abc123@localhost:27017/shrey?authSource=admin
```

## Check the container status and Verify that the application can reach the MongoDB container

(Look for the IP address and ensure that your application is attempting to connect to the correct address and port)

```sh
   docker inspect cont_id
```

## Check the MongoDB logs within the container for any authentication-related issues

```sh
   docker logs cont_id
```

## exit fromm mongo shell

```sh
    exit
```
