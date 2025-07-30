# 🚀 DevOps CI/CD Pipeline on AWS EKS

This project demonstrates a complete DevOps pipeline using **GitHub Actions**, **Terraform**, **Docker**, and **AWS EKS**. It deploys a containerized web app with monitoring and full automation from code to production.

---

## 🔧 Tech Stack

![Terraform](https://img.shields.io/badge/Terraform-623CE4?logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?logo=helm&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white)

---

## 📦 Features

- ✅ Infrastructure-as-Code (Terraform)
- ✅ CI/CD with GitHub Actions
- ✅ Dockerized web application
- ✅ Kubernetes orchestration on AWS EKS
- ✅ Helm chart deployment
- ✅ Monitoring with Prometheus and Grafana
- ✅ Easy to extend and replicate

---

## 🏗️ Architecture

```
Dev → GitHub → GitHub Actions → Docker Hub → AWS EKS (via Helm) → Monitored by Prometheus & Grafana
```

---

## 🗂️ Project Structure

```
├── infra/             # Terraform scripts
├── scripts/           # Shell scripts for build/deploy
├── ui/                # Monitoring dashboard (HTML/CSS/JS)
├── ci/                # GitHub Actions workflow
├── docs/              # Documentation
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Git
- Terraform CLI
- AWS CLI
- Docker
- kubectl
- Helm

### Steps

1. Clone the repository  
   ```bash
   git clone https://github.com/anthonyokeke1/devops-pipeline-eks.git
   cd devops-pipeline-eks
   ```

2. Deploy infrastructure  
   ```bash
   cd infra
   terraform init
   terraform apply
   ```

3. Build and deploy app  
   ```bash
   ./scripts/build.sh
   ./scripts/deploy.sh
   ```

---

## 📊 Monitoring Dashboard

Access the dashboard at `http://<EKS-LoadBalancer-IP>:3000`  
> Prometheus + Grafana setup details are in `docs/architecture.md`

---

## 👤 Author

**Anthony Okeke**  
📍 Abuja, Nigeria | 🌍 Remote & Relocation Ready  
📧 cyberokeke@gmail.com  
🔗 [GitHub](https://github.com/anthonyokeke1)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
