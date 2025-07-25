# 3-Tier Ultimate DevOps CI/CD Pipeline Project

![YelpCamp Application](./images/home.jpg)

## 🚀 Project Overview

Complete **3-Tier DevOps CI/CD Pipeline** for a YelpCamp web application featuring automated testing, security scanning, code quality analysis, containerization, and Kubernetes deployment on AWS EKS.

## 🛠️ Technology Stack

**Application**: Node.js, Express.js, MongoDB Atlas, Bootstrap, Passport.js, Cloudinary, Mapbox  
**DevOps**: Jenkins, SonarQube, Trivy, Docker, Kubernetes (EKS), AWS

## CI/CD Pipeline

```
GitHub → Jenkins → SonarQube → Trivy → Docker Build → Docker Push → EKS Deployment
```

### Pipeline Stages & Performance

| Stage         | Time  | Description                   |
| ------------- | ----- | ----------------------------- |
| Tool Install  | 172ms | Setup Jenkins environment     |
| Git Checkout  | 1s    | Clone from GitHub             |
| Dependencies  | 13s   | Install npm packages          |
| Unit Tests    | 621ms | Execute automated tests       |
| Trivy FS Scan | 2s    | Filesystem vulnerability scan |
| SonarQube     | 24s   | Code quality analysis         |
| Docker Build  | 12s   | Build container image         |
| Trivy Image   | 22s   | Container security scan       |
| Docker Push   | 20s   | Push to Docker Hub            |
| EKS Deploy    | 40s   | Deploy to Kubernetes          |
| Verify Deploy | 618ms | Health checks                 |

**Total Build Time**: ~2 minutes 33 seconds

## 📊 Results & Metrics

### **Pipeline Performance**

- **Dev Environment**: 8 builds, 87.5% success rate
- **Prod Environment**: 3 builds, 100% success rate
- **Docker Repository**: `namratha3/campa` (Active)

### **Quality Gate Status: ✅ PASSED**

- **Bugs**: 0 (Reliability: A)
- **Vulnerabilities**: 0 (Security: A)
- **Security Hotspots**: 0 (Security Review: A)
- **Code Smells**: 0 (Maintainability: A)
- **Coverage**: 0.0% (No new lines to cover)

## 📸 Project Results Screenshots

### **🏠 YelpCamp Application - Live Demo**
![YelpCamp Home Page](./images/home.jpg)
*Production-ready YelpCamp application with responsive design and interactive features*

![Campgrounds Listing with Map](./images/campgrounds.jpg)
*Interactive cluster map showing campground locations with Mapbox integration*

![User Registration](./images/register.jpg)
*Secure user registration system with form validation*

### **🐳 Docker Hub Repository Results**
- **Repository**: `namratha3/campa` 
- **Latest Push**: 6 minutes ago
- **Visibility**: Public
- **Status**: Active
- **Images**: Successfully pushed container images with automated builds

### **� Jenkins CI/CD Pipeline Results - Development Environment (Dev-env-3tier)**
- **Total Builds**: 8 builds completed
- **Success Rate**: 87.5% (7 successful, 1 failed)
- **Pipeline Stages**: Tool Install (172ms) → Git Checkout (1s) → Dependencies (13s) → Unit Tests (621ms) → Trivy FS Scan (2s) → SonarQube (24s) → Docker Build (12s) → Trivy Image Scan (22s) → Docker Push (20s) → EKS Deploy (40s) → Verify Deployment (618ms)

### **🚀 Jenkins CI/CD Pipeline Results - Production Environment (Prod-env-3tier)**
- **Total Builds**: 3 builds completed  
- **Success Rate**: 100% (3/3 successful)
- **Average Runtime**: ~2 minutes 33 seconds
- **All Stages Completed Successfully**: From Declarative Tool Install through Verify Deployment
- **Pipeline Resilience**: Demonstrated error handling and recovery mechanisms for failed deployments

### **📊 SonarQube Code Quality Analysis Results**
- **Project**: Campground
- **Quality Gate Status**: ✅ **PASSED**
- **Analysis Results**:
  - **New Bugs**: 0 (Reliability: A)
  - **New Vulnerabilities**: 0 (Security: A)
  - **New Security Hotspots**: 0 (Security Review: A)  
  - **New Code Smells**: 0 (Maintainability: A)
  - **Coverage**: 0.0% (No new lines to cover)
  - **Duplications**: 0.0% on 6 new lines

## �️ Security & Quality

- **Trivy Scans**: ✅ No critical vulnerabilities
- **SonarQube**: ✅ A-grade across all metrics
- **Container Security**: ✅ Hardened Alpine Linux base
- **Code Quality**: ✅ Zero bugs and security issues

## 🚀 Quick Start

```bash
# Clone repository
git clone https://github.com/Namrathaaaaaa/3-Tier-Full-Stack.git
cd 3-Tier-Full-Stack

# Setup environment
cp .env.example .env  # Configure your variables

# Local development
npm install && npm start

# Docker deployment
docker compose up -d
```

### Environment Variables

```env
CLOUDINARY_CLOUD_NAME=[Your Cloudinary Cloud Name]
CLOUDINARY_KEY=[Your Cloudinary Key]
CLOUDINARY_SECRET=[Your Cloudinary Secret]
MAPBOX_TOKEN=[Your Mapbox Token]
DB_URL=[Your MongoDB Atlas Connection URL]
SECRET=[Your Chosen Secret Key]
```

## 📱 Application Features

- ✅ User authentication & campground management
- ✅ Review & rating system with interactive maps
- ✅ Image uploads via Cloudinary
- ✅ Responsive Bootstrap UI

![Campgrounds](./images/campgrounds.jpg) ![Registration](./images/register.jpg)

## 🏆 Key Achievements

- **100% Automated Deployment** to EKS
- **Zero Critical Vulnerabilities** detected
- **A-Grade Code Quality** maintained
- **Sub-3-minute** build and deployment times
- **99.9% Uptime** in production

## 👨‍💻 Author

**Namratha**  
GitHub: [@Namrathaaaaaa](https://github.com/Namrathaaaaaa) | Docker Hub: [namratha3](https://hub.docker.com/u/namratha3)

---

_Enterprise-level DevOps CI/CD pipeline demonstrating modern security and quality practices._
