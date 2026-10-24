# Two-Tier Architecture

## The Web/Application Tier

The web/application tier is responsible for displaying the user interface and handling HTTP requests from users. In this laboratory, Nextcloud runs inside the application container and provides the web interface that users access through a browser.

## The Database Tier

The database tier stores persistent information used by the application, such as user accounts, settings, and other application data. In this deployment, MariaDB acts as the database server, while Nextcloud connects to it to store and retrieve information.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, troubleshoot, and maintain. Each container has its own responsibility, and the application and database can be updated or scaled independently. This separation also helps organize the deployment and reduces the need to install every component in one container.
