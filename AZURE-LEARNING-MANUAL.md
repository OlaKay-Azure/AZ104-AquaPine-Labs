# AZURE ADMINISTRATOR LEARNING MANUAL
## Your Personal Roadmap to AZ-104 Certification & Portfolio Excellence

**Version**: 2.0  
**Program Duration**: 12-16 weeks  
**Study Commitment**: 15-20 hours/week  
**Outcome**: AZ-104 certified + Portfolio-ready for employment

---

## TABLE OF CONTENTS

1. [Program Overview](#program-overview)
2. [Pre-Flight Checklist](#pre-flight-checklist)
3. [Weekly Study Rhythm](#weekly-study-rhythm)
4. [Daily Routines & Templates](#daily-routines--templates)
5. [Domain-by-Domain Roadmap](#domain-by-domain-roadmap)
6. [Tools Setup Guide](#tools-setup-guide)
7. [GitHub Workflow Guide](#github-workflow-guide)
8. [Study Resources Index](#study-resources-index)
9. [Troubleshooting & FAQ](#troubleshooting--faq)
10. [Progress Tracking](#progress-tracking)

---

## PROGRAM OVERVIEW

### Your Journey at a Glance

```
Week 1-3:   Domain 1 - Identity & Governance
Week 4-6:   Domain 2 - Storage Solutions  
Week 7-9:   Domain 3 - Compute Resources
Week 10-12: Domain 4 - Virtual Networking
Week 13-15: Domain 5 - Monitoring & Backup
Week 16:    Final Portfolio Polish + Exam Prep
```

### Weekly Time Allocation

| Day | Focus | Hours | Activities |
|-----|-------|-------|------------|
| **Monday** | Theory | 2-3 hrs | Microsoft Learn modules, O'Reilly videos |
| **Tuesday** | Theory | 2-3 hrs | Microsoft Learn modules, O'Reilly videos |
| **Wednesday** | Theory | 2-3 hrs | Microsoft Learn modules, note-taking |
| **Thursday** | Theory | 2-3 hrs | Review, flashcards, prep questions |
| **Friday** | Lab Prep | 3-4 hrs | Environment setup, initial coding |
| **Saturday** | Labs | 4-6 hrs | Hands-on deployment and testing |
| **Sunday** | Documentation | 4-6 hrs | GitHub upload, documentation, LinkedIn |

**Total**: 20-25 hours/week (flexible based on your pace)

---

## PRE-FLIGHT CHECKLIST

### ☐ PHASE 1: Account Setup (Week 0)

**Microsoft Accounts**:
- [ ] Create Microsoft account (if needed)
- [ ] Activate Azure for Students subscription
  - Navigate to: https://azure.microsoft.com/en-us/free/students/
  - Verify with school email
  - Confirm $100 credit activated
- [ ] Enroll in Microsoft Learn
  - Profile: https://learn.microsoft.com/users/[yourname]
  - Start AZ-104 learning path

**O'Reilly Access**:
- [ ] Confirm O'Reilly account access
- [ ] Bookmark AZ-104 resources:
  - "Microsoft Azure Administrator (AZ-104)" by Scott Duffy
  - "Exam Ref AZ-104" by Michael Washam
  - Azure documentation portal

**GitHub Setup**:
- [ ] Create GitHub account (professional username)
- [ ] Set up profile (photo, bio, location)
- [ ] Create profile README repository (optional)
- [ ] Create main repository: `AquaPine-Azure-Infrastructure`
- [ ] Initialize with README, .gitignore, LICENSE

**LinkedIn Optimization**:
- [ ] Update headline: "Azure Administrator | AZ-104 Candidate"
- [ ] Add "Microsoft Azure" to skills
- [ ] Connect with Azure community (10-20 professionals)
- [ ] Plan weekly progress post template

---

### ☐ PHASE 2: Tools Installation (Week 0)

**Download & Install**:

1. **Visual Studio Code**
   - [ ] Download: https://code.visualstudio.com
   - [ ] Install Extensions:
     - Azure Account
     - Azure Resources
     - Azure Storage
     - PowerShell
     - Bicep
     - GitLens
     - Terraform (install later in Domain 3)

2. **PowerShell 7**
   - [ ] Download: https://github.com/PowerShell/PowerShell/releases
   - [ ] Verify installation: `pwsh --version`
   - [ ] Install Azure modules:
     ```powershell
     Install-Module -Name Az -Repository PSGallery -Force
     Install-Module -Name Microsoft.Graph -Force
     ```

3. **Azure CLI**
   - [ ] Download: https://docs.microsoft.com/cli/azure/install-azure-cli
   - [ ] Verify installation: `az --version`
   - [ ] Login: `az login`

4. **Git**
   - [ ] Download: https://git-scm.com/downloads
   - [ ] Configure:
     ```bash
     git config --global user.name "Your Name"
     git config --global user.email "your.email@example.com"
     ```

5. **Azure Storage Explorer**
   - [ ] Download: https://azure.microsoft.com/features/storage-explorer
   - [ ] Connect to Azure subscription

6. **Optional Tools**:
   - [ ] GitHub Desktop (if you prefer GUI)
   - [ ] Draw.io Desktop (for diagrams)

---

### ☐ PHASE 3: Repository Initialization (Week 0)

**Create Local Structure**:

```bash
# Create project folder
mkdir AquaPine-Azure-Infrastructure
cd AquaPine-Azure-Infrastructure

# Initialize Git
git init

# Create folder structure
mkdir -p 01-Identity-and-Governance/{scripts,templates,documentation,screenshots}
mkdir -p 02-Storage-Solutions/{scripts,bicep,documentation,screenshots}
mkdir -p 03-Compute-Resources/{scripts,bicep,terraform,documentation,screenshots}
mkdir -p 04-Virtual-Networking/{scripts,bicep,terraform,documentation,diagrams}
mkdir -p 05-Monitoring-and-Backup/{scripts,bicep,documentation,screenshots}
mkdir -p docs learning-journal

# Create initial files
touch README.md .gitignore LICENSE
touch docs/{architecture-overview.md,deployment-guide.md,troubleshooting.md,interview-talking-points.md}

# Create learning journal structure
mkdir -p learning-journal/{week-01,week-02,week-03,week-04}

# Initial commit
git add .
git commit -m "chore: initialize Azure Administrator portfolio structure"

# Connect to GitHub (after creating remote repo)
git remote add origin https://github.com/[your-username]/AquaPine-Azure-Infrastructure.git
git branch -M main
git push -u origin main
```

**Verify Setup**:
- [ ] All folders created
- [ ] Git tracking active
- [ ] Pushed to GitHub successfully
- [ ] Repository visible on your GitHub profile

---

## WEEKLY STUDY RHYTHM

### MONDAY - THURSDAY: Theory Mastery

#### **MONDAY ROUTINE** (2-3 hours)

**Morning Session** (90 minutes):
```
08:00 - 09:30 | Microsoft Learn Module 1
             ├─ Read content carefully
             ├─ Complete knowledge checks
             ├─ Take notes in markdown
             └─ Bookmark unclear concepts
```

**Afternoon Session** (60-90 minutes):
```
14:00 - 15:30 | O'Reilly Video Course
             ├─ Watch 1-2 chapters
             ├─ Pause to understand complex topics
             ├─ Note timestamps for review
             └─ Compare with Microsoft Learn content
```

**Evening Wrap-up** (15 minutes):
```
20:00 - 20:15 | Journal Entry
             ├─ Create: learning-journal/week-X/monday.md
             ├─ Summarize key learnings
             ├─ List questions for instructor
             └─ Plan tomorrow's focus
```

---

#### **TUESDAY ROUTINE** (2-3 hours)

**Same structure as Monday**:
- Microsoft Learn: Continue modules
- O'Reilly: Next chapters
- Note-taking: Expand on unclear Monday concepts

**Additional Activity** (30 minutes):
```
Flashcard Creation (using Notion, Anki, or markdown)
├─ Key terms and definitions
├─ Service comparisons (e.g., Blob vs. File Storage)
├─ Exam-likely facts
└─ PowerShell cmdlets
```

---

#### **WEDNESDAY ROUTINE** (2-3 hours)

**Morning Session** (90 minutes):
- Finish Microsoft Learn modules for the topic
- Complete all knowledge checks
- Review flagged concepts from Mon-Tue

**Afternoon Session** (90 minutes):
- O'Reilly: Complete video chapters
- Read supplementary blog posts or docs
- Start connecting theory to AQUAPINE scenarios

**Evening**:
- Update learning journal
- Begin drafting lab questions

---

#### **THURSDAY ROUTINE** (2-3 hours)

**Active Recall Day** - No new content

**Morning** (90 minutes):
```
Self-Testing Session
├─ Review flashcards
├─ Explain concepts aloud (record yourself)
├─ Quiz yourself on key facts
└─ Identify weak areas
```

**Afternoon** (90 minutes):
```
Lab Preparation
├─ Review upcoming lab requirements
├─ Read lab instructions from instructor (Claude)
├─ List required Azure resources
├─ Draft initial PowerShell/CLI commands
└─ Prepare questions for Friday
```

**Evening** (30 minutes):
```
Weekly Check-In with Instructor
├─ Post questions to Claude
├─ Clarify any confusion
├─ Confirm lab readiness
└─ Get Friday lab brief
```

---

### FRIDAY: Lab Preparation Day

#### **FRIDAY ROUTINE** (3-4 hours)

**Morning Session** (2 hours):
```
09:00 - 11:00 | Environment Setup
             ├─ Login to Azure Portal
             ├─ Verify subscription credits
             ├─ Create resource group for lab
             ├─ Set up VS Code workspace
             └─ Test Azure connections (CLI, PowerShell)
```

**Afternoon Session** (2 hours):
```
13:00 - 15:00 | Initial Coding
             ├─ Create script files
             ├─ Write parameter sections
             ├─ Add error handling structure
             ├─ Test individual commands
             └─ Commit initial code to Git
```

**Key Deliverables by EOD Friday**:
- [ ] Azure environment ready
- [ ] Script scaffolding complete
- [ ] Git repository updated
- [ ] Clear plan for Saturday implementation

---

### SATURDAY: Implementation Day

#### **SATURDAY ROUTINE** (4-6 hours)

**Morning Session** (2-3 hours):
```
09:00 - 12:00 | Deployment Phase
             ├─ Execute scripts step-by-step
             ├─ Deploy Bicep/Terraform templates
             ├─ Validate each resource creation
             ├─ Troubleshoot errors immediately
             └─ Document issues and solutions
```

**Lunch Break** (1 hour):
- Review progress
- Adjust afternoon plan if needed

**Afternoon Session** (2-3 hours):
```
13:00 - 16:00 | Testing & Validation
             ├─ Run all validation commands
             ├─ Test access and permissions
             ├─ Capture screenshots
             ├─ Verify against acceptance criteria
             └─ Refine code based on testing
```

**Evening** (1 hour):
```
18:00 - 19:00 | Code Review Prep
             ├─ Self-review for quality
             ├─ Add missing error handling
             ├─ Improve comments
             ├─ Format code consistently
             └─ Request instructor review
```

**Saturday Deliverables**:
- [ ] All infrastructure deployed
- [ ] Validation complete
- [ ] Screenshots captured
- [ ] Code ready for review

---

### SUNDAY: Documentation & Publishing Day

#### **SUNDAY ROUTINE** (4-6 hours)

**Morning Session** (2-3 hours):
```
09:00 - 12:00 | Technical Documentation
             ├─ Write domain README.md
             ├─ Document architecture decisions
             ├─ Create deployment guide
             ├─ Write troubleshooting notes
             └─ Generate/refine diagrams
```

**Afternoon Session** (2-3 hours):
```
13:00 - 16:00 | GitHub Publishing
             ├─ Organize files properly
             ├─ Review .gitignore (no secrets!)
             ├─ Write professional commit messages
             ├─ Push to GitHub
             ├─ Update main README
             └─ Verify all links work
```

**Evening Session** (1 hour):
```
18:00 - 19:00 | Professional Development
             ├─ Draft LinkedIn post
             ├─ Update interview talking points
             ├─ Write weekly reflection
             ├─ Plan next week's study
             └─ Celebrate wins! 🎉
```

**Sunday Deliverables**:
- [ ] Complete domain folder on GitHub
- [ ] Professional README files
- [ ] LinkedIn post (optional)
- [ ] Learning journal updated
- [ ] Next week planned

---

## DAILY ROUTINES & TEMPLATES

### Daily Learning Journal Template

**File**: `learning-journal/week-X/[day].md`

```markdown
# Week X - [Day] - [Date]

## 📚 Study Session

**Duration**: [X hours]

**Resources Used**:
- [ ] Microsoft Learn: [Module name]
- [ ] O'Reilly: [Video chapter]
- [ ] Azure Docs: [Specific articles]

## 🎯 Topics Covered

1. **[Topic 1]**
   - Key concept: [Brief note]
   - AQUAPINE context: [How it applies]
   - Exam relevance: [Why it matters]

2. **[Topic 2]**
   - [Same structure]

## 💡 Key Takeaways

- [Most important insight 1]
- [Most important insight 2]
- [Most important insight 3]

## ❓ Questions & Confusion

- [ ] [Concept I don't fully understand]
- [ ] [Need clarification on...]
- [ ] [Want to explore deeper...]

## ✅ Action Items

- [ ] [Tomorrow's focus]
- [ ] [Practice needed for...]
- [ ] [Review this concept again]

## 🧠 Flashcards Created

- [Term]: [Definition]
- [Cmdlet]: [Purpose and syntax]

## 📊 Progress

- Microsoft Learn completion: [X%]
- O'Reilly chapters: [X/Y]
- Confidence level: [1-10]

---

**Tomorrow's Goal**: [Specific objective]
```

---

### Weekly Reflection Template

**File**: `learning-journal/week-X/weekly-reflection.md`

```markdown
# Week X Reflection - [Date Range]

## 🎯 Week's Objective

**Planned**: [What you aimed to accomplish]  
**Actual**: [What you actually achieved]

## 📈 Progress Summary

### Theory (Mon-Thu)
- Microsoft Learn modules completed: [X]
- O'Reilly chapters watched: [X]
- Study hours: [X]
- Knowledge retention: [Self-assessment 1-10]

### Labs (Fri-Sun)
- Labs completed: [List]
- GitHub commits: [Count]
- Code quality: [Self-assessment 1-10]
- Challenges overcome: [Brief list]

## 💪 Wins This Week

1. [Specific accomplishment]
2. [Technical skill mastered]
3. [Problem solved independently]

## 🚧 Challenges Faced

| Challenge | How I Addressed It | Outcome |
|-----------|-------------------|---------|
| [Problem] | [Solution tried] | [Result] |

## 📚 Technical Skills Gained

**New Azure Services Learned**:
- [Service 1]: [What you can do with it]
- [Service 2]: [What you can do with it]

**PowerShell/CLI Skills**:
- [New cmdlets/commands learned]
- [Scripting patterns understood]

**IaC Progress**:
- [Bicep/Terraform concepts]

## 🎤 Interview Talking Points Added

```
"At AQUAPINE CONSULT, I [specific action taken this week] which resulted in [business outcome]. I used [technologies] and made [key decision] because [reasoning]."
```

## 📊 Portfolio Status

- [ ] GitHub updated with this week's work
- [ ] README files professional quality
- [ ] Documentation complete
- [ ] LinkedIn post published (optional)

## 🎯 Next Week's Goals

### Learning Objectives
1. [Specific topic to master]
2. [Specific skill to develop]
3. [Specific lab to complete]

### Portfolio Goals
- [ ] [Documentation improvement]
- [ ] [Code refactoring needed]
- [ ] [Diagram to create]

## 🤔 Questions for Instructor

- [ ] [Technical question]
- [ ] [Career advice needed]
- [ ] [Study strategy check]

## ⏰ Time Management

**Total hours this week**: [X]  
**Most productive time**: [Morning/Afternoon/Evening]  
**Adjustment needed**: [Any schedule changes]

---

**Overall Feeling**: [Confident/Overwhelmed/On-track]  
**Motivation Level**: [1-10]  
**Ready for next week**: [Yes/No - why?]
```

---

## DOMAIN-BY-DOMAIN ROADMAP

### DOMAIN 1: Manage Azure Identities and Governance
**Duration**: 2-3 weeks | **Exam Weight**: 25-30%

#### Week 1: Identity Foundation

**Mon-Thu Theory**:
- Microsoft Entra ID (Azure AD) architecture
- Users, groups, administrative units
- Self-service password reset
- Multi-factor authentication

**Fri-Sun Labs**:
- Lab 1.1: Create AQUAPINE organizational structure
- Lab 1.2: Configure RBAC for departments
- Lab 1.3: Implement MFA for admin accounts

**Portfolio Deliverable**:
- PowerShell scripts for user/group provisioning
- RBAC assignment documentation
- Identity architecture diagram

---

#### Week 2: Governance & Management

**Mon-Thu Theory**:
- Subscriptions and management groups
- Azure Policy
- Resource groups and tagging
- Cost Management + Billing

**Fri-Sun Labs**:
- Lab 1.4: Create resource organization structure
- Lab 1.5: Deploy Azure Policy for compliance
- Lab 1.6: Implement cost tracking with tags

**Portfolio Deliverable**:
- Governance policy templates
- Tagging strategy document
- Cost allocation reports

---

#### Week 3: Domain 1 Capstone

**Capstone Project**:
> "Design and deploy complete identity and governance structure for AQUAPINE CONSULT, including all departments (Ibadan farms + Lagos office), RBAC assignments, Azure Policy enforcement, and cost management tags."

**Requirements**:
- [ ] 10+ users across all departments
- [ ] 6+ security groups (department-based)
- [ ] RBAC assignments (Contributor, Reader, custom roles)
- [ ] 3+ Azure Policies (naming, allowed resources, required tags)
- [ ] Tagging strategy implemented
- [ ] Cost allocation dashboard
- [ ] Complete documentation with diagrams

**Instructor Review**: Submit for review before proceeding

---

### DOMAIN 2: Implement and Manage Storage
**Duration**: 2-3 weeks | **Exam Weight**: 15-20%

#### Week 4: Storage Fundamentals

**Mon-Thu Theory**:
- Storage account types
- Blob storage (Hot, Cool, Archive)
- Azure Files and File Sync
- Storage security and networking

**Fri-Sun Labs**:
- Lab 2.1: Deploy storage accounts for different data types
- Lab 2.2: Configure blob lifecycle management
- Lab 2.3: Set up Azure Files for file sharing
- **NEW**: First Bicep template

**Portfolio Deliverable**:
- PowerShell + Bicep templates for storage
- Data classification strategy
- Storage access documentation

---

#### Week 5: Storage Security & Optimization

**Mon-Thu Theory**:
- Storage encryption
- Shared Access Signatures (SAS)
- Storage firewalls and private endpoints
- Azure Backup for storage

**Fri-Sun Labs**:
- Lab 2.4: Implement storage security layers
- Lab 2.5: Configure storage replication
- Lab 2.6: Set up Azure Backup for file shares

---

#### Week 6: Domain 2 Capstone

**Capstone Project**:
> "Implement comprehensive storage solution for AQUAPINE CONSULT with data segregation (farm operations, HR records, sales analytics), appropriate access controls, lifecycle policies, and backup."

**Requirements**:
- [ ] 3+ storage accounts (segregated by data type)
- [ ] Blob lifecycle policies (Hot→Cool→Archive)
- [ ] Azure Files for department file sharing
- [ ] Private endpoints for HR data
- [ ] SAS tokens for external consultant access
- [ ] Backup configuration
- [ ] Complete Bicep template
- [ ] Cost optimization analysis

---

### DOMAIN 3: Deploy and Manage Azure Compute
**Duration**: 3-4 weeks | **Exam Weight**: 20-25%

#### Week 7: Virtual Machines

**Mon-Thu Theory**:
- VM sizes and series
- Availability sets and zones
- VM extensions and custom script
- Azure Bastion

**Fri-Sun Labs**:
- Lab 3.1: Deploy Windows VM (for microbiology lab)
- Lab 3.2: Deploy Linux VM (for sales office)
- Lab 3.3: Configure availability set
- **NEW**: First Terraform template (parallel to Bicep)

**Portfolio Deliverable**:
- VM deployment scripts (PowerShell + Bicep + Terraform)
- Sizing decision matrix
- Remote access configuration

---

#### Week 8: VM Management & Containers

**Mon-Thu Theory**:
- VM backup and restore
- Azure Update Management
- Azure Container Instances
- Azure Kubernetes Service (AKS) basics

**Fri-Sun Labs**:
- Lab 3.4: Configure VM backup
- Lab 3.5: Automate VM patching
- Lab 3.6: Deploy simple container (optional)

---

#### Week 9: App Service & Automation

**Mon-Thu Theory**:
- Azure App Service plans
- Web Apps deployment
- VM automation and desired state

**Fri-Sun Labs**:
- Lab 3.7: Deploy web app for sales portal
- Lab 3.8: Configure auto-scaling

---

#### Week 10: Domain 3 Capstone

**Capstone Project**:
> "Deploy VM infrastructure for AQUAPINE CONSULT: Windows VM for microbiology lab, Linux VMs for sales office, including availability, backup, patch management, and remote access configuration."

**Requirements**:
- [ ] Windows Server VM (microbiology department)
- [ ] 2x Linux VMs (sales office - load balanced)
- [ ] Availability set configuration
- [ ] Azure Backup configured
- [ ] Patch management automated
- [ ] Azure Bastion for secure access
- [ ] Both Bicep AND Terraform templates
- [ ] Cost comparison: IaC approaches
- [ ] Runbook documentation

---

### DOMAIN 4: Configure and Manage Virtual Networking
**Duration**: 2-3 weeks | **Exam Weight**: 20-25%

#### Week 11: Network Foundation

**Mon-Thu Theory**:
- Virtual Networks and subnets
- IP addressing (public and private)
- Network Security Groups
- Azure Firewall

**Fri-Sun Labs**:
- Lab 4.1: Design network topology for AQUAPINE
- Lab 4.2: Deploy VNets for Ibadan and Lagos
- Lab 4.3: Configure NSG rules

**Portfolio Deliverable**:
- Network architecture diagram
- IP addressing scheme
- NSG rule documentation

---

#### Week 12: Network Connectivity

**Mon-Thu Theory**:
- VNet peering
- VPN Gateway
- ExpressRoute
- Azure DNS and Load Balancer

**Fri-Sun Labs**:
- Lab 4.4: Configure VNet peering
- Lab 4.5: Set up VPN gateway (site-to-site simulation)
- Lab 4.6: Deploy Azure Load Balancer

---

#### Week 13: Domain 4 Capstone

**Capstone Project**:
> "Design and implement secure network connectivity between Ibadan farms and Lagos office, including VNet peering, NSG rules, and site-to-site VPN simulation."

**Requirements**:
- [ ] 2 VNets (Ibadan, Lagos)
- [ ] Subnet segmentation by department
- [ ] VNet peering configured
- [ ] NSG rules (allow/deny traffic)
- [ ] VPN Gateway (or simulation)
- [ ] Azure Firewall (optional)
- [ ] Network topology diagram
- [ ] IaC templates (Bicep or Terraform)
- [ ] Troubleshooting runbook

---

### DOMAIN 5: Monitor and Back Up Azure Resources
**Duration**: 2-3 weeks | **Exam Weight**: 10-15%

#### Week 14: Monitoring

**Mon-Thu Theory**:
- Azure Monitor architecture
- Log Analytics workspace
- Application Insights
- Alerts and action groups

**Fri-Sun Labs**:
- Lab 5.1: Set up Log Analytics
- Lab 5.2: Configure VM monitoring
- Lab 5.3: Create alert rules

---

#### Week 15: Backup & Recovery

**Mon-Thu Theory**:
- Azure Backup architecture
- Recovery Services vault
- Azure Site Recovery
- Backup policies and retention

**Fri-Sun Labs**:
- Lab 5.4: Configure Azure Backup for VMs
- Lab 5.5: Test backup and restore
- Lab 5.6: Set up Site Recovery (optional)

---

#### Week 16: Domain 5 Capstone + Final Portfolio Polish

**Capstone Project**:
> "Implement comprehensive monitoring and backup strategy for all AQUAPINE Azure resources with alerting, dashboards, and disaster recovery plan."

**Requirements**:
- [ ] Log Analytics workspace collecting all logs
- [ ] VM performance monitoring
- [ ] Storage account metrics
- [ ] Custom dashboards
- [ ] Alert rules for critical issues
- [ ] Backup configured for all VMs
- [ ] Backup tested and validated
- [ ] Disaster recovery runbook
- [ ] Complete documentation

**Final Portfolio Tasks**:
- [ ] Audit all GitHub repositories
- [ ] Update main README with all domains
- [ ] Create architecture overview diagram
- [ ] Polish all documentation
- [ ] Create interview talking points summary
- [ ] Practice explaining your work (record yourself)
- [ ] LinkedIn profile final update
- [ ] Schedule AZ-104 exam

---

## TOOLS SETUP GUIDE

### Visual Studio Code Configuration

**Essential Extensions**:
```
code --install-extension ms-vscode.azure-account
code --install-extension ms-azuretools.vscode-azureresourcegroups
code --install-extension ms-azuretools.vscode-azurestorage
code --install-extension ms-vscode.powershell
code --install-extension ms-azuretools.vscode-bicep
code --install-extension eamodio.gitlens
code --install-extension hashicorp.terraform (Domain 3+)
```

**Recommended Settings** (`settings.json`):
```json
{
  "editor.formatOnSave": true,
  "editor.rulers": [80, 120],
  "files.autoSave": "afterDelay",
  "powershell.codeFormatting.preset": "OTBS",
  "git.autofetch": true,
  "azure.resourceGroups.groupBy": "resourceType"
}
```

---

### PowerShell Profile Setup

**Create PowerShell profile** (`$PROFILE`):
```powershell
# Azure Administrator Profile

# Import Azure modules
Import-Module Az
Import-Module Microsoft.Graph

# Helpful aliases
Set-Alias -Name k -Value kubectl  # Domain 3+
Set-Alias -Name tf -Value terraform  # Domain 3+

# Custom functions
function Connect-AquaPineAzure {
    Connect-AzAccount -Subscription "Azure for Students"
    Set-AzContext -Subscription "Azure for Students"
    Write-Host "✅ Connected to AQUAPINE Azure subscription" -ForegroundColor Green
}

# Welcome message
Write-Host "🐟 AQUAPINE Azure Administrator Environment Ready" -ForegroundColor Cyan
Write-Host "Run 'Connect-AquaPineAzure' to start" -ForegroundColor Yellow
```

---

## GITHUB WORKFLOW GUIDE

### Daily Git Workflow

```bash
# Start of day: Pull latest
git pull origin main

# Create feature branch (optional, for complex work)
git checkout -b feat/storage-account-deployment

# Work on your files...

# Stage changes
git add .

# Commit with meaningful message
git commit -m "feat: implement blob storage lifecycle for AQUAPINE farm data"

# Push to GitHub
git push origin main  # or your feature branch
```

---

### Commit Message Standards

Use **Conventional Commits** format:

```
<type>: <description>

[optional body]
[optional footer]
```

**Types**:
- `feat`: New feature or lab
- `fix`: Bug fix or correction
- `docs`: Documentation only
- `refactor`: Code improvement (no functionality change)
- `test`: Adding validation or tests
- `chore`: Maintenance tasks

**Examples**:
```bash
git commit -m "feat: implement Entra ID user provisioning for AQUAPINE departments"
git commit -m "docs: add storage architecture decision records"
git commit -m "fix: correct RBAC scope for farm managers group"
git commit -m "refactor: optimize VM deployment script for readability"
git commit -m "chore: update .gitignore to exclude sensitive configs"
```

---

### Branch Naming (Optional, for Advanced Work)

```
feat/[feature-name]       # New feature
fix/[bug-description]     # Bug fix
docs/[doc-update]         # Documentation
refactor/[improvement]    # Code refactoring

# Examples
feat/vnet-peering-setup
fix/storage-access-permissions
docs/deployment-guide-update
refactor/powershell-error-handling
```

---

## STUDY RESOURCES INDEX

### Microsoft Learn (Primary)

**AZ-104 Learning Path**:
https://learn.microsoft.com/en-us/certifications/exams/az-104

**Module Breakdown**:
1. Prerequisites for Azure administrators
2. Manage identities and governance
3. Implement and manage storage
4. Deploy and manage Azure compute resources
5. Configure and manage virtual networks
6. Monitor and maintain Azure resources

**Pro Tips**:
- Complete all hands-on exercises in Microsoft Learn sandbox
- Retake knowledge checks until 100%
- Use "Download PDF" for offline study

---

### O'Reilly Platform

**Recommended Video Courses**:
1. "Microsoft Azure Administrator (AZ-104)" by Scott Duffy (12+ hours)
2. "Azure Administrator Certification (AZ-104)" by Skylines Academy
3. "Azure Administration: Identities and Governance" (LinkedIn Learning)

**Recommended Books**:
1. "Exam Ref AZ-104 Microsoft Azure Administrator" - Washam, Hotek, De Kort
2. "Azure for Architects" - Ritesh Modi
3. "Learn Azure in a Month of Lunches" - Iain Foulds

**Study Strategy**:
- Watch videos at 1.25x-1.5x speed
- Pause to take notes
- Follow along with demos in your own Azure subscription
- Bookmark specific timestamps for review

---

### Supplementary Resources

**Official Microsoft Docs**:
- https://docs.microsoft.com/azure

**Azure Blog**:
- https://azure.microsoft.com/blog

**Community**:
- Reddit: r/Azure, r/AzureCertification
- Discord: Azure community servers
- Twitter: Follow @Azure, @AzureSupport

**Practice Exams** (Use in final weeks):
- MeasureUp AZ-104 practice tests
- Whizlabs AZ-104 practice exams
- Microsoft Learn assessment questions

---

## TROUBLESHOOTING & FAQ

### Common Issues

**"My Azure credit ran out!"**
- Check usage in Cost Management
- Delete unused resources daily
- Use B-series VMs (cheapest)
- Stop/deallocate VMs when not in use
- Apply for additional student credits if needed

**"My script isn't working!"**
- Check Azure subscription context: `Get-AzContext`
- Verify resource group exists
- Check RBAC permissions
- Review error message carefully
- Search Microsoft docs for error code
- Ask instructor (Claude) with full error message

**"I'm falling behind on schedule"**
- It's okay! Quality > speed
- Adjust weekly goals to match your pace
- Focus on one domain at a time
- Don't skip fundamentals
- Consider extending program to 20 weeks

**"GitHub isn't syncing"**
- Check remote: `git remote -v`
- Pull before push: `git pull origin main`
- Check for merge conflicts
- Verify GitHub authentication
- Use GitHub Desktop if CLI is confusing

**"I don't understand a concept"**
- Re-read Microsoft Learn module
- Watch O'Reilly video on same topic
- Draw it out (diagrams help!)
- Explain it to someone (or yourself aloud)
- Ask instructor specific questions
- Build it in a lab (hands-on solidifies understanding)

---

## PROGRESS TRACKING

### Weekly Checklist Template

```markdown
# Week X Progress Tracker

## Theory Completion (Mon-Thu)
- [ ] Microsoft Learn Module 1
- [ ] Microsoft Learn Module 2
- [ ] Microsoft Learn Module 3
- [ ] O'Reilly Video Chapter 1
- [ ] O'Reilly Video Chapter 2
- [ ] Flashcards created: [count]
- [ ] Study hours: [X/8-12]

## Lab Completion (Fri-Sun)
- [ ] Friday: Environment setup
- [ ] Friday: Initial scripts written
- [ ] Saturday: Deployment complete
- [ ] Saturday: Validation successful
- [ ] Sunday: Documentation finished
- [ ] Sunday: GitHub updated
- [ ] Lab hours: [X/12-18]

## Portfolio Quality
- [ ] README.md professional
- [ ] Code has error handling
- [ ] No hardcoded secrets
- [ ] Screenshots captured
- [ ] Diagrams created (if needed)
- [ ] Commit messages meaningful

## Professional Development
- [ ] LinkedIn post published (optional)
- [ ] Interview talking points updated
- [ ] Learning journal completed
- [ ] Next week planned

## Self-Assessment
**Confidence level (1-10)**: [X]  
**Readiness to proceed**: [Yes/No]  
**Questions for instructor**: [List]
```

---

### Domain Completion Checklist

```markdown
# Domain X Completion Checklist

## Technical Mastery
- [ ] All Microsoft Learn modules complete (100%)
- [ ] All O'Reilly chapters watched
- [ ] All hands-on labs completed
- [ ] Validation successful for all labs
- [ ] Capstone project complete
- [ ] Instructor review passed

## Portfolio Deliverables
- [ ] Domain folder on GitHub complete
- [ ] README.md professional quality
- [ ] All scripts tested and documented
- [ ] Bicep/Terraform templates validated
- [ ] Screenshots and diagrams included
- [ ] Interview talking points written

## Exam Readiness
- [ ] Can explain all concepts clearly
- [ ] Know PowerShell cmdlets for domain
- [ ] Understand exam objectives
- [ ] Practice questions answered (80%+ correct)

## Approval
- [ ] **Student self-approval**: Ready to proceed
- [ ] **Instructor (Claude) approval**: Code review passed

**Date Completed**: [YYYY-MM-DD]  
**Time Invested**: [X hours]  
**Next Domain**: [Name]
```

---

### Final AZ-104 Readiness Checklist

```markdown
# AZ-104 Exam Readiness - Final Check

## Knowledge Domains
- [ ] Domain 1: Identity & Governance (25-30%) - CONFIDENT
- [ ] Domain 2: Storage (15-20%) - CONFIDENT
- [ ] Domain 3: Compute (20-25%) - CONFIDENT
- [ ] Domain 4: Networking (20-25%) - CONFIDENT
- [ ] Domain 5: Monitoring (10-15%) - CONFIDENT

## Practical Skills
- [ ] Can deploy resources via Portal, PowerShell, CLI
- [ ] Comfortable with Bicep templates
- [ ] Understand Terraform basics
- [ ] Can troubleshoot common issues
- [ ] Know Azure pricing and cost management

## Portfolio Complete
- [ ] GitHub repository polished
- [ ] LinkedIn profile updated
- [ ] Resume includes Azure projects
- [ ] Can explain work in interviews (practiced)

## Exam Logistics
- [ ] AZ-104 exam scheduled
- [ ] Study materials reviewed
- [ ] Practice exams taken (75%+ score)
- [ ] Exam day plan prepared

## Final Approval
- [ ] **Self-assessment**: READY
- [ ] **Instructor (Claude) assessment**: READY
- [ ] **Confidence level**: 8+/10

**Exam Date**: [YYYY-MM-DD]  
**Good luck! 🎯**
```

---

## FINAL WORDS

### Your Success Mantra

```
📘 STUDY with intention (quality over quantity)
💻 CODE like a professional (error handling, documentation)
📝 DOCUMENT for your future self (you'll forget details)
🚀 PUBLISH consistently (GitHub is your resume)
🎤 PRACTICE storytelling (technical interviews are conversations)
```

### When You Feel Stuck

1. **Pause** - Take a break, walk outside
2. **Review** - Go back to basics, re-read notes
3. **Ask** - Use Claude (instructor), Azure community, forums
4. **Build** - Hands-on practice solidifies understanding
5. **Reflect** - Journal what you're learning and why it's hard

### Remember

> "You're not just learning Azure—you're building a career in cloud computing. Every script you write, every resource you deploy, and every mistake you troubleshoot is making you a better Azure Administrator. The AQUAPINE CONSULT scenario isn't just a story—it's your professional narrative. Own it."

---

**You've got this! 🚀**

Start with Week 0 Pre-Flight Checklist and work through systematically.

When ready, activate your instructor (Claude) with the master prompt and begin:

> "Instructor, I've completed the pre-flight checklist. I'm ready to begin AZ-104 Domain 1: Manage Azure Identities and Governance. This is Week 1, Monday—theory day."

**Welcome to your Azure Administrator journey!**

---

**END OF LEARNING MANUAL**