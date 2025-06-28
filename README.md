# Simple Apache Site

A basic Apache project for deploying a static site using GitHub Actions CI/CD.

## 🚀 GitHub Actions Workflows

This project includes three GitHub Actions workflows for comprehensive CI/CD:

### 1. `apache-deploy.yml` - Basic Deployment
- **Triggers**: Push/PR to main branch
- **Purpose**: Simple Apache deployment with basic testing
- **Features**:
  - Sets up Apache web server
  - Deploys static files
  - Tests deployment with curl
  - Validates Apache status

### 2. `advanced-deploy.yml` - Production-Ready CI/CD
- **Triggers**: Push to main/develop, manual workflow dispatch
- **Purpose**: Enterprise-grade deployment pipeline
- **Features**:
  - **Testing Stage**: HTML validation, file structure checks
  - **Staging Environment**: Deploy to staging with visual indicators
  - **Production Environment**: Secure deployment with:
    - Security headers configuration
    - Backup creation
    - Comprehensive testing
    - Deployment artifacts
    - Detailed deployment summaries

### 3. `dev-workflow.yml` - Development & Quality Assurance
- **Triggers**: Any branch push, PRs to main/develop
- **Purpose**: Code quality and development support
- **Features**:
  - HTML syntax validation
  - Web development best practices checking
  - Quick Apache functionality tests
  - Security scanning for common vulnerabilities

## 📁 Project Structure

```
.
├── .github/
│   └── workflows/
│       ├── apache-deploy.yml      # Basic deployment
│       ├── advanced-deploy.yml    # Production CI/CD
│       └── dev-workflow.yml       # Development QA
├── public-html/
│   ├── index.html                 # Main page
│   └── about.html                 # About page
├── instructions.md                # Setup instructions
└── README.md                      # This file
```

## 🔧 Workflow Features

- **Multi-environment support**: Staging and Production
- **Security-first**: Security headers, HTTPS recommendations
- **Quality assurance**: HTML validation, best practices checking
- **Artifact management**: Deployment packages with metadata
- **Comprehensive testing**: Functionality, security, and performance checks
- **Visual feedback**: Deployment summaries and status indicators
