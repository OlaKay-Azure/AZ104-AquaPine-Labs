# AQUAPINE CONSULT - Azure Infrastructure Portfolio

> **Real-world Azure Administrator portfolio demonstrating end-to-end cloud infrastructure management for a multi-site aquaculture business.**

[![Azure](https://img.shields.io/badge/Azure-Administrator-0078D4?logo=microsoft-azure)](https://azure.microsoft.com)
[![PowerShell](https://img.shields.io/badge/PowerShell-7.x-5391FE?logo=powershell)](https://github.com/PowerShell/PowerShell)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Project Overview

This repository contains **production-ready Azure infrastructure code and documentation** created as part of my **Microsoft AZ-104 (Azure Administrator)** certification journey and hands-on cloud operations experience.

### Business Scenario

**AQUAPINE CONSULT** is an aquaculture farming and consulting business with:
- **2 production sites** (Ibadan, Nigeria) - Fish farms with microbiology labs, hatcheries, feed production
- **1 administrative office** (Lagos, Nigeria) - HR, IT, Sales, Logistics departments
- **Operational requirements**: Water quality monitoring, inventory management, secure HR data, sales analytics

**My Role**: Azure Administrator responsible for designing, deploying, and managing the complete Azure infrastructure from scratch.

---

## 🎯 Learning Objectives & Skills Demonstrated

### AZ-104 Domains Covered

| Domain | Topics | Status |
|--------|--------|--------|
| **Identity & Governance** | Entra ID, RBAC, Azure Policy, Resource Groups | 🚧 In Progress |
| **Storage Solutions** | Blob Storage, File Shares, Lifecycle Management | 📅 Planned |
| **Compute Resources** | Virtual Machines, Availability Sets, Scale Sets | 📅 Planned |
| **Virtual Networking** | VNets, NSGs, VPN Gateway, Load Balancers | 📅 Planned |
| **Monitoring & Backup** | Azure Monitor, Log Analytics, Backup Vaults | 📅 Planned |

### Technical Skills

- **Infrastructure as Code**: ARM Templates, Bicep, Terraform
- **Automation**: PowerShell 7, Azure CLI
- **Identity Management**: Microsoft Entra ID, RBAC, Conditional Access
- **Security**: Network Security Groups, Azure Policy, Key Vault
- **Monitoring**: Azure Monitor, Log Analytics Workspaces
- **Version Control**: Git, GitHub

---

## 🏗️ Architecture Highlights

**Multi-Site Design**
- Primary Region: West Africa (data residency compliance)
- Department-based resource segregation
- Role-based access control for farm vs. office users

**Security-First Approach**
- Least privilege access (RBAC)
- Network segmentation with NSGs
- Encrypted storage and secrets management
- Comprehensive audit logging

**Cost Optimization**
- Resource tagging for cost allocation
- Auto-shutdown policies for non-production resources
- Right-sized compute instances

---

## 📁 Repository Structure
```
AZ104-AquaPine-Labs/
│
├── 01-Identity-and-Governance/    # Domain 1 labs and scripts
├── 02-Storage-Solutions/          # Domain 2 labs and scripts
├── 03-Compute-Resources/          # Domain 3 labs and scripts
├── 04-Virtual-Networking/         # Domain 4 labs and scripts
├── 05-Monitoring-and-Backup/      # Domain 5 labs and scripts
├── docs/                          # Architecture docs, guides
├── learning-journal/              # Weekly progress notes
└── README.md                      # This file
```

Each domain folder contains:
- **scripts/**: PowerShell and Azure CLI automation
- **bicep/** or **terraform/**: Infrastructure as Code templates
- **documentation/**: Lab notes, architecture decisions
- **screenshots/**: Validation and deployment evidence

---

## 🚀 Quick Start

### Prerequisites
- Azure subscription (Azure for Students or Free Tier)
- PowerShell 7+
- Azure CLI 2.50+
- Visual Studio Code
- Git

### Deployment
```powershell
# Clone repository
git clone https://github.com/Olakay.azure/AZ104-AquaPine-Labs.git
cd AZ104-AquaPine-Labs

# Navigate to specific domain
cd 01-Identity-and-Governance/scripts

# Connect to Azure
Connect-AzAccount

# Run deployment script
./01-entra-id-setup.ps1
```

See individual domain READMEs for detailed instructions.

---

## 📊 Project Outcomes

✅ **Production-Ready Infrastructure**: All code tested and validated  
✅ **Comprehensive Documentation**: Architecture decisions, deployment guides, troubleshooting  
✅ **Automation-First**: Repeatable, scriptable deployments  
✅ **Real-World Scenarios**: Actual business requirements, not abstract demos  
✅ **Security & Compliance**: RBAC, encryption, audit logging  

---

## 🎓 Certifications & Learning

- **Microsoft Certified: Azure Administrator Associate (AZ-104)** - In Progress
- **Study Resources**: Microsoft Learn, O'Reilly Platform
- **Expected Completion**: [Month Year]

---

## 🤝 Connect With Me

- **GitHub**: [@Olakay.azure](https://github.com/Olakay.azure)
- **LinkedIn**: www.linkedin.com/in/olatunde-ogunti-22383b194
- **Location**: Lagos, Nigeria

---

## 📝 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Microsoft Learn AZ-104 Learning Path
- Azure documentation and best practices
- Real-world operational experience at AQUAPINE CONSULT

---

**⭐ If you find this repository helpful, please consider giving it a star!**

---

**Last Updated**: January 12, 2026