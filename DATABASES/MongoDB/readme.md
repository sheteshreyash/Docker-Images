# MongoDB using docker

## to start the docker service

```sh
   sudo systemctl start docker
```   

2. to start docker container
   docker compose up -d

3. to stop the docker container
   docker compose down

4. see the running containers
   sudo docker ps

5. to get the shell access
   sudo docker exec -it cont_id bash

6. access the mongodb shell with authentication
   mongosh --username root --password abc123

7. Connect to the mongo database from mongodb compass using below link (it uses shrey database)
   mongodb://root:abc123@localhost:27017/shrey?authSource=admin

8. Check the container status and Verify that the application can reach the MongoDB container:
   docker inspect cont_id
   (Look for the IP address and ensure that your application is attempting to connect to the correct address and port)

9. Check the MongoDB logs within the container for any authentication-related issues:
   docker logs cont_id

10. exit fromm mongo shell
    exit
