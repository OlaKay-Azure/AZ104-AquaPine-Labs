# AQUAPINE CONSULT - Azure Infrastructure Portfolio

> **Real-world Azure Administrator labs demonstrating enterprise cloud infrastructure deployment, governance, and management.**

[![AZ-104](https://img.shields.io/badge/AZ--104-Certified-0078D4?style=flat-square&logo=microsoft-azure)](https://learn.microsoft.com/certifications/azure-administrator/)
[![PowerShell](https://img.shields.io/badge/PowerShell-7-5391FE?style=flat-square&logo=powershell)](https://github.com/PowerShell/PowerShell)
[![Bicep](https://img.shields.io/badge/Bicep-IaC-0078D4?style=flat-square)](https://learn.microsoft.com/azure/azure-resource-manager/bicep/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

---

## 📋 Project Overview

This repository documents my work as an **Azure Administrator** designing and deploying cloud infrastructure for **AQUAPINE CONSULT**, a multi-site aquaculture operation transitioning from on-premises to Azure cloud services.

The project demonstrates real-world scenarios aligned with **Microsoft AZ-104 certification objectives**.

### What's Inside:

- ✅ **Identity and Governance** - Entra ID, RBAC, Azure Policy, Cost Management
- ✅ **Storage Solutions** - Blob storage, file shares, data protection
- ✅ **Compute Resources** - VMs, availability sets, autoscaling
- ✅ **Virtual Networking** - VNets, VPNs, NSGs, load balancing
- ✅ **Monitoring & Backup** - Azure Monitor, Log Analytics, Recovery Services

---

## 🏢 Business Scenario

**AQUAPINE CONSULT** operates:

### Ibadan (Production Sites - 2 Fish Farms)
- Farm Management
- Microbiology Department
- Fish Feed Production
- Hatchery Unit
- Security
- Store

### Lagos (Administrative Office)
- Human Resources
- IT Department
- Sales
- Logistics

### Cloud Requirements
- ✅ Secure multi-site connectivity
- ✅ Department-based access control
- ✅ Data protection and compliance
- ✅ Cost-optimized infrastructure
- ✅ Scalable and resilient architecture

---

## 🛠️ Technologies & Tools

| Category | Technologies |
|----------|-------------|
| **Cloud Platform** | Microsoft Azure |
| **Infrastructure as Code** | Bicep, ARM Templates |
| **Scripting** | PowerShell 7, Azure CLI |
| **Version Control** | Git, GitHub |
| **Development** | VS Code, Azure Cloud Shell |
| **Monitoring** | Azure Monitor, Log Analytics |
| **Security** | Entra ID, Key Vault, Azure Policy, RBAC |

---

## 📂 Repository Structure
```
AZ104-AquaPine-Labs/
├── 01-Identity-and-Governance/      # Entra ID, RBAC, Azure Policy
├── 02-Storage-Solutions/            # Storage accounts, data protection
├── 03-Compute-Resources/            # VMs, scaling, availability
├── 04-Virtual-Networking/           # VNets, VPN, security groups
├── 05-Monitoring-and-Backup/        # Azure Monitor, backup strategies
├── Architecture-Diagrams/           # Visual infrastructure designs
├── Scripts/                         # Reusable automation scripts
└── Documentation/                   # Guides and best practices
```

Each lab includes:
- 📖 **README** with business context and objectives
- 💻 **Scripts** (PowerShell/CLI) for deployment
- 📋 **Templates** (Bicep/ARM) for infrastructure as code
- ✅ **Validation** steps and expected outputs
- 🎯 **AZ-104 exam relevance** notes

---

## 🚀 Getting Started

### Prerequisites
- Azure subscription (Free tier or Azure for Students)
- PowerShell 7+
- Azure CLI
- VS Code
- Git

### Quick Start

1. **Clone the repository**
```bash
   git clone https://github.com/OlaKay-azure/AZ104-AquaPine-Labs.git
   cd AZ104-AquaPine-Labs
```

2. **Connect to Azure**
```powershell
   Connect-AzAccount
```

3. **Navigate to a lab and follow the README**
```bash
   cd 01-Identity-and-Governance/Lab-1.1-Environment-Setup
   Each lab contains detailed instructions, scripts, and validation steps.
```

---

## 📚 Learning Path

| Domain | Status | Key Topics |
|--------|--------|------------|
| **1. Identity & Governance** | 🚧 In Progress | Entra ID, RBAC, Policies |
| **2. Storage Solutions** | 📅 Planned | Blob, Files, Backup |
| **3. Compute Resources** | 📅 Planned | VMs, Containers, App Services |
| **4. Virtual Networking** | 📅 Planned | VNets, VPN, Load Balancers |
| **5. Monitoring & Backup** | 📅 Planned | Azure Monitor, Disaster Recovery |

---

## 🎯 Key Achievements

- ✅ Designed multi-site identity architecture with department-based RBAC
- ✅ Implemented Azure Policy for governance and compliance
- ✅ Automated infrastructure deployment using Bicep templates
- ✅ Established cost management and budget alerts
- ✅ Documented all deployments with enterprise-grade READMEs

---

## 🎯 Skills Demonstrated

### Azure Administration
- Identity and access management (Entra ID)
- Role-based access control (RBAC)
- Resource organization and governance
- Cost management and optimization
- Policy enforcement and compliance

### Infrastructure as Code
- Bicep template development
- ARM template deployment
- Parameterized, reusable templates
- Version-controlled infrastructure

### Automation & Scripting
- PowerShell automation
- Azure CLI scripting
- Deployment automation
- Operational runbooks

### Documentation
- Technical writing
- Architecture diagrams
- Deployment guides
- Troubleshooting documentation

---

## 🏆 Certifications

**Microsoft Certified: Azure Administrator Associate (AZ-104)**  
Issued: October, 2024

---

## 📞 +2348169283961

**Olatunde Ogunti**  
Azure Administrator | Cloud Infrastructure Specialist  

📧 Email: ola_ogunti@outlook.com  
💼 LinkedIn: [www.linkedin.com/in/olatunde-ogunti-22383b194]  

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Microsoft Learn documentation
- Azure community contributions
- Real-world enterprise architecture patterns

---

*Built with ☁️ by an Azure Administrator passionate about cloud infrastructure*

**Last Updated:** January 2026
```
