# GRC Portfolio - Governance, Risk & Compliance

A comprehensive Governance, Risk, and Compliance (GRC) portfolio demonstrating practical security assessment and control implementation methodologies aligned with ISO 27001:2022.

---

## 📋 Project Overview

This portfolio contains practical GRC artifacts that demonstrate understanding of:
- **Governance**: Security policies, roles, and accountability structures
- **Risk**: Systematic identification, assessment, and mitigation of security risks
- **Compliance**: Alignment with international standards (ISO 27001, NIST CSF, GDPR)

### Artifacts Included:
1. **ISO 27001 Gap Analysis** — Control assessment (20 critical controls)
2. **Risk Register** — Organizational risk identification and scoring (10 organizational risks)
3. **Supporting Documentation** — Methodology, executive summary, detailed explanations

### Case Study: TechCo Pvt Ltd
A fictional 50-person software company in Karachi serving as the basis for all assessments. Used to demonstrate realistic security assessment in a startup environment.

---

## 📁 Contents

### 1. **ISO 27001 Gap Analysis** (`ISO27001_Gap_Analysis_TechCo.xlsx`)

**What it is**: A comprehensive control assessment against ISO 27001:2022 Annex A (93 controls across 4 themes).

### 2. **Risk Register** (`Risk_Register_TechCo.xlsx`)

**What it is**: A comprehensive control assessment against ISO 27001:2022 Annex A (93 controls across 4 themes).

