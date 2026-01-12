$fridayTemplate = @"
# Week 1, Friday - January 16, 2026

## 📋 Finalization Day

**Focus**: Complete remaining labs + Begin documentation  
**Duration**: [X] hours

## 🔧 Lab Completion
- [ ] Lab 1.3: Azure Policy ✅
- [ ] All validations passed ✅
- [ ] Code review complete ✅

## 📝 Documentation Started
- [ ] Lab READMEs drafted
- [ ] Architecture decisions documented
- [ ] Screenshots organized

## ✅ Week 1 Labs Status
- Lab 1.1: ✅ Complete
- Lab 1.2: ✅ Complete
- Lab 1.3: ✅ Complete

**Overall Domain 1 Progress**: [X%]

## 🎯 Weekend Plan
**Saturday**: Documentation & GitHub publishing  
**Sunday**: Reflection & Week 2 prep

**Status**: Week 1 labs complete! 🎉
"@

$fridayTemplate | Out-File -FilePath "learning-journal/week-01/friday.md" -Encoding utf8
