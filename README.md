# 🚀 ECommerce Shopping Website CI/CD Pipeline | Ultimate DevOps Project 🚀

This project showcases the implementation of a highly efficient CI/CD pipeline tailored for an ECommerce shopping platform, optimizing development and deployment processes across 11 microservices.

## 🏗️ Project Overview
- **Microservices Architecture**: Implemented CI/CD for 11 microservices.
- **CI/CD Automation**: Streamlined the build, test, and deployment process.
- **Infrastructure as Code**: Managed cloud infrastructure using Terraform.
- **Containerized Deployment**: Leveraged Docker and Kubernetes for scalable deployments.

## 📌 Key Features

### 🔗 Branch-Per-Microservice Strategy
- Adopted a **branch-per-microservice** model.
- Ensured **granular version control** and **streamlined collaboration**.
- Simplified maintenance workflows for efficient microservice updates.

### 🛠️ Jenkinsfile Integration
- Integrated **Jenkinsfiles** within each microservice repository.
- Enabled tailored pipeline configurations for seamless CI/CD execution.
- Enhanced maintainability and automation of build/test processes.

### 🔄 Automated Pipeline Triggering
- Configured **multibranch pipeline automation**.
- Used **generic webhook triggers** for automatic CI pipeline activation.
- Minimized manual intervention and increased development efficiency.

### 🏑 Docker Image CI Pipelines
- Built **11 independent CI pipelines** for **Docker images**.
- Ensured uniformity and reliability in containerized application artifacts.
- Automated build verification and testing before image push.

### 🛳️ Automated Docker Image Pushing
- Automated **pushing of Docker images** to a container registry post-build.
- Reduced operational overhead with seamless artifact delivery.
- Ensured rapid deployment readiness across multiple environments.

### 🚀 Terraform for Infrastructure as Code (IaC)
- Defined and provisioned cloud infrastructure using **Terraform**.
- Managed **EC2 instances, security groups, and EKS cluster**.
- Ensured **consistent, repeatable, and scalable deployments**.

### 🌐 Kubernetes-Driven Deployments
- Used **Kubernetes manifests** for declarative application deployments.
- Orchestrated **scalable, automated rollouts** across environments.
- Improved **resilience and fault tolerance** with microservice-based deployment.

## 📂 Repository Structure
```bash
📦 ecommerce-ci-cd-pipeline
├── 📁 microservice-1
│   ├── Dockerfile
│   ├── Jenkinsfile
│   └── k8s-deployment.yaml
├── 📁 microservice-2
│   ├── Dockerfile
│   ├── Jenkinsfile
│   └── k8s-deployment.yaml
├── 📁 terraform
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
├── 📁 kubernetes
│   ├── deployment.yaml
│   ├── service.yaml
└── README.md
```

## 🚀 How to Get Started
### Prerequisites
- **Docker & Kubernetes** installed
- **Jenkins** configured with GitHub Webhooks
- **Terraform** for infrastructure automation

### Deployment Steps
1. **Clone the repository**
   ```bash
   git clone [https://github.com/your-repo/ecommerce-ci-cd-pipeline.git](https://github.com/harshal1996sahadeokar/DEVOPS-PROJECT-3-E-Commerce-Website-via-CI-CD.git)
   cd ecommerce-ci-cd-pipeline
   ```
2. **Deploy Infrastructure with Terraform**
   ```bash
   cd terraform
   terraform init
   terraform apply -auto-approve
   ```
3. **Build and Push Docker Images**
   ```bash
   docker build -t your-registry/microservice-1:latest ./microservice-1
   docker push your-registry/microservice-1:latest
   ```
4. **Deploy to Kubernetes**
   ```bash
   kubectl apply -f kubernetes/deployment.yaml
   ```

## 🎯 Future Enhancements
- **Implement Helm charts** for simplified Kubernetes deployment.
- **Add monitoring and logging** with Prometheus & Grafana.
- **Enable blue-green deployments** for zero-downtime releases.

## 📜 License
This project is licensed under the MIT License.

## 👨‍💻 Author
**Harshal Sahadeokar** - [GitHub Profile](https://github.com/your-profile)
