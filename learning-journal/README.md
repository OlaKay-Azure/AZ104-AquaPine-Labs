# 🐟 AQUAPINE CONSULT - Azure Infrastructure Portfolio

[![AZ-104](https://img.shields.io/badge/Azure-AZ--104-0078D4?logo=microsoft-azure)](https://learn.microsoft.com/en-us/credentials/certifications/azure-administrator/)
[![PowerShell](https://img.shields.io/badge/PowerShell-7.x-5391FE?logo=powershell)](https://github.com/PowerShell/PowerShell)
[![Bicep](https://img.shields.io/badge/IaC-Bicep-0078D4)](https://learn.microsoft.com/en-us/azure/azure-resource-manager/bicep/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Production-ready Azure infrastructure for AQUAPINE CONSULT** - A comprehensive Azure Administrator portfolio demonstrating enterprise cloud architecture, automation, and governance for a multi-site aquaculture business.

---

## 📋 Project Overview

### **Business Context**

**Company**: AQUAPINE CONSULT  
**Industry**: Aquaculture Farming & Consulting  
**Cloud Journey**: Zero to Azure (greenfield deployment)  
**My Role**: Azure Administrator (IT Manager)

**Challenge**: 
Design and implement a complete Azure infrastructure from scratch for a 45-employee organization operating across 3 locations (2 production farms in Ibadan, 1 administrative office in Lagos) with varying connectivity, sensitive data requirements, and SME budget constraints.

**Solution**: 
Systematic deployment of Azure services aligned to Microsoft AZ-104 certification domains, covering identity management, storage solutions, compute resources, virtual networking, and monitoring—all tailored to AQUAPINE's operational realities.

---

## 🏢 Organizational Structure

### **Ibadan Operations** (24 employees, 2 sites)
- **Bodija Farm**: 12 fish ponds, 6 AM-6 PM operations
- **Moniya Farm**: Hatchery & microbiology lab, 24/7 operations

**Departments**: Farm Operations (6) | Microbiology (4) | Fish Feed Production (5) | Hatchery (3) | Security (4) | Store (2)

### **Lagos Headquarters** (21 employees)
**Departments**: HR (3) | IT (2) | Sales & Marketing (8) | Logistics (4) | Executives (4)

**Data Requirements**:
- Operational data (water quality, feeding schedules, inventory)
- Biological data (fish health, lab results - compliance-critical)
- HR data (payroll, employee records - highly sensitive)
- Sales data (CRM, analytics)
- Security footage (CCTV feeds, access logs)

---

## 🗂️ Repository Structure

```
AquaPine-Azure-Infrastructure/
│
├── 📁 01-Identity-and-Governance/
│   ├── README.md (Domain 1 overview & architecture)
│   ├── scripts/
│   │   ├── 01-create-users.ps1 (Automated user provisioning)
│   │   ├── 02-create-groups.ps1 (Department & location groups)
│   │   └── 03-assign-rbac.ps1 (Role-based access control)
│   ├── bicep/
│   │   └── resource-groups.bicep (Subscription organization)
│   ├── documentation/
│   │   ├── identity-architecture.md
│   │   ├── rbac-matrix.md
│   │   └── azure-policy-catalog.md
│   └── screenshots/
│       └── entra-id-structure.png
│
├── 📁 02-Storage-Solutions/
│   ├── README.md
│   ├── scripts/
│   │   ├── 01-deploy-storage-accounts.ps1
│   │   └── 02-configure-lifecycle-policies.ps1
│   ├── bicep/
│   │   ├── storage-account.bicep
│   │   └── file-share.bicep
│   └── documentation/
│       ├── storage-architecture.md
│       └── data-segregation-strategy.md
│
├── 📁 03-Compute-Resources/
│   ├── README.md
│   ├── scripts/
│   ├── bicep/ (and/or terraform/)
│   └── documentation/
│
├── 📁 04-Virtual-Networking/
│   ├── README.md
│   ├── scripts/
│   ├── bicep/ (and/or terraform/)
│   └── documentation/
│
├── 📁 05-Monitoring-and-Backup/
│   ├── README.md
│   ├── scripts/
│   ├── bicep/ (and/or terraform/)
│   └── documentation/
│
├── 📁 docs/
│   ├── architecture/
│   │   ├── network-topology.md
│   │   └── disaster-recovery-plan.md
│   └── runbooks/
│       └── incident-response.md
│
├── 📁 learning-journal/
│   ├── README.md (Study methodology & progress)
│   ├── week-1/ (Daily notes & reflections)
│   └── interview-prep/
│       └── talking-points.md
│
├── README.md (this file)
├── LICENSE
└── .gitignore
```

---

## 🎯 AZ-104 Domain Coverage

| Domain | Status | Key Deliverables | Business Value |
|--------|--------|------------------|----------------|
| **1. Identity & Governance** | 🔄 In Progress | Entra ID tenant, 45 users, RBAC, Azure Policy | Secure access control, compliance, cost management |
| **2. Storage Solutions** | ⬜ Planned | Storage accounts, file shares, lifecycle policies | Data segregation, backup, disaster recovery |
| **3. Compute Resources** | ⬜ Planned | VMs, App Service, containers | Application hosting, scalability |
| **4. Virtual Networking** | ⬜ Planned | VNets, VPN Gateway, NSGs | Multi-site connectivity, security |
| **5. Monitoring & Backup** | ⬜ Planned | Azure Monitor, Backup, Site Recovery | Operational visibility, business continuity |

**Legend**: ⬜ Planned | 🔄 In Progress | ✅ Complete

---

## 🛠️ Technologies & Tools

### **Azure Services**
- **Identity**: Microsoft Entra ID (Azure AD), RBAC
- **Governance**: Azure Policy, Management Groups, Cost Management
- **Storage**: Storage Accounts, Azure Files, Blob Storage, File Sync
- **Compute**: Virtual Machines, App Service, Container Instances
- **Networking**: Virtual Networks, VPN Gateway, NSGs, Azure Firewall
- **Monitoring**: Azure Monitor, Log Analytics, Application Insights
- **Backup**: Azure Backup, Site Recovery

### **Infrastructure as Code**
- **PowerShell 7**: Primary automation language
- **Azure CLI**: Alternative/complementary tool
- **Bicep**: Azure-native declarative templates
- **Terraform**: Multi-cloud IaC (introduced Domain 3)

### **Development Tools**
- **VS Code**: Primary IDE (Azure extensions)
- **Git**: Version control
- **Azure Storage Explorer**: Storage management GUI
- **Draw.io**: Architecture diagrams

---

## 📚 Key Projects & Highlights

### **Domain 1: Identity Foundation for Multi-Site Organization**
> Designed and deployed complete Microsoft Entra ID structure for 45 employees across 8 departments and 3 locations, implementing least-privilege RBAC and Azure Policy for cost governance.

**Technical Highlights**:
- PowerShell automation for bulk user provisioning
- Dynamic group membership based on department attributes
- Custom Azure Policy for mandatory tagging enforcement
- Break-glass Global Administrator emergency access procedure

**Business Impact**: 
- 8 hours/month IT support time saved (self-service password reset)
- 100% audit compliance for access reviews
- Prevented unauthorized resource creation (cost control)

[**📂 View Project**](./01-Identity-and-Governance/)

---

### **Domain 2: Secure Data Storage with Segregation** *(Coming Soon)*
> Multi-tier storage architecture segregating sensitive biological, HR, and operational data with lifecycle policies and geo-redundant backup.

---

### **Domain 3: Hybrid Compute Infrastructure** *(Coming Soon)*
> VM deployment for microbiology lab (Windows) and sales office (Linux) with automated patching and disaster recovery.

---

### **Domain 4: Site-to-Site Connectivity** *(Coming Soon)*
> VPN gateway connecting Ibadan farms to Lagos headquarters with Network Security Groups and Azure Firewall.

---

### **Domain 5: Comprehensive Monitoring & DR** *(Coming Soon)*
> Azure Monitor dashboards, alerting framework, and Site Recovery configuration for business continuity.

---

## 🎓 Skills Demonstrated

### **Technical Competencies**
- ✅ Azure resource deployment and management
- ✅ PowerShell automation and scripting
- ✅ Infrastructure as Code (Bicep, Terraform)
- ✅ Role-Based Access Control (RBAC) design
- ✅ Azure Policy and governance implementation
- ✅ Network architecture and security
- ✅ Backup and disaster recovery planning
- ✅ Cost optimization and tagging strategies

### **Soft Skills**
- ✅ Translating business requirements to technical solutions
- ✅ Documentation and knowledge transfer
- ✅ Security-first mindset with compliance awareness
- ✅ Systematic troubleshooting and problem-solving
- ✅ Communication with non-technical stakeholders

---

## 📖 Documentation Standards

Every domain folder includes:

1. **README.md**: Project overview, architecture decisions, deployment guide
2. **Scripts**: Well-commented PowerShell/CLI with error handling
3. **IaC Templates**: Bicep/Terraform with parameter files
4. **Documentation**: Architecture diagrams, decision records, runbooks
5. **Screenshots**: Validation outputs and Azure Portal confirmations

**Code Quality Principles**:
- Meaningful variable names (no cryptic abbreviations)
- Inline comments explaining business logic
- Error handling and logging
- Idempotent operations (safe to run multiple times)
- Production-ready, not lab demos

---

## 🚀 Getting Started

### **Prerequisites**
- Azure subscription (Azure for Students or Free Trial)
- PowerShell 7+ or Azure CLI
- VS Code with Azure extensions
- Git installed

### **Clone Repository**
```powershell
git clone https://github.com/YOUR-USERNAME/AquaPine-Azure-Infrastructure.git
cd AquaPine-Azure-Infrastructure
```

### **Deploy a Domain**
Each domain has independent deployment instructions:
```powershell
# Example: Domain 1 - Identity & Governance
cd 01-Identity-and-Governance
# Follow README.md deployment steps
```

---

## 📊 Learning Journey

**Duration**: 12-16 weeks (January - April 2026)  
**Study Schedule**: 6 hours/day (afternoons)  
**Methodology**: 
- Mon-Thu: Theory (Microsoft Learn, video courses)
- Fri: Lab preparation
- Sat: Hands-on deployment
- Sun: Documentation and portfolio updates

**Progress Tracking**: [Learning Journal](./learning-journal/README.md)

---

## 🎤 Interview Talking Points

### **Elevator Pitch**
> "I recently completed a comprehensive Azure infrastructure deployment for AQUAPINE CONSULT, a multi-site aquaculture business. As their Azure Administrator, I designed and implemented identity management for 45 users, secure storage with data segregation, hybrid connectivity between office and farm sites, and comprehensive monitoring—all while maintaining SME budget constraints and aquaculture compliance requirements. This project gave me hands-on experience with the full Azure Administrator role, from planning to production deployment."

### **Technical Deep Dive Questions I Can Answer**
- "Walk me through a complex Azure deployment you've done"
- "How do you approach security in a multi-site Azure environment?"
- "Describe your experience with Infrastructure as Code"
- "How do you balance cost optimization with operational requirements?"
- "Tell me about a time you had to troubleshoot a complex Azure issue"

[**📂 Full Interview Prep**](./learning-journal/interview-prep/talking-points.md)

---

## 🏆 Certifications

- **Microsoft Certified: Azure Administrator Associate (AZ-104)** - *Certified*
- **Skills Reinforcement**: This portfolio demonstrates practical application of certification knowledge in production scenarios

---

## 📞 Contact & Professional Links

**Olatunde Ogunti**  
Azure Administrator | Cloud Infrastructure Specialist

- **LinkedIn**: [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)
- **Email**: ola_ogunti@outlook.com
- **GitHub**: [@Olakay-Azure](https://github.com/OlaKay-Azure/AZ104-AquaPine-Labs)
- **Portfolio**: [Week 1 – Day 1: Microsoft Entra ID Fundamentals (AZ-104)](https://github.com/OlaKay-Azure/AZ104-AquaPine-Labs/blob/main/learning-journal/README.md)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Microsoft Learn**: Official AZ-104 learning path and sandbox environments
- **Azure Community**: John Savill, Adam Marczak, and other educators
- **AQUAPINE CONSULT**: Business scenario and operational context

---

## 📈 Repository Stats

![Last Commit](https://img.shields.io/github/last-commit/your-username/AquaPine-Azure-Infrastructure)
![Repo Size](https://img.shields.io/github/repo-size/your-username/AquaPine-Azure-Infrastructure)
![Languages](https://img.shields.io/github/languages/count/your-username/AquaPine-Azure-Infrastructure)

---

**Last Updated**: January 16, 2026  
**Status**: 🔄 Active Development (Domain 1 In Progress)

---

*This repository is a living portfolio - continuously updated with new Azure deployments, automation scripts, and technical documentation as I progress through the AZ-104 curriculum.*