# Assessment Methodology

## ISO 27001 Gap Analysis — TechCo Pvt Ltd

---

## Executive Summary

This document outlines the methodology used to conduct a comprehensive ISO 27001:2022 gap analysis for TechCo Pvt Ltd, a 50-person software development company in Karachi.

**Assessment Scope**: 20 critical ISO 27001:2022 Annex A controls across 4 themes
**Assessment Date**: June 2026
**Methodology**: Control-based evaluation with maturity assessment
**Risk Rating**: MEDIUM (3 Implemented, 7 Partial, 10 Missing)

---

## 1. Assessment Approach

### 1.1 Control Selection Criteria

Controls were selected based on:
- **Relevance to startup environment** (50-person software company)
- **High-risk categories** (Access control, logging, incident response)
- **Compliance importance** (Most frequently audited controls)
- **Practical impact** (Controls with immediate business implications)

### 1.2 Evaluation Framework

Each control was assessed across 4 dimensions:

```
┌─────────────────────────────────────────┐
│         Control Assessment              │
├─────────────────────────────────────────┤
│ 1. Existence: Does the control exist?   │
│ 2. Formality: Is it documented?         │
│ 3. Effectiveness: Does it work?         │
│ 4. Maturity: How mature is it?          │
└─────────────────────────────────────────┘
```

---

## 2. Maturity Levels

### **Level 0 - Missing** (Red)
- ❌ No control exists
- ❌ No process documented
- ❌ No accountability
- 🎯 **Immediate action required**

### **Level 1 - Partial** (Yellow)
- ⚠️ Control exists but incomplete
- ⚠️ Process is informal/undocumented
- ⚠️ Limited effectiveness
- 🎯 **Needs formalization and documentation**

### **Level 2 - Implemented** (Green)
- ✅ Control fully in place
- ✅ Process documented
- ✅ Effective and monitored
- 🎯 **Maintain and improve**

---

## 3. Risk Prioritization Matrix

Controls were prioritized using Likelihood × Impact scoring:

```
Impact (Confidentiality, Integrity, Availability)
│
│  High (9-10)  │  Medium  │  High   │
│               │ (6-8)    │ (8-10)  │
├───────────────┼──────────┼─────────┤
│ Medium (5-6)  │  Low     │ Medium  │
│               │ (3-5)    │ (6-8)   │
├───────────────┼──────────┼─────────┤
│  Low (1-4)    │  Low     │ Low     │
│               │ (1-4)    │ (4-6)   │
└───────────────┴──────────┴─────────┘
            Likelihood →
```

### Priority Classification

**Critical** (Risk Score 8-10)
- Privileged access management
- Event logging
- Secure areas
- Incident response

**High** (Risk Score 6-7)
- Access control policies
- Cryptography management
- Third-party access
- User access reviews

**Medium** (Risk Score 4-5)
- Personnel screening
- Physical security (non-critical)
- Encryption policies

**Low** (Risk Score 1-3)
- Policy review cycles
- Environmental monitoring

---

## 4. Control Categories

### Organisational Controls
Focus on governance, policies, and accountability structures.
- Example: A.5.1 (Security Policies), A.5.2 (Roles & Responsibilities)

### People Controls
Focus on personnel, training, and human security.
- Example: A.6.1 (Screening), A.6.2 (Employment Terms)

### Physical Controls
Focus on physical security and premises protection.
- Example: A.7.1 (Physical Entry), A.7.2 (Secure Areas)

### Technological Controls
Focus on systems, access control, logging, and encryption.
- Example: A.8.2 (PAM), A.11.1 (Event Logging), A.12.2 (Incident Response)

---

## 5. TechCo Assessment Context

### Company Profile
- **Size**: 50 employees
- **Type**: Software development
- **Location**: Karachi, Pakistan
- **Maturity**: Early-stage startup
- **Security Posture**: Developing

### Assessment Assumptions

**What TechCo Likely HAS**:
✅ Basic office setup with some security measures
✅ Founder/CTO with security awareness
✅ Some encryption (databases)
✅ Cloud infrastructure (GitHub, AWS, Slack)
✅ Initial backup processes

**What TechCo Likely LACKS**:
❌ Dedicated security team
❌ Formal security processes/documentation
❌ Enterprise security tools (PAM, SIEM)
❌ Formal compliance program
❌ Structured incident response

---

## 6. Assessment Methodology - Detail

### Step 1: Control Definition
- Review ISO 27001:2022 Annex A control description
- Understand control objectives and intent
- Identify what "implemented" means for that control

### Step 2: Current State Analysis
- Assess what TechCo currently has in place
- Evaluate formality and documentation level
- Score against maturity criteria

