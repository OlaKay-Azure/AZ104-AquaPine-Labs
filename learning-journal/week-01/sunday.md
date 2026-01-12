$sundayTemplate = @"
# Week 1, Sunday - January 18, 2026

## 🔄 REFLECTION & PLANNING DAY

**Focus**: Week review + Week 2 preparation  
**Duration**: [X] hours

## 📊 Week 1 Final Statistics

**Study Hours**:
- Monday: [X] hrs
- Tuesday: [X] hrs
- Wednesday: [X] hrs
- Thursday: [X] hrs
- Friday: [X] hrs
- Saturday: [X] hrs
- Sunday: [X] hrs
- **Total**: [X/55] hours

**Domains Completed**: 
- Domain 1: [X%]

**Labs Deployed**: 3/3 ✅

## 💡 Week 1 Key Learnings
1. **Technical**:
2. **Process**:
3. **Personal**:

## 🎯 Week 2 Preview
**Focus**: Domain 1 completion + Capstone  
**Microsoft Learn**: [Modules planned]  
**Labs**: Governance, Policy, Capstone

## 💼 LinkedIn Activity
- [ ] Weekly post published ✅
- [ ] Engagement count: [X reactions, X comments]

## 🎓 Self-Assessment
**Confidence by Topic**:
- Entra ID: [1-10]
- RBAC: [1-10]
- Azure Policy: [1-10]

**Overall Week 1 Rating**: [1-10]

## 🎯 Week 2 Goals
1. [Specific goal 1]
2. [Specific goal 2]
3. [Specific goal 3]

**Status**: Week 1 COMPLETE! 🎉  
**Readiness for Week 2**: [High/Medium/Low]
"@

$sundayTemplate | Out-File -FilePath "learning-journal/week-01/sunday.md" -Encoding utf8
