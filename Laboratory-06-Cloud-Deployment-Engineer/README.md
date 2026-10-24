# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory demonstrates how to deploy a multi-tier cloud application using Docker Compose. The deployment consists of a Nextcloud web application and a MariaDB database running in separate containers.

## Objectives

- Understand the purpose of a two-tier architecture.
- Define multiple container services using a `docker-compose.yml` file.
- Deploy and inspect a multi-container application.
- Access the Nextcloud web interface.
- Document deployment commands and reflect on cloud deployment practices.

## Commands Executed

- `mkdir` - Create project directories.
- `nano docker-compose.yml` - Create the Docker Compose configuration.
- `docker-compose up -d` - Start the services in the background.
- `docker-compose ps` - Check container status.
- `docker-compose down` - Stop and remove the Compose containers and network.
- `git add`, `git commit`, and `git push` - Save and upload project documentation to GitHub.

## Skills Learned

- Multi-tier architecture fundamentals.
- Docker Compose configuration and YAML indentation.
- Container networking and environment variables.
- Deploying and managing a Nextcloud and MariaDB stack.
- Technical documentation and GitHub version control.

## Screenshots

Deployment and teardown screenshots are stored in the `screenshots/` directory.
