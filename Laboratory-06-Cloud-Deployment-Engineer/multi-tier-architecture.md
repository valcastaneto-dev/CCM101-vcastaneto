# ☁️ Two-Tier Architecture: Nextcloud and MariaDB

## 📑 Table of Contents

1. [Overview](#1-overview)
2. [The Web/Application Tier](#2-the-webapplication-tier)
3. [The Database Tier](#3-the-database-tier)
4. [Why Separate Them?](#4-why-separate-them)
5. [Architecture Summary](#5-architecture-summary)
6. [Screenshots](#6-screenshots)
7. [Conclusion](#7-conclusion)

---

## 1. Overview

A two-tier architecture is an application design that separates a system into two main parts: the web/application tier and the database tier. In this laboratory, I used Nextcloud for the web application and MariaDB for the database, with Docker Compose managing both services.

| Tier | Service Name | Image | Role |
|------|--------------|-------|------|
| Web/Application | `app` | `nextcloud` | Serves the web interface and handles user requests |
| Database | `database` | `mariadb:10.6` | Stores persistent application data |

---

## 2. The Web/Application Tier

The web/application tier is responsible for displaying the user interface and processing user requests. In this laboratory, Nextcloud serves as the web application that allows users to access and manage their files through a web browser. It receives HTTP requests through port 8080 on the host, which maps to port 80 inside the container.

| Port Mapping | Meaning |
|--------------|---------|
| `8080:80` | Host port 8080 forwards to port 80 inside the Nextcloud container |

---

## 3. The Database Tier

The database tier stores and manages the application's data. In this laboratory, MariaDB is used as the database for Nextcloud. It stores information such as user account details, file metadata, and other application-related records needed for the system to operate.

---

## 4. Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, maintain, and troubleshoot. Each container has a specific responsibility, so the application and database can be updated or configured independently. This separation also makes it easier to scale the components when needed and helps organize the application's security controls.

---

## 5. Architecture Summary

The system uses two main services: Nextcloud and MariaDB. Users access Nextcloud through a web browser using port 8080, while Nextcloud communicates with MariaDB using the service name `database` through Docker's internal network. Docker Compose defines and manages both services using a single YAML configuration file.

```text
Browser ──► Host port 8080 ──► Nextcloud (port 80) ──► database (MariaDB)
                                   app service          internal Docker network
```

---

## 6. Screenshots

The following screenshots provide evidence of the deployment:

- `screenshots/compose-deployment.png` — Shows the successful deployment and both containers running.
- `screenshots/nextcloud-web.png` — Shows the Nextcloud installation page in the browser.
- `screenshots/compose-teardown.png` — Shows the containers being stopped and removed.

---

## 7. Conclusion

This activity helped me understand how a web application and a database work together in a multi-tier architecture. I learned that Docker Compose makes it easier to configure and manage multiple containers using a single YAML file. I also learned that separating services makes an application easier to maintain and troubleshoot.