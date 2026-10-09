<div align="center">

# ☁️ Research: Types of Cloud Storage

</div>

---

## 📑 Table of Contents
- [Comparison of Cloud Storage Types](#comparison-of-cloud-storage-types)
- [Why Object Storage Is Best for User-Uploaded Images](#why-object-storage-is-best-for-user-uploaded-images)
- [References](#references)

---

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Divides data into fixed-sized blocks that work together like a hard drive. | Best for virtual machines, operating systems, and databases that need fast data access. | AWS EBS |
| **File Storage** | Organizes data into files and folders, similar to the file system on a regular computer. | Best for shared folders and applications that need to access the same files. | AWS EFS |
| **Object Storage** | Stores data as individual objects containing the file, its metadata, and a unique identifier. | Best for storing images, videos, backups, and other uploaded files. | AWS S3 |

---

## Why Object Storage Is Best for User-Uploaded Images

Object Storage is a good choice for our client's photo-sharing application because it can handle large numbers of images as the application grows. Services like AWS S3 make it easy to store and retrieve images without keeping them inside the web server. It also provides durable storage and can work with a content delivery network (CDN) to help images load faster for users.

---

## References

- Amazon Web Services. [What is Cloud Storage?](https://aws.amazon.com/what-is/cloud-storage/)
- Amazon Web Services. [Amazon S3](https://aws.amazon.com/s3/)
- Amazon Web Services. [Amazon EBS](https://aws.amazon.com/ebs/)
- Amazon Web Services. [Amazon EFS](https://aws.amazon.com/efs/)

---