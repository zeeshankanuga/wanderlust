# 🌍 WanderLust – MERN Travel Blog Site with DevSecOps Pipeline 🚀

**WanderLust** is a full-stack **MERN (MongoDB, Express, React, Node.js)** based travel blog website designed to help users share and explore travel stories from around the world.

This open-source project is ideal for those looking to contribute to real-world applications while learning about full-stack development, Docker, CI/CD, and DevSecOps practices.

> 🔗 **Source Code**: [https://github.com/zeeshankanuga/wanderlust.git](https://github.com/zeeshankanuga/wanderlust.git)


## 🏗️ 3-Tier Architecture Overview

WanderLust follows a standard **three-tier architecture**:

### 1. **Frontend (Client Tier)**
- Developed using **React.js**
- Users can read and post travel blogs in a clean, responsive UI

### 2. **Backend (Application Tier)**
- Built with **Node.js** and **Express.js**
- Handles business logic and RESTful API endpoints

### 3. **Database (Data Tier)**
- Powered by **MongoDB**
- Stores user profiles, blog content, and media

All components are containerized using **Docker** and managed through **Docker Compose**.


## 🔐 DevSecOps Features (Integrated in Jenkins Pipeline)

This project features a **secure, automated CI/CD pipeline** implemented with **Jenkins**, along with several security and quality tools:

### 🔁 Jenkins CI/CD Pipeline
- Builds, tests, and deploys automatically via a declarative `Jenkinsfile`

### 🔍 SonarQube Integration
- Performs static code analysis for bugs, code smells, and maintainability

### 🛡️ OWASP Dependency-Check
- Identifies known vulnerabilities in project dependencies (CVEs)

### 🧪 Trivy Security Scanning
- Scans Docker images and file systems for vulnerabilities

These integrations help shift security left in the development lifecycle, promoting a secure-by-design approach.

## 🚀 Deployment

### 📦 Docker & Docker Compose
All services (frontend, backend, database) run in isolated containers.


## 🛠️ Tech Stack Summary

| Layer            | Technology                                 |
|------------------|---------------------------------------------|
| Frontend         | React.js, HTML, CSS                         |
| Backend          | Node.js, Express.js                         |
| Database         | MongoDB                                     |
| Containerization | Docker, Docker Compose                      |
| CI/CD            | Jenkins                                     |
| Code Quality     | SonarQube                                   |
| Security Scans   | OWASP Dependency-Check, Trivy               |
| Future Upgrade   | Kubernetes & Helm Charts (Coming Soon)      |

## 🧑‍💻 How to Contribute

Whether you’re just starting or experienced in DevOps or full-stack development, contributions are always welcome!

You can contribute by:

- Improving UI/UX design
- Fixing bugs or enhancing performance
- Extending DevSecOps capabilities
- Helping transition the project to Kubernetes

### Steps to contribute:

```bash
git clone https://github.com/zeeshankanuga/wanderlust.git
cd wanderlust
docker-compose up --build
```

## 📬 Contact & Community

For any queries, collaboration, or support:

- 📧 **Email**: [zeeshan.kanuga@gmail.com](mailto:zeeshan.kanuga@gmail.com)
- 💼 **LinkedIn**: [Zeeshan Kanuga](https://www.linkedin.com/in/zeeshan-kanuga-6635857a/)
