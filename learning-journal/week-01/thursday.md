$thursdayTemplate = @"
# Week 1, Thursday - January 15, 2026

## 🔥 IMPLEMENTATION DAY

**Lab Focus**: Lab 1.1 Entra ID Setup + Lab 1.2 RBAC  
**Total Duration**: [X] hours (Target: 10-12 hrs)

## 🚀 Deployment Log

### Morning Session (8:00-13:00)
**Lab 1.1: Entra ID Setup**

\`\`\`powershell
# Commands executed
# [Paste your actual commands here]
\`\`\`

**Resources Deployed**:
- [ ] Resource Group: rg-aquapine-identity
- [ ] 10 users created (Ibadan + Lagos)
- [ ] 6 security groups created

**Issues Encountered**:
1. **Issue**: [Describe problem]
   - **Solution**: [How you fixed it]
   - **Time Lost**: [X minutes]

### Afternoon Session (14:00-19:00)
**Lab 1.2: RBAC Configuration**

**RBAC Assignments**:
- [ ] Farm Managers → Contributor (Ibadan RG)
- [ ] HR Department → Owner (HR RG)
- [ ] Sales → Reader (Sales RG)

## ✅ Validation Results

### Test 1: User Authentication
\`\`\`powershell
Get-AzADUser -UserPrincipalName "farmmanager@aquapine.com"
# Output: [Paste result]
\`\`\`
**Status**: ✅ Pass / ❌ Fail

### Test 2: RBAC Verification
**Status**: ✅ Pass / ❌ Fail

## 📸 Screenshots Captured
- [ ] Entra ID user list
- [ ] Security groups overview
- [ ] RBAC assignments
- [ ] Validation outputs

## 💡 Lessons Learned
1. **Technical**: 
2. **Process**: 

## 🐛 Troubleshooting Log
| Time | Issue | Root Cause | Solution | Prevention |
|------|-------|------------|----------|------------|
| 10:30 | [Issue] | [Cause] | [Fix] | [How to avoid] |

## 📊 Lab Progress
**Lab 1.1**: [X%] Complete  
**Lab 1.2**: [X%] Complete  
**Overall Domain 1 Labs**: [X%]

## 🎯 Tomorrow's Focus
- [ ] Lab 1.3: Azure Policy
- [ ] Code review and refinement
- [ ] Begin documentation

**Confidence Level**: [1-10]  
**Status**: Day 4 - Labs in progress! 💻
"@

$thursdayTemplate | Out-File -FilePath "learning-journal/week-01/thursday.md" -Encoding utf8
