# OpenWebRX Docker Compose File
### Pre-requisite: docker & docker-compose installed on Linux
```
 curl -fsSL https://get.docker.com -o get-docker.sh

 sudo sh get-docker.sh
```
1. Clone this repo and cd into the folder
2. Create a ".env" file for use in the Docker Compose file
```
mv .env-sample .env
```

3. Update the admin username/password in the ".env" file
4. Run the docker compose file
  ```
  docker compose up -d
  ```
5. Naviagte to http://localhost:8073 (or the IP address of the server running the container)
