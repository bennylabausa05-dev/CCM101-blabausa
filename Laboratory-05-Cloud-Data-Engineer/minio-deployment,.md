# MinIO Deployment

## Docker command used

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  scnd/minio-mirror:RELEASE.2025-09-07T16-13-09Z server /data --console-address ":9001"
```

Note: the module's `minio/minio` image is no longer available on Docker Hub, so I used `scnd/minio-mirror`, an unmodified copy of the last official MinIO release.

## Web console port

**9001** (opened through the KillerCoda "Traffic / Ports" menu). The S3 API runs on port 9000.

## Bucket created

**client-photos**

## What the `-e` flags did

The `-e` flag sets environment variables inside the container. MinIO reads them at startup:

- `MINIO_ROOT_USER=cloudadmin` set the admin username.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` set the admin password.

These are the credentials I used to log in to the web console. Without them, MinIO would fall back to the default `minioadmin` / `minioadmin` login.
