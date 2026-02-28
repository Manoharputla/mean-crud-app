# DevOps Engineer Internship Assignment

## MEAN Stack Application – Docker | CI/CD | AWS | Nginx

---

## Project setup

## Project Overview

This project demonstrates containerization, CI/CD automation, and cloud deployment of a full-stack **MEAN (MongoDB, Express, Angular, Node.js)** application.

The application has been:

- Containerized using Docker
- Orchestrated using Docker Compose
- Deployed on an Ubuntu EC2 instance
- Configured with Nginx Reverse Proxy (Port 80)
- Automated using Jenkins CI/CD pipeline

---

# Assignment Requirements & Implementation

---

## 1. Repository Setup

- Created a new GitHub repository
- Pushed complete source code
- Included:
  - Backend Dockerfile
  - Frontend Dockerfile
  - docker-compose.yml
  - Nginx configuration
  - README.md

## GitHub URL: https://github.com/Manoharputla/mean-crud-app.git

## 2. Containerization

### Backend

- Base Image: Node
- Installs dependencies
- Runs Express server on port 8080

### Frontend

- Multi-stage Docker build
- Angular production build
- Served via Nginx

---

## Docker Images

## Service - Docker Image

Backend - manohar2024/backend-image
Frontend - manohar2024/frontend-image
MongoDB - Official Mongo image
Nginx - Official Nginx image

Docker images are built and pushed to Docker Hub through Jenkins pipeline.

---

## 3. Docker Compose Deployment

All services are defined in `docker-compose.yml`.

Services:

- mongo
- backend
- frontend
- nginx

To start the application:

````bash
docker compose up -d

To deploy the application:

```Open Browser
http://43.205.127.95
````
