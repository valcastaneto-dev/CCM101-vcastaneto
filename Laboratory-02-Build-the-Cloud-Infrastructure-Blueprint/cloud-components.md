# Cloud Infrastructure Components

> **Checkpoint 3** — Identification of core cloud infrastructure components
> observed in the KillerCoda Linux environment.

## Table of Contents
- [Compute Resources](#1-compute-resources)
- [Storage Resources](#2-storage-resources)
- [Networking Resources](#3-networking-resources)
- [Operating System](#4-operating-system)

---

## 1. Compute Resources

The compute resource I observed in the KillerCoda Linux environment is the
CPU/processor and its available CPU cores. I used the `lscpu` command to
view information about the CPU.

| | |
|---|---|
| **Purpose** | Compute resources provide the processing power needed to run applications, commands, and processes. |
| **Importance in Cloud Computing** | Compute resources are important in cloud computing because they allow applications and services to perform tasks. Cloud computing can provide different amounts of computing resources depending on the needs of the user or application. |
| **Relation to KillerCoda** | In KillerCoda, the Linux server uses its available CPU resources to execute commands and run processes. The CPU information and available CPU resources were observed using the `lscpu` command. |

---

## 2. Storage Resources

The storage resource I observed in the KillerCoda Linux environment is the
server's disk storage and mounted file systems. I used the `df -h` command
to check the available disk space and file systems.

| | |
|---|---|
| **Purpose** | Storage resources provide a place to store the operating system, applications, files, and other data. |
| **Importance in Cloud Computing** | Storage is important in cloud computing because applications and services need a place to store and access data. Cloud storage can also provide scalable storage for different amounts of data. |
| **Relation to KillerCoda** | The KillerCoda Linux environment uses disk storage to store the operating system and files required by the server. I observed its disk capacity and mounted file systems using the `df -h` command. |

---

## 3. Networking Resources

The networking resources I observed in KillerCoda include the hostname and
IP address of the Linux environment. I used the `hostname` and
`hostname -I` commands to identify them.

| | |
|---|---|
| **Purpose** | Networking resources allow servers, applications, users, and other systems to communicate and exchange information. |
| **Importance in Cloud Computing** | Networking is important in cloud computing because cloud resources need to communicate with users and other services. It provides connectivity between different resources and allows applications to be accessed through a network. |
| **Relation to KillerCoda** | The KillerCoda Linux server has a hostname and IP address that identify it within its network environment. These networking details helped me understand how a cloud server can be connected and accessed through a network. |

---

## 4. Operating System

The operating system I observed in the KillerCoda environment is Linux. I
used the `cat /etc/os-release` command to identify the Linux distribution
and version.

|---|---|
| **Purpose** | An operating system manages the computer's hardware and provides an environment where applications and commands can run. |
| **Importance in Cloud Computing** | The operating system is important in cloud computing because cloud servers need an operating environment for applications and services to run. Linux is commonly used in server and cloud environments. |
| **Relation to KillerCoda** | KillerCoda provides a Linux environment where I was able to execute commands and investigate the server's resources. I identified the operating system and its version using `cat /etc/os-release`. |
