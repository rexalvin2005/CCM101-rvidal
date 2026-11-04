# Firewall Configuration Report

## 1. Allow SSH

Command:

`sudo ufw allow ssh`

This rule permits SSH traffic so administrators can remotely manage the server.

## 2. Configure the Default Policies

Commands:

`sudo ufw default deny incoming`

`sudo ufw default allow outgoing`

The first command blocks incoming connections unless a rule allows them, while the second allows outgoing connections by default.

## 3. Enable the Firewall

Command:

`sudo ufw enable`

After enabling UFW, I used `sudo ufw status verbose` to check the firewall status and default policies.

## 4. Allow the Web Application Port

Command:

`sudo ufw allow 8080/tcp`

This rule allows TCP traffic on port 8080 for the web application.

## 5. Why SSH Must Be Allowed First

If I enable UFW before allowing SSH on a remote server, I could lose my remote administrative connection if the firewall blocks SSH traffic.