### Step 3: Gap Identification
- Identify specific gaps between standard and current state
- Describe the security implication of each gap
- Assess risk level (Likelihood × Impact)

### Step 4: Recommendation Development
- Recommend specific solutions aligned with ISO 27001
- Include tool recommendations where applicable
- Provide implementation approach

### Step 5: Prioritization
- Assign priority based on risk and effort
- Create implementation roadmap
- Identify quick wins vs. long-term projects

---

## 7. Gap Analysis Output

### Control Assessment Report
**Format**: Spreadsheet with 7 columns:
1. Control ID (ISO 27001 reference)
2. Control Name (what it's about)
3. Category (Organisational/People/Physical/Technological)
4. Status (Implemented/Partial/Missing)
5. Gap Description (what's wrong, why it matters)
6. Recommendation (specific action with tools/standards)
7. Priority (Critical/High/Medium/Low)

### Summary Metrics
- Total controls: 20
- Implemented: 3 (15%)
- Partial: 7 (35%)
- Missing: 10 (50%)
- Critical gaps: 6
- Overall risk: MEDIUM

---

## 8. Recommendation Framework

Each recommendation follows this structure:

```
PROBLEM: [What's missing]
↓
IMPACT: [Why it matters - security/compliance/business]
↓
SOLUTION: [Specific recommendation]
↓
APPROACH: [How to implement]
↓
TOOLS: [Specific products/solutions]
↓
TIMELINE: [Suggested implementation window]
```

**Example - A.8.2 (Privileged Access Management)**

```
PROBLEM: No PAM system, shared admin passwords, no logging
IMPACT: Admins can access anything without audit trail; 
        insider threat risk; compliance violation
SOLUTION: Implement centralized PAM with access logging
APPROACH: 
  1. Select PAM tool (Vault or AWS IAM)
  2. Onboard critical systems
  3. Implement access approval workflow
  4. Enable audit logging
TOOLS: HashiCorp Vault, AWS IAM, Okta
TIMELINE: 1-2 months
```

---

## 9. Implementation Roadmap

### Phase 1: Critical Controls (Months 1-2)
- Secure server room (A.7.2)
- PAM implementation (A.8.2, A.9.2)
- Incident response plan (A.12.2)

### Phase 2: Compliance Foundation (Months 2-3)
- Centralized logging (A.11.1, A.11.2)
- User access reviews (A.9.4)
- Vendor access control (A.9.3)

### Phase 3: Policy Formalization (Months 4-6)
- Encryption policy (A.10.1)
- Access provisioning process (A.9.1)
- Incident classification (A.12.1)

---

## 10. Success Criteria

### Short-term (3 months)
- [ ] 6 critical controls improved
- [ ] Incident response plan in place
- [ ] PAM system deployed
- [ ] Logging centralized

### Medium-term (6 months)
- [ ] 12 controls at "Implemented" level
- [ ] Formal policies documented
- [ ] Vendor access governance active
- [ ] User access reviews conducted

### Long-term (12 months)
- [ ] ISO 27001 certification audit-ready
- [ ] 15+ controls fully implemented
- [ ] Compliance program established
- [ ] Annual audit completion

---

## 11. Methodology Limitations

### Scope Limitations
- Assessment is fictional scenario-based
- Does not include actual system testing
- Based on assumed current state

### Control Selection
- 20 controls selected from 93 total
- Focused on highest-risk controls
- May not cover all compliance requirements

### Recommendation Applicability
- Recommendations are general guidance
- Specific tools/approaches should be validated with security team
- Implementation should follow organizational change management

---

## 12. Quality Assurance

### Control Verification
- Each control assessed against ISO 27001:2022 standard
- Gap descriptions validated against control objectives
- Recommendations cross-referenced with best practices

### Consistency Checks
- Similar controls have consistent assessment approach
- Risk prioritization applied consistently
- Recommendation quality verified

---

## 13. References & Standards

- **ISO/IEC 27001:2022** - Information Security Management System
- **ISO/IEC 27002:2022** - Code of Practice
- **NIST Cybersecurity Framework** - Risk management approach
- **CIS Controls** - Critical security controls
- **COSO ERM** - Enterprise risk management

---

## Conclusion

This gap analysis demonstrates a structured, risk-based approach to ISO 27001 compliance assessment. The methodology:

✅ Follows industry standards (ISO 27001:2022)
✅ Prioritizes controls by risk
✅ Provides actionable recommendations
✅ Creates implementation roadmap
✅ Enables compliance planning

---

**Prepared by**: GRC Portfolio Assessment
**Date**: June 2026
**Version**: 1.0
