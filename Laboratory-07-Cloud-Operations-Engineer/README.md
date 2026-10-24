# ☁️ The Cloud Operations Engineer

## 📌 Mission Overview

This laboratory activity focuses on cloud operations, Linux system monitoring, and container observability. Using the KillerCoda Ubuntu Playground, an Nginx web server was deployed in a Docker container, HTTP requests were generated, application logs were examined, and container resource usage was monitored.

---

## 🎯 Objectives

- Monitor host memory and disk capacity using Linux command-line tools.
- Observe CPU utilization and running processes using `top`.
- Deploy an Nginx web server using Docker.
- Generate HTTP requests and simulate a 404 Not Found error.
- Inspect application access logs using `docker logs`.
- Monitor container CPU, memory, and network activity using `docker stats`.
- Document system health and monitoring results using Markdown.

---

## 🛠️ Monitoring Commands Executed

| Command | Description |
|---------|-------------|
| `free -h` | Displays RAM usage and availability. |
| `df -h /` | Displays root filesystem storage capacity. |
| `top` | Monitors CPU activity, system load, and running processes. |
| `docker run -d --name client-website -p 8080:80 nginx` | Creates and runs the Nginx container in the background. |
| `curl -i http://localhost:8080/` | Sends an HTTP request to test the web server. |
| `curl -i http://localhost:8080/hidden-admin-page` | Tests a nonexistent page and generates an HTTP 404 response. |
| `docker logs client-website` | Displays the container's application logs. |
| `docker stats client-website` | Displays real-time resource usage for the container. |

---

## 💡 Skills Learned

- **Linux Monitoring:** Checking memory, disk capacity, CPU activity, and running processes.
- **Docker Management:** Deploying and inspecting a containerized web server.
- **HTTP Testing:** Using `curl` to generate requests and identify HTTP response codes.
- **Log Analysis:** Examining application logs to identify failed requests and troubleshoot issues.
- **Container Observability:** Measuring CPU, memory, and network usage with Docker.
- **Technical Documentation:** Recording monitoring results and organizing evidence using Markdown.

---

## 📊 Key Observations

The Nginx container reported a CPU usage of 0.00% and memory usage of 2.73MiB / 1.859GiB during the recorded measurement. The memory utilization was 0.14%, indicating low resource consumption at that particular time.

The application log evidence recorded an HTTP 404 response for the request to `/hidden-admin-page`. This demonstrated how application logs can help identify unsuccessful requests and investigate website issues.

---

## 📸 Evidence

| Screenshot | Shows |
|------------|-------|
| `screenshots/memory-check.png` | Host memory usage (`free -h`) |
| `screenshots/disk-check.png` | Root filesystem capacity (`df -h`) |
| `screenshots/install-nginx.png` | Nginx container deployment |
| `screenshots/simulation1.png` | Successful HTTP requests |
| `screenshots/simulation2.png` | The 404 Not Found response |
| `screenshots/docker-logs.png` | Container application logs |
| `screenshots/container-metrics.png` | Container resource usage (`docker stats`) |

---

## 📁 Repository Contents

- `README.md` – Mission overview, objectives, commands, and skills learned.
- `system-baseline-report.md` – Host memory, disk, and CPU observations.
- `container-observability.md` – Application logs and container metrics.
- `reflection.md` – Personal reflection on the laboratory activity.
- `screenshots/` – Screenshots collected as laboratory evidence.

---

## ✅ Conclusion

This laboratory activity demonstrated the importance of monitoring both host resources and container performance. Linux monitoring commands, Docker metrics, and application logs provide useful evidence for troubleshooting and assessing the health of a containerized web server.