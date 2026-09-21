# Laboratory 04 – Cloud-Native Engineer

## Mission Overview

This laboratory focuses on cloud-native technologies, particularly virtualization and containerization. The activity introduces the differences between Virtual Machines and containers and provides hands-on experience deploying and managing a Docker container. An Nginx web server is deployed using Docker to demonstrate how containers can simplify application deployment.

## Objectives

* Understand the differences between Virtual Machines and containers.
* Learn how Docker containers work.
* Verify that Docker is installed and running.
* Pull and run an official Nginx Docker image.
* Understand Docker port mapping.
* Practice managing the container lifecycle.
* Document cloud-native activities in a GitHub portfolio.

## Docker Commands Executed

### Docker Environment

```bash
docker --version
docker info
```

### Download Nginx

```bash
docker pull nginx
```

### Run Nginx

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

### Test Nginx

```bash
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

Through this laboratory, I learned how containers differ from traditional Virtual Machines and why containers are useful in cloud-native environments. I learned how to pull Docker images, create and run containers, map ports, test a web server, and manage the container lifecycle. I also practiced documenting technical activities and organizing project files in a GitHub repository.

## Challenges Encountered

One challenge was understanding the difference between a Docker image and a running container. Another challenge was understanding port mapping and how port 8080 on the host connects to port 80 inside the Nginx container. Managing the container lifecycle also required careful attention because a stopped container still exists until it is removed using `docker rm`.

