# MinIO on Coolify

This repository contains the setup to deploy MinIO using Docker Compose on a Coolify-managed Ubuntu VPS.

## 📦 What’s Inside

- `docker-compose.yml` — Defines the MinIO container
- `.env` — Stores environment variables like root user and password

## 🚀 Deployment Steps

1. **Push this repository to GitHub or GitLab**

2. **In Coolify:**
   - Click `+ New Resource`
   - Choose `Git Repository`
   - Paste the URL of this repo
   - Select `Docker Compose` as the build pack
   - Click `Create Resource`

3. **Set up your domain (e.g., `minio.elvisautomation.site`)**
   - Go to the **Domains** tab in Coolify
   - Add your domain
   - Set the exposed port to `9001`
   - Enable SSL

4. **Click Deploy**

## 🔐 Default Credentials

- **Username:** `elvis`
- **Password:** `Rudeboy7`

Change these after first login.

## 🌐 Access

- **MinIO Console UI:** `https://minio.elvisautomation.site`
- **S3 API:** `http://5.189.190.37:8000` (Replace IP with your VPS's IP address)
- **S3 API (SSL):** `https://minio.elvisautomation.site` (Replace IP with your VPS's IP address)
