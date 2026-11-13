# 🌐 Enterprise Cloud Architecture: Laboratory 10

[![Docker Compose](https://img.shields.io/badge/Docker-Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![WordPress](https://img.shields.io/badge/WordPress-5F9EA0?style=for-the-badge&logo=wordpress&logoColor=white)](https://wordpress.org/)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Ubuntu Server](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/)

A containerized, multi-tier enterprise web service cluster engineered for the **CCM101** cloud infrastructure curriculum. This architecture decouples front-end content delivery from persistent transactional database storage using isolated Docker bridge networking, declarative orchestration, and automated local backup flows.

---

## 📖 Project Overview

Modern enterprise deployments demand strict isolation between public-facing web applications and backend data stores. In **Laboratory 10**, a monolithic WordPress and MySQL stack is decomposed into independent, reproducible microservices running on an Ubuntu Server host. By routing inter-container traffic through a custom bridge network (`enterprise_net`) while exposing only the HTTP application gateway to the host, the stack minimizes its external attack surface and guarantees zero-downtime data persistence across container lifecycles.

---

## 🧩 Service Specifications

| Service Container | Role & Responsibilities | Port Exposure | Storage & Persistence |
| :--- | :--- | :--- | :--- |
| **`enterprise_wordpress_app`** | Handles client HTTP requests, theme rendering, and CMS administration | `8080:80` (Public) | Persistent volume mapping for `/var/www/html` |
| **`enterprise_mysql_db`** | Manages relational database schemas, user authentication, and post transactions | `3306` (Internal Only) | Dedicated named volume (`db_data`) for `/var/lib/mysql` |

---

## 📁 Repository Structure

```text
CCM101-rvidal/
├── Laboratory-10-Enterprise-Cloud-Architect/
│   ├── docker-compose.yml       # Multi-container orchestration & network definitions
│   ├── .env                     # Environment secrets & database credentials (gitignored)
│   └── backup/                  # Automated database & volume backup routines
└── README.md                    # System documentation & deployment manual
