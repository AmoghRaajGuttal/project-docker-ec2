# Cloud Demo App — Docker + GitHub Actions → AWS EC2

A simple Flask web app packaged in Docker, automatically built and deployed to an AWS EC2 instance via GitHub Actions.

**Status:** ✅ Deployed (via GitHub Actions)

---

## Overview

This project demonstrates a small end-to-end DevOps workflow:

- Containerize a Python/Flask app using Docker.
- Build and push Docker images to DockerHub.
- Deploy the Docker image onto an AWS EC2 instance using GitHub Actions (SSH).
- Automatic redeploy on `main` branch pushes.

---

## Repo layout

├─ cloud-demo/
│ └─ app/
│ ├─ app.py
│ └─ requirements.txt
├─ docker/
│ └─ Dockerfile
├─ nginx/
│ └─ default.conf
├─ deploy/
│ └─ deploy.sh
├─ .github/
│ └─ workflows/
│ └─ deploy.yml
├─ .gitignore
└─ README.md