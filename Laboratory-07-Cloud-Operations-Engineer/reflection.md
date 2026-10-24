# Mission Reflection

This laboratory helped me understand why monitoring is an important responsibility of a Cloud Operations Engineer. Even when containers are running properly, checking the host server's resources is still necessary because the server has limited CPU, RAM, and disk space. If these resources become exhausted, applications may become slow or stop working even when their containers have no configuration problems.

I also learned how the `docker logs` command helps troubleshoot application issues. For example, if a user cannot access a page, I can inspect the logs to find failed requests and HTTP status codes. These details help me identify whether the problem involves an incorrect URL, a missing page, or another application issue instead of relying only on guesses.

Another important lesson is the difference between logs and metrics. Logs describe individual events, such as a successful request or a 404 error. Metrics provide numerical measurements, such as CPU percentage, memory usage, and network activity. Using both gives engineers a better understanding of an application's behavior and performance.

Large enterprise companies may use monitoring platforms such as Prometheus and Grafana to collect, organize, visualize, and monitor information from thousands of containers. Prometheus can collect time-series metrics, while Grafana can display dashboards and help teams identify unusual behavior. Alerts can also notify engineers when important thresholds are exceeded.

My ability to troubleshoot Linux environments has improved because I am now more familiar with commands for checking system resources, testing web requests, inspecting container logs, and measuring resource consumption. Instead of immediately assuming that an application is broken, I can collect evidence and investigate the problem systematically. Overall, this laboratory showed me that cloud operations involves not only deploying applications but also continuously monitoring their health, performance, and reliability.

I learned that even a simple Nginx container produces useful information when users access it. By generating successful and failed requests, I could see how monitoring helps engineers understand real application behavior and make better decisions when troubleshooting a service.
