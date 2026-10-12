# MinIO Deployment

## Overview

MinIO is an S3-compatible object storage server. In this laboratory, Docker was used to deploy MinIO and its web console was used to create a bucket for client photos.

## Docker Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e MINIO_ROOT_USER=cloudadmin -e MINIO_ROOT_PASSWORD=CloudNova2026! minio/minio server /data --console-address ":9001"
