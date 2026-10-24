# Laboratory 07 - Cloud Operations Engineer

## Mission Overview

This laboratory focuses on monitoring a Linux host and observing a containerized web server using Docker. It demonstrates how system resource checks, application logs, and container metrics help engineers maintain reliable services.

## Objectives

- Establish a baseline for host memory and disk usage.
- Deploy an Nginx web server container.
- Generate successful HTTP requests and a 404 response.
- Inspect application logs for troubleshooting.
- Monitor container CPU and memory consumption.

## Monitoring Commands Executed

- `free -h` - Check memory usage.
- `df -h /` - Check root filesystem storage.
- `top` - Observe CPU load and running processes.
- `docker run` - Deploy the Nginx container.
- `curl` - Generate HTTP requests.
- `docker logs` - Inspect application logs.
- `docker stats` - Monitor container resource usage.

## Skills Learned

- Linux system monitoring.
- Docker container deployment and management.
- HTTP request testing.
- Log analysis and troubleshooting.
- Container resource monitoring and observability.

## Screenshots

Screenshots of the system baseline, Nginx deployment, HTTP requests, logs, and container metrics are stored in the `screenshots/` directory.
