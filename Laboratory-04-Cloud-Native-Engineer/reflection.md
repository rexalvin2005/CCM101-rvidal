# Mission Reflection

This laboratory helped me understand how containerization can make application deployment faster and easier compared to using traditional Virtual Machines. When installing an operating system on a Virtual Machine, the process usually requires more time because the complete operating system must be installed, configured, and started. In comparison, a Docker container can start within seconds because it uses an existing host operating system kernel and only includes the application and its required dependencies. This makes containers useful for applications that need to be deployed quickly and consistently.

Port mapping is also an important part of running a web server inside a container. The `-p 8080:80` option connects port 8080 of the host machine to port 80 inside the container. Without this mapping, users outside the container would not be able to access the Nginx web server through the host's port. Using `curl http://localhost:8080` allowed me to verify that the Nginx server was successfully running.

I also learned that using `docker rm` removes the container itself. Any data stored only inside the container can be lost when the container is removed, which is why persistent data should normally be stored using Docker volumes or other external storage solutions.

Containerization can also change how developers and IT operations teams work together. Developers can package applications with their dependencies, while operations teams can deploy the same containerized application across different environments. This supports a DevOps approach by improving consistency and simplifying deployment.

My GitHub portfolio is also evolving as I add more cloud computing laboratories. Each activity gives me an opportunity to document what I learned, organize technical files, and demonstrate practical skills. This laboratory adds Docker and cloud-native concepts to my portfolio and shows my progress as an Information Technology student.

