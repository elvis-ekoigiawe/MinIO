# MinIO on Coolify

This repository contains the setup to deploy MinIO using Docker Compose on a Coolify-managed Ubuntu VPS.

## 📦 What’s Inside

- `docker-compose.yml` — Defines the MinIO container with persistent storage
- `.env` — Stores environment variables like root user and password

---

## 🚀 Deployment Steps

1. **Push this repository to GitHub or GitLab**

2. **In Coolify:**
   - Go to your Project
   - Click `+ New Resource`
   - Choose `Git Repository`
   - Paste the URL of this repo
   - Select `Docker Compose` as the build pack
   - Set the Compose file path as `docker-compose.yml`
   - Click `Create Resource`

3. **Add your domain (e.g., `minio.elvisautomation.site`)**
   - Go to the **Domains** tab in Coolify
   - Click `+ Add Domain`
   - Enter `minio.elvisautomation.site`
   - Set the exposed port to `9000`
   - Enable SSL (Let’s Encrypt)
   - Save the domain

4. **Click Deploy**

---

## 🔐 Default Credentials

- **Username:** `elvis`
- **Password:** `Rudeboy7`

> Change these after first login inside the MinIO console for security.

---

## 🌐 Access

- **MinIO Console UI & S3 API (HTTPS):** https://minio.elvisautomation.site

---

## 🧰 Useful Tips

- Avoid exposing raw IP + ports (e.g., `http://5.189.190.37:8000`)
- Always point Coolify domains to **port 9000 only**
- Use IAM keys instead of root creds in production

---

## 🛡 Recommended Next Steps

- Change root password
- Create buckets and access keys for your apps
- Enable logging and monitor usage
