# Mission Reflection

Object storage is well suited for storing millions of photos because it is designed to manage large amounts of unstructured data. Unlike traditional block storage, which presents storage as blocks that an operating system or application must manage through a file system, object storage stores each image as an object with its own identifier and metadata. Object storage services can scale to support growing collections of images and provide features for durability and access management. This makes object storage a practical choice for photo-sharing platforms and other applications with many user-uploaded files.

Docker made deploying MinIO easier because I did not need to manually install and configure every component on the operating system. By running a Docker command, I could download the MinIO image, configure the required environment variables, map the ports, and start the server in a container. I could also check the container status and logs using Docker commands, which made the deployment process easier to manage.

A bucket is a logical container used to organize objects in an object storage system. In this activity, I created a bucket named `client-photos` and uploaded a sample file. A real application could use a bucket to store uploaded images and retrieve them when users need them.

Large enterprise companies reduce the risk of losing object storage data through redundancy, replication, backups, and durable storage systems. Depending on the service and configuration, data may be stored across multiple devices or locations so that a hardware failure does not automatically cause permanent data loss. Companies must also configure access controls, retention policies, and recovery procedures to protect important information.

My confidence in using the Linux command line is improving through each laboratory activity. I have practiced creating folders, managing Markdown files, running Docker containers, checking logs, and verifying services. This activity helped me connect cloud storage concepts with a working storage server. It also improved my ability to troubleshoot issues and document technical steps in my GitHub portfolio.
