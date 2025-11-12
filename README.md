# DevOps Templates

A curated collection of secure, production-ready CI/CD templates and GitHub Actions workflows. 
Accelerate your DevOps setup with built-in security scanning, artifact signing, and best practices.

## 🛡️ Security First
- Container vulnerability scanning with Trivy
- Cosign keyless signing for supply chain security
- SBOM generation and compliance checks
- Security gates and policy enforcement

## 🚀 Quick Start
Copy-paste ready templates for:
- Secure container builds and signing
- Kubernetes deployments
- Multi-architecture builds
- Security scanning pipelines

## 📋 Usage Example
### Step 1: Create your project structure:

```go
your-username/your-project/
├── .github/workflows/
│   └── ci.yml          # ← Create this file
├── src/
├── Dockerfile
└── package.json
```
### Step 2: In ci.yml add:

```go
name: 🚀 CI/CD Pipeline

on: [push]

jobs:
build-and-scan:
uses: cooler-SAI/devops-templates/.github/workflows/secure-container.yml@main
with:
image-name: your-app-name
docker-context: .
```

### Step 3: Commit and push - done! 🎉

## 📁 Available Templates

#### secure-container.yml - Build, scan and sign containers

#### k8s-deploy.yml - Kubernetes deployment workflows

#### security-scan.yml - Comprehensive security scanning

## ⚙️ Configuration
### Each template accepts parameters - check individual workflow files for available inputs and requirements.
