# Mission Reflection

This laboratory helped me understand how Docker Compose makes deploying cloud applications easier and more organized. Instead of typing separate Docker commands for every container, I can define the services, images, ports, and environment variables in one `docker-compose.yml` file. This saves time, reduces repeated work, and makes it easier to deploy the same setup again.

I also learned that YAML indentation is very important. If I accidentally use a Tab instead of spaces or place a line at the wrong indentation level, Docker Compose may fail to read the configuration. This means I need to check the spacing and structure carefully before starting the deployment. A small formatting mistake can prevent the whole stack from starting correctly.

Environment variables, such as `MYSQL_PASSWORD`, allow the application and database to use the configuration values they need. For example, Nextcloud uses the database name, username, password, and host to connect to MariaDB. I learned that the host can be the Compose service name, `database`, because the services can communicate through their shared network. However, I also understand that passwords written directly in a Compose file are suitable only for this classroom exercise and should be handled more securely in real projects.

Deploying Nextcloud in a few minutes felt rewarding because I could see how several components work together to provide a cloud storage service. The application container handles the web interface, while the database container stores the information required by the application.

Since Mission 1, my understanding of cloud computing has grown from learning basic cloud concepts and infrastructure to actually configuring and deploying a multi-container application. I now understand more clearly how containers, networking, configuration files, and databases work together. This activity also showed me why automation and documentation are important skills for a cloud engineer.
