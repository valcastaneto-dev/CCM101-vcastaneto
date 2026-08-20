# Infrastructure Report

> Investigation of the Linux server environment provided
> by the KillerCoda Playground.

## Table of Contents
- [Server Information](#server-information)
- [Disk Capacity & Mounted File Systems](#disk-capacity--mounted-file-systems)
- [Network Information](#network-information)

---

## Server Information

| Item | Result |
|---|---|
| **Operating System** | Ubuntu 24.04.4 LTS |
| **Kernel Version** | 6.8.0-138-generic |
| **CPU Model** | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| **CPU(s)** | 1 |
| **Total RAM** | 19Gi |

---

## Disk Capacity & Mounted File Systems

```
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           191M  992K  190M   1% /run
/dev/vda1        19G  5.4G   13G  30% /
tmpfs           952M   84K  952M   1% /dev/shm
tmpfs           5.0M     0  5.0M   0% /run/lock
/dev/vda16      881M  117M  703M  15% /boot
/dev/vda15      105M  6.2M   99M   6% /boot/efi
```

The main filesystem is mounted at `/` on `/dev/vda1`, with a total capacity of 19G, of which 5.4G is used (30%). The remaining mounts (`/boot`, `/boot/efi`, and the `tmpfs` entries) are smaller system and temporary filesystems used for boot files and in-memory storage.

---

## Network Information

| Item | Result |
|---|---|
| **Hostname** | ubuntu |
| **IP Address** | 172.30.1.2, 172.17.0.1 |

---

## Evidence

- `screenshots/server-information-1.png`
- `screenshots/server-information-2.png`
- `screenshots/storage-information.png`
- `screenshots/network-information.png`
