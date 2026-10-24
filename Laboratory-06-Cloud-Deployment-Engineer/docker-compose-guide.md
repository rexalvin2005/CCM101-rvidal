# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In this project, it defines two services: `database`, which uses the MariaDB image, and `app`, which uses the Nextcloud image. Docker Compose reads these definitions to create and manage the containers together.

## How Does Nextcloud Find the Database?

The `MYSQL_HOST=database` environment variable tells Nextcloud to connect to the database service named `database`. Docker Compose creates a shared network for the services, allowing them to communicate using their service names instead of requiring a manually configured IP address.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is commonly used to start an individual container by specifying its image and options directly in the command. Docker Compose uses a YAML configuration file to define multiple related services and their settings. The `docker-compose up -d` command starts the defined services in the background, making a multi-container deployment easier to repeat and manage.

## Conclusion

Docker Compose helps cloud engineers organize application infrastructure as code. It makes deployments more consistent, easier to understand, and simpler to start or stop as a group.
