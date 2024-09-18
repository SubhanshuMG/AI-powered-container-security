# AI-powered-container-security
Dive into how AI can automatically detect vulnerabilities and secure Kubernetes and Docker environments—ensuring smarter, faster threat detection.

# How to run the demo

This repository demonstrates an AI-powered security solution for Docker and Kubernetes environments, using Aqua Security for automated vulnerability scanning and threat detection.

## Prerequisites

- Docker
- Kubernetes (Minikube or any other cluster)
- Jenkins
- Aqua Security

## Setup

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/ai-powered-container-security.git
   cd ai-powered-container-security

2. Build the Docker image:
   ```docker build -t ai-secure-app .

3. Run the application in Docker
   ```docker run -d -p 3000:3000 ai-secure-app

4. Deploy the application in Kubernetes
   ```kubectl apply -f kubernetes/ai-secure-app-deployment.yaml

Next Steps:
- Set up your Aqua Security account.
- Push the Docker image to your Docker Hub or any container registry.
- Test the Aqua Security integration with the Jenkins pipeline.