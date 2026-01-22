# DevOps Term Project – University Department Website

## 📌 Project Overview

This repository contains an **end-to-end DevOps term project** for a static **University Department website**. The main goal of this project is to practically implement core DevOps concepts including **Git Flow**, **Docker containerization**, **Continuous Integration (CI)**, **Continuous Deployment (CD)**, and **multi-environment deployment** using **GitHub Actions** and **Render**.

The website is intentionally kept static and simple so that the focus remains on DevOps workflows, automation, and collaboration practices.

---

## 🎯 Project Objectives

* Implement a complete end-to-end DevOps workflow
* Practice Git Flow and collaborative development
* Containerize a static website using Docker
* Design separate CI and CD pipelines for multiple environments
* Deploy the application automatically to Development, Staging/QA, and Production environments
* Manage secrets securely using GitHub Environments and Render

---

## 🌐 Website Pages

The static website consists of the following pages:

* **Home Page:** Department overview, mission, and highlights
* **Courses Page:** List of courses with brief descriptions
* **Faculty Page:** Faculty profiles and office hours
* **Admissions Page:** Admission criteria, process, and deadlines
* **Contact Page:** Contact details and department location
* **Events Page:** Shows social and educational events happening in university

---

## 🔀 Git Flow Strategy

The project follows **Git Flow best practices**:

* `feature/*` – Individual feature development (HTML/CSS pages, workflows)
* `develop` – Integration branch for all team members
* `staging` – QA and testing environment
* `main` – Production-ready code

---

## 🐳 Dockerization

* The website is containerized using **Docker**
* A single **Dockerfile** is used for all environments
* Multi-stage build is used to build the website and serve it using **Nginx**

---

## ⚙️ CI/CD Pipelines

### Continuous Integration (CI)

* HTML and CSS linting
* Application build process
* Docker image build and push to Docker Hub
* Different image tags for each environment:

  * `dev` for Development
  * `qa` for Staging/QA
  * `prod` for Production

### Continuous Deployment (CD)

* Automated deployment using **Render Deploy Hooks**
* Separate deployment pipelines for:

  * Development
  * Staging/QA
  * Production

---

## 🔐 Secrets Management

* **Docker Hub credentials** stored as repository secrets
* **Render deploy hooks** stored using **GitHub Environments**:

  * `development`
  * `staging`
  * `production`

---

## 🚀 Deployment Environments

The application is deployed to three separate Render web services:

* **Development Environment**
* **Staging / QA Environment**
* **Production Environment**

Each environment has its own URL and deployment pipeline.

---

## 🧪 Local Setup & Testing

```bash
# Build Docker image locally
docker build -t devops-term-project .

# Run container locally
docker run -p 8080:80 devops-term-project
```

Access the website at: `http://localhost:8080`

---

## 📄 License

This project is created for **academic purposes** as part of a DevOps course.

---

✅ **This repository demonstrates industry-standard DevOps practices applied to a real-world inspired academic project.**
