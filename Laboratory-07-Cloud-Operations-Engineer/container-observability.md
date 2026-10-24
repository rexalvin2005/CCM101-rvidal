# Container Observability Report

## Application Logs

### Failed HTTP Request

Paste the actual Nginx log entry for the `/hidden-admin-page` request here.

### Why Logs Matter

Application logs help engineers identify failed requests, investigate errors, and understand what happened before a problem occurred. They provide useful details such as request paths, timestamps, and HTTP status codes, making troubleshooting more accurate.

## Container Resource Metrics

### Client Website Container

- Memory Usage: [Record the actual value shown by `docker stats`]
- CPU Percentage: [Record the actual percentage shown by `docker stats`]

### Why Metrics Matter

Container metrics help engineers determine whether an application is consuming too much CPU or memory. Monitoring these values can reveal resource bottlenecks before they cause service interruptions.
