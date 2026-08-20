# Laboratory 02 – Build the Cloud Infrastructure Blueprint

> Technical documentation summarizing the mission,
> objectives, tools, commands, and outcomes of this laboratory activity.

## Table of Contents
- [Mission Overview](#mission-overview)
- [Objectives](#objectives)
- [Cloud Infrastructure Components](#cloud-infrastructure-components)
- [Tools Used](#tools-used)
- [Linux Commands Executed](#linux-commands-executed)
- [Skills Learned](#skills-learned)
- [Challenges Encountered](#challenges-encountered)

---

## Mission Overview

Congratulations,

Your onboarding has been successfully completed, and your Cloud Computing Portfolio has been approved by your supervisor.

CloudNova Technologies has now assigned you to your first official project.

Before deploying cloud services, every cloud engineer must understand the infrastructure that powers modern cloud computing. Your mission is to investigate the components of cloud infrastructure, identify how compute, storage, networking, and identity services work together, and document your findings as if you were preparing technical documentation for a client.

Using the KillerCoda Playground, Linux tools, official cloud documentation, and your GitHub Cloud Computing Portfolio, you will complete a series of engineering tasks that simulate the planning phase of a cloud deployment.

Remember: **Great cloud engineers build systems—but exceptional cloud engineers document and justify every design decision.**

---

## Objectives

- Explain the major components of cloud infrastructure
- Investigate the hardware and software resources available in a Linux environment
- Differentiate compute, storage, networking, and identity resources
- Interpret the relationship between cloud infrastructure components
- Create professional technical documentation using Markdown
- Continue building a structured GitHub Cloud Computing Portfolio

---

## Cloud Infrastructure Components

On the KillerCoda Linux server, I identified the CPU as the compute resource, disk storage as the storage resource, and the hostname/IP as networking resources. The operating system was Linux, which manages hardware and provides the environment for these components to work together.

Full details are documented in [`cloud-components.md`](./cloud-components.md).

---

## Tools Used

- KillerCoda Playground
- Linux terminal
- GitHub
- Draw.io

---

## Linux Commands Executed

| Command | What It's Used For |
|---|---|
| `cat /etc/os-release` | Displays the Linux distribution name and version running on the server |
| `uname -r` | Shows the current kernel version in use |
| `lscpu` | Shows CPU details, including the processor model and number of cores |
| `free -h` | Shows how much RAM is installed, in use, and available, in human-readable format |
| `df -h` | Shows disk space usage and capacity for each mounted filesystem |
| `hostname` | Displays the name assigned to the server |
| `hostname -I` | Displays the server's assigned IP address(es) |

---

## Skills Learned

- How to inspect Linux system resources using terminal commands
- How to interpret CPU, memory, and disk information
- How to research and compare cloud provider services
- How to build a basic cloud architecture diagram

---

## Challenges Encountered

- Understanding the difference between the "Size" and "Mounted on" columns in `df -h` output
- Deciding how to visually represent the cloud boundary in the architecture diagram
