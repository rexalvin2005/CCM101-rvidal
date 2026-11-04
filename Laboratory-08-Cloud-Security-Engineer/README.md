# Laboratory 08 - Cloud Security Engineer

## Mission Overview

This laboratory demonstrates basic server security using UFW, a host-based firewall in Ubuntu. It covers deploying an Nginx web server, applying a default-deny incoming policy, and allowing only the required network ports.

## Objectives

- Understand the Principle of Least Privilege.
- Identify a server's attack surface.
- Configure UFW firewall rules.
- Allow SSH and web application traffic on the required ports.
- Verify firewall rules and test the Nginx application.

## Commands Executed

- `docker run` - Deploy the Nginx container.
- `curl -I` - Test the HTTP response.
- `sudo ufw allow ssh` - Allow SSH connections.
- `sudo ufw default deny incoming` - Block incoming traffic by default.
- `sudo ufw default allow outgoing` - Allow outgoing traffic.
- `sudo ufw enable` - Enable the firewall.
- `sudo ufw status verbose` - Inspect firewall status and policies.
- `sudo ufw allow 8080/tcp` - Allow TCP port 8080.
- `sudo ufw status numbered` - Display numbered firewall rules.

## Skills Learned

- Basic Linux firewall configuration.
- Network port management.
- Docker-based web server deployment.
- Security auditing and documentation.
- Applying the principle of least privilege and reducing attack surfaces.

## Screenshots

The `screenshots/` directory contains the application test and firewall verification screenshots.
