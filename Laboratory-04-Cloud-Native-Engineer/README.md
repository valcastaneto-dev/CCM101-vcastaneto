<div align="center">

# 🐳 Laboratory 04 — Cloud-Native Engineer

</div>

---

## 🧭 Mission Overview

Congratulations! After successfully guiding our clients through multi-cloud evaluations, you have been promoted to the Cloud-Native Engineering Team at CloudNova Technologies. Modern cloud computing is no longer just about renting Virtual Machines (VMs) from AWS or Azure. Today's enterprise applications are built using lightweight, portable, and lightning-fast technologies called Containers. Your new mission is to understand the shift from traditional virtualization to containerization. Using the KillerCoda Playground, you will step into the shoes of a Cloud-Native Engineer. You will research the differences between VMs and containers, execute your very first Docker commands, and deploy a live, containerized web server in seconds.

---

## 🎯 Objectives
- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull, run, manage, and terminate a containerized application (Nginx).
- Create professional technical documentation of container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing Portfolio.

---

## 📁 Contents
| File | Description |
|---|---|
| [`virtualization-vs-containers.md`](./virtualization-vs-containers.md) | VM vs. container comparison table + client summary |
| [`docker-deployment.md`](./docker-deployment.md) | Docker verification, Nginx deployment, container lifecycle |
| [`reflection.md`](./reflection.md) | Mission reflection |
| `screenshots/` | Evidence screenshots |

## 🖥️ Commands Executed

| Command | What It Does |
|---|---|
| `docker --version` | Displays the installed Docker version to confirm Docker is installed. |
| `docker info` | Displays the current status and details of the Docker environment. |
| `docker pull nginx` | Downloads the official Nginx image from Docker Hub. |
| `docker run -d -p 8080:80 --name nginx-server nginx` | Runs the Nginx container in detached mode, maps host port 8080 to container port 80, and names it `nginx-server`. |
| `curl http://localhost:8080` | Sends an HTTP request to confirm the Nginx web server is running. |
| `docker ps` | Displays the Docker containers that are currently running. |
| `docker stop nginx-server` | Stops the running Nginx container without removing it. |
| `docker ps -a` | Displays all containers and allows verification that the Nginx container has stopped. |
| `docker rm nginx-server` | Removes the stopped Nginx container completely from the Docker environment. |

---

## 💡 Skills Learned
- I learned how to check whether Docker is installed and running.
- I learned how to download and run a Docker image.
- I learned how to map a host port to a container port.
- I learned how to test a web server using `curl`.
- I learned how to stop and remove Docker containers.

---

## 🧩 Challenges Encountered
One challenge I had was understanding how Docker connects the host port to the container port. At first, I was also a little unsure about which container name to use when stopping and removing it. After checking my commands and the container status, I was able to understand the process and complete the activity successfully.

---



---