**What you'll find**:
- **Gap Analysis Sheet**: 20 critical controls evaluated across:
  - Control ID & Name (ISO 27001 reference)
  - Category (Organisational, People, Physical, Technological)
  - Status (Implemented, Partial, Missing)
  - Gap Description (what's missing and why it matters)
  - Recommendation (specific solution with tools/standards)
  - Priority (Critical, High, Medium, Low)

- **Summary Sheet**: Auto-calculated metrics showing:
  - Control compliance breakdown (3 Implemented, 7 Partial, 10 Missing)
  - Critical control count (6 critical gaps identified)
  - Overall risk level: **MEDIUM**

**Key Findings**:
- ✅ **Strengths**: Basic policies in place, some encryption, CCTV monitoring
- ⚠️ **Weaknesses**: No PAM, no incident response plan, unlogged admin access
- 🔴 **Critical Gaps**: Secure areas, privileged access management, event logging, log protection

**How to Use**:
1. Open in Excel or Google Sheets
2. Review the Gap Analysis tab for detailed control assessments
3. Check Summary tab for high-level risk metrics
4. Use recommendations as roadmap for security improvements

### 2. **Risk Register** (`Risk_Register_TechCo.xlsx`)

**What it is**: A comprehensive organizational risk assessment using Likelihood × Impact scoring methodology.

**What you'll find**:
- **Risk Register Sheet**: 10 organizational risks evaluated across:
  - Risk ID (unique identifier)
  - Asset (what's at risk)
  - Threat (what could go wrong)
  - Vulnerability (why it's possible)
  - Likelihood (1-5 scale)
  - Impact (1-5 scale)
  - Risk Score (Likelihood × Impact = 1-25)
  - Treatment (Mitigate/Accept/Transfer/Avoid)
  - Owner (who's responsible)
  - Status (Not Started/In Progress/Planned/Monitored)

- **Summary Sheet**: Auto-calculated metrics showing:
  - Risk distribution by severity (0 Critical, 3 High, 7 Medium, 0 Low)
  - Treatment strategy breakdown (8 Mitigate, 1 Accept, 1 Avoid)
  - Implementation status (3 Not Started, 4 In Progress, 2 Planned, 1 Monitored)

**Key Findings**:
- 🟠 **3 HIGH-RISK items** (scores 13-20):
  - Phishing Attack (16)
  - Unauthorized Database Access (16)
  - Data Breach via Third Party (15)

- 🟡 **7 MEDIUM-RISK items** (scores 6-12):
  - Unpatched Server Vulnerability
  - Insider Threat/Data Theft
  - DDoS Attack
  - Missing Security Headers
  - Weak Password Policy
  - No MFA on Critical Systems
  - Outdated Dependencies

**How to Use**:
1. Open in Excel and review Risk Register tab
2. Understand each risk (Likelihood × Impact scoring)
3. Note which risks are high-priority (orange color)
4. Review treatment strategy for each risk
5. Check Summary tab for distribution metrics
6. Use as roadmap for security remediation

---

## 🎯 GRC Concepts Demonstrated

### Governance
- Role-based access control (RBAC)
- Responsibility matrices
- Policy documentation and review cycles
- Vendor management processes

### Risk
- **Control assessment methodology** (Gap Analysis)
- **Risk identification and scoring** (Risk Register)
- **Likelihood vs. Impact evaluation** (1-5 scale)
- **Risk prioritization** (Critical/High/Medium/Low)
- Mitigation strategies and treatment selection

### Compliance
- ISO 27001:2022 Annex A alignment
- Control categorization (Organisational, People, Physical, Technological)
- Documentation requirements
- Audit readiness

---

## 🔒 Security Controls Assessed

### Organisational (2)
- Policies for information security
- Information security roles and responsibilities

### People (2)
- Personnel screening
- Employment terms and conditions

### Physical (3)
- Physical entry control
- Secure areas
- Physical and environmental security

### Technological (13)
- User endpoint devices
- Privileged access rights
- Information access restriction
- Access to cryptographic keys
- User registration and provisioning
- Third-party access control
- User access reviews
- Cryptography use policy
- Event logging
- Log protection
- Incident response classification
- Incident management

---

## 📊 Assessment Methodology

### 1. Gap Analysis (Controls)
Evaluated 20 critical ISO 27001:2022 controls against current state.
- Status: 3 Implemented (15%), 7 Partial (35%), 10 Missing (50%)
- Overall risk from missing controls: MEDIUM

### 2. Risk Register (Organizational Risks)
Identified and scored 10 organizational risks using Likelihood × Impact methodology.
- High-Risk items: 3 (Phishing, Unauthorized access, Third-party breach)
- Medium-Risk items: 7 (Unpatched systems, weak passwords, no MFA, etc.)
- Risk score range: 1-25 (higher = worse)

### Combined Assessment
- **Gap Analysis** identifies WHAT controls are missing
- **Risk Register** prioritizes WHICH risks to address first
- Together they form a complete security assessment and remediation roadmap

---
1. **Implement PAM Solution** (A.8.2, A.9.2)
   - Recommended: HashiCorp Vault or AWS IAM
   - Requirement: Full audit logging of admin actions
   
2. **Establish Secure Server Room** (A.7.2)
   - Requirement: Badge access, CCTV, environmental monitoring
   
3. **Deploy Centralized Logging** (A.11.1, A.11.2)
   - Recommended: CloudWatch, Splunk, or ELK Stack
   - Requirement: Immutable storage (AWS S3 Object Lock)

4. **Develop Incident Response Plan** (A.12.2)
   - Requirement: Documented procedures, escalation matrix, communication templates

### High Priority (Within 3 months)
- User access review process (quarterly)
- Vendor access agreements
- Encryption policy enforcement
- Offboarding procedure for departing employees

### Medium Priority (Within 6 months)
- Encryption key management automation
- Environmental monitoring sensors
- Endpoint encryption standardization

---

## 📊 Assessment Methodology

### Control Evaluation Criteria

**Implemented** (Green)
- Control fully in place
- Documented process exists
- Regularly reviewed/updated

**Partial** (Yellow)
- Control exists but incomplete
- Some gaps in documentation
- Process may be informal

**Missing** (Red)
- Control not implemented
- No formal process
- Immediate risk identified

---

## 🚀 Next Steps

### Phase 1 (Month 1)
- Secure server room implementation
- PAM tool selection and deployment
- Incident response plan development

### Phase 2 (Month 2-3)
- Centralized logging deployment
- User access review process
- Vendor access governance

### Phase 3 (Month 4-6)
- Encryption policy implementation
- Advanced monitoring (SIEM)
- Formal ISO 27001 audit preparation

---

## 📚 Standards & Frameworks Referenced

- **ISO 27001:2022** - Information Security Management System
- **ISO 27002:2022** - Code of Practice for Information Security Controls
- **NIST Cybersecurity Framework** - Risk-based security approach
- **GDPR** - Data protection compliance (relevant for EU customer data)
- **COSO ERM** - Enterprise Risk Management framework

---

## 👤 Author Notes

This gap analysis was conducted as a learning exercise in GRC principles and control assessment methodologies. It demonstrates:

✅ Understanding of ISO 27001 control structure
✅ Ability to identify gaps in security posture
✅ Knowledge of practical remediation approaches
✅ Risk prioritization methodology
✅ Professional security assessment documentation

**Assessment Rigor**: Controls were evaluated based on realistic startup scenario assumptions, industry best practices, and compliance requirements.

---

## 📞 Usage & Attribution

This portfolio is created for educational and professional development purposes. 

**Portfolio Context**: Demonstrating GRC competency for:
- Security analyst/engineer roles
- GRC specialist positions
- Risk assessment capabilities
- Compliance audit knowledge

---

## 📝 License

Educational portfolio - All frameworks and methodologies reference published standards (ISO 27001, NIST CSF, GDPR).

---

## 🔗 Connect

- **GitHub**: [@Shaheer005](https://github.com/Shaheer005)
- **LinkedIn**: [Shaheer Ahmed](https://www.linkedin.com/in/shaheer-ahmed-64055223b/)
- **Email**: shaheer05ahmed@gmail.com

---

**Last Updated**: June 2, 2026
**Assessment Company**: TechCo Pvt Ltd (Fictional)
**Standard**: ISO 27001:2022
**Assessment Type**: Comprehensive Gap Analysis
