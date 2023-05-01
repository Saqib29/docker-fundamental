# Docker Fundamentals

Cheat sheet for the fundamental Docker commands:

## Commands:

1. **Build**: This command is used to build an image from a Dockerfile.
   - `docker build -t <image_name> .`
   - `docker build -t <image_name>:<version_name> .`

2. **Run**: This command is used to run a container from an image.
   - `docker run --name <container_name> <image_name>`
   - `docker run --name <container_name> -p 8000:4000 -d <image_name>:<version_name>`
   - `docker run --name <container_name> -p 4000:4000 -d <image_name>`
   - `docker run --name <container_name> -p 4000:4000 --rm <image_name>:<version_name>`
   - `docker run --name <container_name> -p 7000:4000 --rm -v <path>:<container_path> -v <container_path_specific> <image_name>:<version_name>`

3. **Stop and Start**: These commands are used to stop and start containers.
   - `docker stop <container_name>`
   - `docker start <container_name>`

4. **Images and Containers**: These commands are used to list images and containers.
   - `docker images`
   - `docker ps`
   - `docker ps -a`

5. **Remove**: These commands are used to remove images and containers.
   - `docker image rm <image_name>`
   - `docker image rm <image_name>:<version_name>`
   - `docker image rm <image_name> -f`
   - `docker container rm <container_name>`

6. **Clean up**: This command is used to remove all unused data.
   - `docker system prune`
   - `docker system prune -a`

7. **Compose**: These commands are used to manage Docker Compose.
   - `docker-compose down`
   - `docker-compose down --rmi all -v`