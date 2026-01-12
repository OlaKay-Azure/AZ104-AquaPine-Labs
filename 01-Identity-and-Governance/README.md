# Domain 1: Manage Azure Identities and Governance

## 🎯 Domain Objectives

Implement secure identity management, role-based access control, and governance policies for AQUAPINE CONSULT's multi-site operations.

---

## 📋 Business Context

**Challenge**: AQUAPINE CONSULT had no structured identity management. Staff were sharing credentials, and there was no audit trail for access to production systems.

**Solution**: As the Azure Administrator, I designed and deployed:
- Microsoft Entra ID organizational structure
- Role-Based Access Control (RBAC) for departments
- Azure Policy for governance and compliance
- Resource tagging strategy for cost allocation

---

## 🏗️ Architecture Overview

### Identity Structure
**Naming Convention**: `AQUAPINE-[ROLE]-[LOCATION]`

**Security Groups Created**:
- `AQUAPINE-FarmManagers-Ibadan` (Production site managers)
- `AQUAPINE-MicrobiologyTeam-Ibadan` (Lab technicians)
- `AQUAPINE-SalesTeam-Lagos` (Sales and customer service)
- `AQUAPINE-HRDepartment-Lagos` (HR administrators)
- `AQUAPINE-ITAdministrators` (Cloud administrators)
- `AQUAPINE-ExternalConsultants` (Temporary contractor access)

### RBAC Implementation
| Group | Role | Scope | Rationale |
|-------|------|-------|-----------|
| Farm Managers | Reader | Production RG | View-only access to operational data |
| Sales Team | Contributor | Sales RG | Manage customer databases and analytics |
| IT Administrators | Owner | Subscription | Full administrative access |
| HR Department | Contributor | HR RG | Manage employee data (restricted access) |
| External Consultants | Reader | Specific RGs | Limited, auditable access |

### Governance Policies
- **Required Tags**: Environment, CostCenter, Owner, Department
- **Allowed Locations**: West Africa, South Africa North (data residency)
- **Naming Standards**: Enforced via Azure Policy
- **Allowed VM SKUs**: B-series, D-series (cost control)

---

## 📂 Repository Contents

### Scripts (`scripts/`)
PowerShell automation for identity and governance:
- `01-entra-id-setup.ps1` - User and group provisioning
- `02-rbac-assignment.ps1` - Role-based access control
- `03-policy-deployment.ps1` - Azure Policy deployment
- `04-tagging-strategy.ps1` - Resource tagging automation

### Templates (`templates/`)
Infrastructure as Code definitions:
- `policy-definitions/` - Custom Azure Policy rules
- `rbac-roles/` - Custom RBAC role definitions

### Documentation (`documentation/`)
Lab notes and architecture decisions:
- `lab-1.1-entra-id-setup.md` - Identity foundation lab
- `lab-1.2-rbac-configuration.md` - RBAC implementation
- `lab-1.3-governance-policies.md` - Policy deployment
- `architecture-decisions.md` - Design rationale

### Screenshots (`screenshots/`)
Validation and deployment evidence

### Outputs (`outputs/`)
Command outputs and validation logs

---

## 🚀 Labs Completed

### ✅ Lab 1.1: Microsoft Entra ID Setup
**Objective**: Create organizational identity structure

**What Was Built**:
- 6 security groups for departments and roles
- User provisioning automation
- MFA configuration for admin accounts
- Self-service password reset

**Key Learnings**:
- Microsoft Graph PowerShell for identity automation
- Difference between security groups and Microsoft 365 groups
- Best practices for naming conventions
- Audit logging configuration

---

### 🚧 Lab 1.2: RBAC Configuration (Planned)
**Objective**: Implement role-based access control

**Scope**:
- Assign roles to security groups
- Test least-privilege access
- Create custom RBAC roles if needed

---

### 📅 Lab 1.3: Azure Policy Deployment (Planned)
**Objective**: Enforce governance and compliance

**Scope**:
- Deploy tagging policies
- Implement naming standards
- Restrict resource types and locations
- Cost management policies

---

## 💡 Key Takeaways

### Technical Skills Demonstrated
✅ Microsoft Entra ID administration  
✅ PowerShell automation (Microsoft Graph)  
✅ Role-Based Access Control (RBAC)  
✅ Azure Policy as Code  
✅ Resource organization and tagging  
✅ Security best practices  

### Business Value Delivered
💼 **Security**: Eliminated shared credentials, implemented least-privilege access  
📊 **Compliance**: Audit trail for all identity changes  
💰 **Cost Control**: Tagged resources enable departmental cost allocation  
📈 **Scalability**: Automated provisioning supports business growth  

---

## 🎤 Interview Talking Points

> **"Tell me about a complex Azure project you've worked on."**
> 
> "At AQUAPINE CONSULT, I was hired as the Azure Administrator to establish their cloud infrastructure from scratch. One of my first priorities was implementing secure identity and governance. The company had no structured identity management—staff were sharing admin credentials, and there was no way to track who accessed what.
> 
> I designed a hierarchical identity structure in Microsoft Entra ID with six security groups aligned to their business units: farm operations in Ibadan, and office departments in Lagos. Using PowerShell and Microsoft Graph, I automated user provisioning to ensure consistency and created an audit trail for compliance.
> 
> I then implemented RBAC following the principle of least privilege. Farm managers got read-only access to production resources, while sales teams had contributor rights to their databases. IT administrators had full ownership. I deployed Azure Policy to enforce tagging standards across all resources, which enabled accurate cost allocation by department—critical for their budget-conscious environment.
> 
> The result was a secure, auditable, and cost-efficient identity foundation that supports their multi-site operations and scales as they grow."

---

## 📊 AZ-104 Exam Relevance

This domain covers **25-30%** of the AZ-104 exam:

**Key Exam Topics**:
- Manage Azure Active Directory (Entra ID) objects
- Configure RBAC (built-in and custom roles)
- Implement Azure Policy
- Manage subscriptions and governance
- Configure resource groups and tagging
- Analyze costs and create budgets

**Hands-On Skills Tested**:
- Create users and groups via Portal, PowerShell, CLI
- Assign RBAC roles at different scopes
- Create and assign Azure Policy definitions
- Implement and manage tags
- Configure management groups

---

## ✅ Domain Status

**Progress**: Lab 1.1 Complete | Labs 1.2-1.3 Planned  
**Completion**: [Your completion date]  
**Next Domain**: [02-Storage-Solutions](../02-Storage-Solutions/)

---

**Last Updated**: January 13, 2026