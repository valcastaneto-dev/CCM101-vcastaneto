# 🐳 Docker Compose Guide

## 📑 Table of Contents

1. [Compose File Used](#1-compose-file-used)
2. [What Does the `services:` Block Do?](#2-what-does-the-services-block-do)
3. [How Does Nextcloud Find MariaDB?](#3-how-does-nextcloud-find-mariadb)
4. [Difference Between `docker run` and `docker-compose up -d`](#4-difference-between-docker-run-and-docker-compose-up--d)
5. [Infrastructure as Code](#5-infrastructure-as-code)
6. [References](#6-references)

---

## 1. Compose File Used

```yaml
version: '3'

services:
  database:
    image: mariadb:10.6
    environment:
      - MYSQL_ROOT_PASSWORD=cloudnova_root
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user

  app:
    image: nextcloud
    ports:
      - 8080:80
    environment:
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user
      - MYSQL_HOST=database
```

| Service | Image | Port Mapping |
|---------|-------|--------------|
| `database` | `mariadb:10.6` | None (internal network only) |
| `app` | `nextcloud` | `8080:80` |

---

## 2. What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In this deployment, it declares two services: `database`, which uses the MariaDB 10.6 image, and `app`, which uses the Nextcloud image. Each service has its own configuration, including its image, environment variables, or port mappings.

---

## 3. How Does Nextcloud Find MariaDB?

The environment variable `MYSQL_HOST=database` tells Nextcloud to connect to the database service using the hostname `database`. Docker Compose provides service-name-based networking on its default network, allowing the application container to reach the database container without requiring a manually assigned IP address.

---

## 4. Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is commonly used to create and start an individual container with options specified on the command line. Docker Compose uses a YAML configuration file to define multiple related services and starts them together with `docker-compose up -d`. The `-d` option runs the services in the background, while the configuration file makes the deployment easier to repeat and maintain.

---

## 5. Infrastructure as Code

Infrastructure as Code (IaC) means defining infrastructure through machine-readable configuration files rather than relying entirely on manual setup. The Compose file records the application's service definitions and settings, making deployments more consistent, understandable, and repeatable.

---

## 6. References

- Docker Compose documentation: <https://docs.docker.com/compose/>
- Docker networking documentation: <https://docs.docker.com/compose/how-tos/networking/>