# MinIO Deployment Documentation

## Introduction

For this laboratory, I deployed MinIO using Docker in the KillerCoda Ubuntu Playground. The purpose was to create a simple object storage environment similar to a cloud storage service. I also used the MinIO web console to create a bucket and upload a sample file.

## Docker Command Used

I used the following command to run MinIO:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

At first, the command looked complicated because it contains several options. After breaking it down, I understood that the command was creating a MinIO container and configuring the ports and login credentials at the same time.

## Checking the Container

After running the command, I checked if the container was running using:

```bash
docker ps
```

I looked for the container named:

```text
minio-server
```

The container was running successfully, which showed me that the MinIO server had started properly.

## Port Configuration

I used two ports in the Docker command:

| Port   | Purpose           |
| ------ | ----------------- |
| `9000` | MinIO API         |
| `9001` | MinIO Web Console |

I used **port 9001** to access the MinIO Web Console through the KillerCoda port access feature.

## Environment Variables

The `-e` options were used to set environment variables for MinIO.

```text
-e "MINIO_ROOT_USER=cloudadmin"
-e "MINIO_ROOT_PASSWORD=CloudNova2026!"
```

The first variable sets the administrator username, while the second sets the administrator password. I learned that environment variables can be useful because configuration values can be provided when the container starts instead of having to configure them manually afterward.

## Creating the Bucket

After opening the MinIO Web Console, I logged in using the credentials from the Docker command. I then went to **Buckets** and created a bucket named:

```text
client-photos
```

After creating the bucket, I uploaded a sample file to test whether the object storage system was working correctly.

## My Understanding

The part I found useful was seeing the connection between Docker and cloud storage. Docker handled the deployment of MinIO, while the MinIO web console allowed me to manage the storage without having to use only command-line commands.

This activity also helped me understand why ports are important. Port `9001` allowed me to access the MinIO management interface through my browser, while port `9000` was used for the MinIO API.

## Evidence

The deployment screenshot is saved as:

```text
screenshots/minio-deployed.png
```

The bucket and uploaded object screenshot is saved as:

```text
screenshots/minio-bucket-upload.png
```

