<div align="center">

# 🚀 Multi-Cloud Explorer

**CloudNova Technologies Cloud Evaluation Team

</div>

---

## 🧭 Mission Summary
As part of CloudNova Technologies' Cloud Evaluation Team, this lab explores AWS, Microsoft Azure, and Google Cloud Platform, compares their core services, and recommends the most appropriate cloud provider for different client business scenarios.

## 📁 Contents
| File | Description |
|---|---|
| [`aws-research.md`](./aws-research.md) | AWS overview, infrastructure, core services, advantages, use cases |
| [`azure-research.md`](./azure-research.md) | Azure overview, infrastructure, core services, advantages, use cases |
| [`gcp-research.md`](./gcp-research.md) | GCP overview, infrastructure, core services, advantages, use cases |
| [`cloud-platform-comparison.md`](./cloud-platform-comparison.md) | Comparison table + equivalent services table |
| [`client-recommendations.md`](./client-recommendations.md) | Recommendations for 4 client scenarios + decision matrix |
| [`reflection.md`](./reflection.md) | Mission reflection |
| `screenshots/` | Evidence screenshots |

---

## 🐧 Checkpoint 7 — Linux Investigation (KillerCoda)

A Linux Playground was launched in KillerCoda, and Linux commands were used to identify the operating system, CPU, memory, and disk space.

### Commands Used

| Command | What It's Used For |
|---|---|
| `cat /etc/os-release` | Displays the Linux distribution name and version running on the server |
| `lscpu` | Displays CPU architecture, number of CPUs, cores, and other processor details |
| `free -h` | Displays total, used, and available system memory in human-readable format |
| `df -h` | Displays available and used disk space for mounted file systems |

---

## ☁️ Cloud Migration Options

If this Linux server were migrated to the cloud, it could be hosted using virtual machine services from AWS, Microsoft Azure, or Google Cloud.

| Cloud Provider | Service | Purpose |
|---|---|---|
| 🟧 **AWS** | Amazon EC2 | Hosts Linux virtual machines in the AWS cloud. |
| 🔵 **Microsoft Azure** | Azure Virtual Machines | Hosts Linux virtual machines in Microsoft Azure. |
| 🔴 **Google Cloud** | Compute Engine | Hosts Linux virtual machines on Google Cloud. |

### AWS — Amazon EC2
Amazon EC2 (Elastic Compute Cloud) would allow the Linux server to run as a virtual machine in AWS. The CPU, memory, storage, and networking resources can be selected according to the server's requirements.

### Microsoft Azure — Azure Virtual Machines
Azure Virtual Machines can host Linux-based servers in Microsoft's cloud. The virtual machine size can be selected based on the CPU and memory requirements of the original server.

### Google Cloud — Compute Engine
Google Compute Engine provides virtual machines that can run Linux operating systems. The machine type, storage, and other resources can be configured to match the requirements of the existing Linux server.

### 🏁 Conclusion
The Linux server could be migrated to any of the three major cloud platforms. Amazon EC2, Azure Virtual Machines, and Google Compute Engine all provide virtual machine environments capable of running Linux, so the final choice would depend on factors such as cost, existing infrastructure, performance requirements, and preferred cloud ecosystem.

---


---

<p align="center"><sub>⚠️ Note: System info output and terminal screenshots not yet included — see lab instructions for evidence requirements.</sub></p>
