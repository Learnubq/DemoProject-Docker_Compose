## Demo Project - Running Multiple Docker Containers with Docker Compose

This demo shows the process of writing Docker Compose files to run multiple docker containers at once, without having to execute commands repeatedly for each container.

## Technologies Used
- Docker
- MongoDB
- MongoExpress

## Steps to Use Docker Compose to Run Multiple Docker Containers

1. **Saved the Docker Compose file in the Project Directory and Installed Docker Compose:**
```bash
mkdir -p ~/.docker/cli-plugins
curl -SL https://github.com/docker/compose/releases/latest/download/docker-compose-linux-$(uname -m) \
  -o ~/.docker/cli-plugins/docker-compose
chmod +x ~/.docker/cli-plugins/docker-compose
```

3. **Started the Docker Containers Using the Docker Compose File After Checking No Containers Were Running:**

```bash
cd ~/js-app/app
docker ps
docker compose --file docker_compose_mongo.yaml up
```

<img width="1858" height="186" alt="image" src="https://github.com/user-attachments/assets/15c1dfdb-26d0-4eac-9b1e-09ab64ba917d" />

4. **Checked the created docker network is working:**

```bash
docker network ls
```

<img width="994" height="81" alt="image" src="https://github.com/user-attachments/assets/e25f8e6b-b190-494f-a317-b6c00571d171" />

5. **Then checked that Docker containers were running:**

```bash
docker ps
```

<img width="1847" height="136" alt="image" src="https://github.com/user-attachments/assets/5c9d7a6d-5c98-4577-b037-3a467d0adc9a" />




