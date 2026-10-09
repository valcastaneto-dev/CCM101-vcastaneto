<div align="center">

# 🗄️ MinIO Deployment Documentation

</div>

---

## 📑 Table of Contents
- [Overview](#1-overview)
- [Docker Command Used](#2-docker-command-used)
- [Port Configuration](#3-port-configuration)
- [Environment Variables](#4-environment-variables)
- [Bucket Created](#5-bucket-created)
- [Deployment Verification](#6-deployment-verification)
- [Screenshots](#7-screenshots)
- [Conclusion](#8-conclusion)

---

## 1. Overview

In this activity, I used Docker to deploy MinIO, an S3-compatible object storage server. The purpose was to create a storage bucket and upload a sample file to demonstrate how object storage works.

---

## 2. Docker Command Used

The Docker command I used to run the MinIO server was:

```
docker run -d \
-p 9000:9000 -p 9001:9001 \
--name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
cgr.dev/chainguard/minio server /data --console-address ":9001"
```

---

## 3. Port Configuration

| Port | Purpose |
|---|---|
| **9000** | MinIO API and S3-compatible storage operations |
| **9001** | MinIO web console, accessed through a browser |

I used port 9001 through the KillerCoda port-forwarding interface to access the management console.

---

## 4. Environment Variables

The `-e` flag allows environment variables to be passed into a Docker container.

| Variable | What It Does |
|---|---|
| `MINIO_ROOT_USER=cloudadmin` | Sets the administrator username |
| `MINIO_ROOT_PASSWORD=CloudNova2026!` | Sets the administrator password |

These environment variables configure the login credentials used to access the storage service.

---

## 5. Bucket Created

- **Bucket name:** `client-photos`
- **Purpose:** To organize and store uploaded images and other files for the photo-sharing application.
- **Test file uploaded:** `github-image.jpg`

---

## 6. Deployment Verification

I used the following command to check the container status:

```
docker ps
```

I also checked the container logs when necessary:

```
docker logs minio-server
```

After starting the server, I used the web console to manage the storage service and create the bucket.

---

## 7. Screenshots

The following screenshots provide evidence of the deployment:

- `screenshots/minio-deployed.png` — Shows the Docker container running.
- `screenshots/minio-bucket-upload.png` — Shows the `client-photos` bucket and uploaded file.

---

## 8. Conclusion

This activity helped me understand how Docker can be used to deploy an object storage service. I also learned how port mapping, environment variables, and buckets are used when configuring and managing cloud storage.

---