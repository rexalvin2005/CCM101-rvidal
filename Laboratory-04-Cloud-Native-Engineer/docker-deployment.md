# Docker Deployment

## Docker Commands

### 1. List Running Containers

```bash
docker ps
```

This command lists all Docker containers that are currently running.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container without removing it.

### 3. Verify the Container is Stopped

```bash
docker ps
```

This command verifies whether the Nginx container is still running.

```bash
docker ps -a
```

This command displays both running and stopped containers.

### 4. Remove the Container

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container completely from the Docker environment.

## Nginx Deployment

The Nginx image was downloaded using:

```bash
docker pull nginx
```

The Nginx container was started using:

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

The web server was tested using:

```bash
curl http://localhost:8080
```

The port mapping `8080:80` allowed requests sent to port 8080 on the host to reach port 80 inside the Nginx container.
