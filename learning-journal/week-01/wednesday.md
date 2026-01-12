# Wednesday Template
$wednesdayTemplate = @"
# Week 1, Wednesday - January 14, 2026

## 📚 Study Session Summary
**Total Duration**: [X] hours

## 📖 Resources Completed
- [ ] Final Microsoft Learn modules
- [ ] Final O'Reilly chapters

## 🎯 Domain Completion Status
**Microsoft Learn Domain 1**: [X%]  
**O'Reilly Identity Section**: [Complete/In Progress]

## 🔧 Lab Preparation
### Environment Setup Checklist
- [ ] Azure Portal logged in
- [ ] Resource group created
- [ ] Naming conventions defined
- [ ] PowerShell scripts ready
- [ ] VS Code workspace configured

### Scripts Finalized
- [ ] 01-create-users.ps1 - Error handling added ✅
- [ ] 02-create-groups.ps1 - Validation logic added ✅

## 💡 Key Insights
1. 
2. 

## ❓ Final Questions Before Lab
- [ ] Q1: 
- [ ] Q2: 

## 🎯 Thursday Lab Plan
**Lab 1.1 Objectives**:
1. Deploy Entra ID structure
2. Create 10+ users
3. Configure RBAC

**Expected Duration**: 5-6 hours

**Confidence Level**: [1-10]  
**Status**: Ready for implementation! 🚀
"@

$wednesdayTemplate | Out-File -FilePath "learning-journal/week-01/wednesday.md" -Encoding utf8
