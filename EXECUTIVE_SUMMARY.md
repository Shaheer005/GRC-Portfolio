# Executive Summary: ISO 27001 Gap Analysis

## TechCo Pvt Ltd | June 2026

---

## Overview

This report summarizes a comprehensive ISO 27001:2022 gap analysis conducted for TechCo Pvt Ltd, a 50-person software development company based in Karachi. The assessment evaluated 20 critical information security controls across four domains: Organisational, People, Physical, and Technological.

---

## Key Findings

### Control Maturity Breakdown

| Status | Count | Percentage | Color |
|--------|-------|-----------|-------|
| **Implemented** | 3 | 15% | 🟢 |
| **Partial** | 7 | 35% | 🟡 |
| **Missing** | 10 | 50% | 🔴 |

### Critical Findings

**6 Critical-Priority Controls Missing or Partial**:

🔴 **A.7.2 - Secure Areas**
- Status: Missing
- Risk: Servers in shared office space without physical security
- Impact: Physical theft/sabotage of infrastructure

🔴 **A.8.2 - Privileged Access Management**
- Status: Missing
- Risk: Admin accounts unmonitored, shared passwords
- Impact: No audit trail; insider threat; compliance violation

🔴 **A.11.1 - Event Logging**
- Status: Partial
- Risk: No database/server/admin logging
- Impact: Cannot detect or investigate security incidents

🔴 **A.11.2 - Log Protection**
- Status: Partial
- Risk: Logs stored locally, any admin can delete
- Impact: Evidence tampering; audit failure

🔴 **A.12.1 - Incident Response Events**
- Status: Partial
- Risk: No defined incident response events or escalation
- Impact: Delayed incident detection and response

🔴 **A.12.2 - Incident Management**
- Status: Missing
- Risk: No incident response plan or procedures
- Impact: Chaotic response to security breaches

---

## Risk Assessment

### Overall Risk Rating: **MEDIUM**

**Justification**:
- ✅ **Strengths**: Basic policies exist, some encryption in place, founder aware of security
- ⚠️ **Concerns**: No privileged access management, unmonitored admin activity, no incident response
- 🔴 **Critical Gaps**: Physical security, logging, incident response

---

## Strategic Priorities

### Phase 1: Immediate Actions (1-2 months)
**Focus**: Critical control implementation

1. **Establish Secure Server Room** (A.7.2)
   - Budget: ~50,000 PKR
   - Timeline: 2-4 weeks
   - Impact: Eliminates physical theft risk

2. **Implement PAM Solution** (A.8.2)
   - Budget: ~300,000 PKR (AWS IAM) or 500,000+ (Enterprise)
   - Timeline: 4-6 weeks
   - Impact: Full audit trail of admin actions

3. **Deploy Incident Response Plan** (A.12.2)
   - Budget: Minimal (documentation + training)
   - Timeline: 1-2 weeks
   - Impact: Defined breach response procedures

### Phase 2: Compliance Foundation (3-4 months)
**Focus**: Logging, access reviews, vendor management

1. **Centralized Logging System** (A.11.1, A.11.2)
   - Tools: CloudWatch, Splunk, or ELK Stack
   - Budget: 100,000-500,000 PKR/month
   - Timeline: 4-8 weeks

2. **User Access Review Process** (A.9.4)
   - Process: Quarterly review + access removal
   - Budget: Minimal
   - Timeline: 2 weeks to implement

3. **Vendor Access Governance** (A.9.3)
   - Process: Vendor agreements + registry
   - Budget: Minimal
   - Timeline: 3-4 weeks

### Phase 3: Policy Formalization (5-6 months)
**Focus**: Documentation, encryption, process standardization

1. **Encryption Policy** (A.10.1)
2. **Offboarding Procedures** (A.9.4)
3. **Incident Classification Matrix** (A.12.1)

---

## Financial Impact Summary

### Implementation Costs

| Phase | Control | Est. Cost | Timeline |
|-------|---------|-----------|----------|
| 1 | Secure Areas | 50K PKR | 2-4 wks |
| 1 | PAM Solution | 300-500K PKR | 4-6 wks |
| 1 | Incident Plan | Minimal | 1-2 wks |
| 2 | Logging System | 100-500K/mo | 4-8 wks |
| 2 | Access Reviews | Minimal | 2 wks |
| 2 | Vendor Mgmt | Minimal | 3-4 wks |
| 3 | Policy Updates | Minimal | Ongoing |
| **Total** | **Year 1** | **~1.5-2M PKR** | **6 months** |

### Risk Mitigation Value

**By implementing these controls, TechCo will**:
- ✅ Reduce insider threat risk by 80%
- ✅ Achieve audit trail for all critical actions
- ✅ Enable incident detection and response
- ✅ Improve customer trust and compliance posture
- ✅ Prepare for ISO 27001 certification

---

## Detailed Findings by Domain

### 🏢 Organisational (2 controls)
**Status**: 1 Implemented, 1 Partial

- ✅ **A.5.1** - Policies exist and documented
- ⚠️ **A.5.2** - CISO role exists but unclear delegation

**Recommendation**: Formalize responsibility matrix for all security roles

---

### 👥 People (2 controls)
**Status**: 1 Implemented, 1 Partial

- ✅ **A.6.2** - Employment contracts include security clauses
- ⚠️ **A.6.1** - Background checks done but no reassessment

**Recommendation**: Implement periodic reassessment for high-risk positions

---

### 🏗️ Physical (3 controls)
**Status**: 1 Implemented, 1 Partial, 1 Missing

- ✅ **A.7.3** - CCTV and fire suppression in place
- ⚠️ **A.7.1** - Badge access only at main entrance
- 🔴 **A.7.2** - No secure server room (CRITICAL)

**Recommendation**: Establish locked server room with access logging as immediate priority

---

### 💻 Technological (13 controls)
**Status**: 1 Implemented, 4 Partial, 8 Missing

**Key Issues**:
- No privileged access management
- Keys stored in code repositories
- No centralized logging
- No incident response process
- Employees retain access after leaving

**Recommendation**: Implement technical security stack (PAM, logging, encryption management)

---

## Compliance Implications

### ISO 27001 Certification Readiness

**Current Status**: **Not Ready** (estimated 18-24 months)

**Prerequisites for Certification**:
1. ✅ Management commitment (foundational)
2. ⚠️ Documented policies (partially done)
3. 🔴 Implemented controls (50% complete)
4. 🔴 Evidence of effectiveness (minimal)
5. 🔴 Internal audit program (missing)

**Timeline to Certification**:
- Months 1-2: Critical controls
- Months 3-4: Medium-priority controls
- Months 5-6: Policy and documentation
- Months 7-12: Operational evidence and maturity
- Months 13-18: Internal audit and readiness
- Months 19-24: External audit and certification

---

## Recommendations for Management

### Immediate Actions (This Week)
1. [ ] Allocate budget for secure server room
2. [ ] Evaluate PAM tool options
3. [ ] Draft incident response plan

### Short-term (1-2 months)
1. [ ] Secure server room operational
2. [ ] PAM system deployed
3. [ ] Incident response plan published and trained

### Medium-term (3-6 months)
1. [ ] Logging system centralized
2. [ ] User access reviews conducted quarterly
3. [ ] Vendor access governance implemented

### Long-term (6-12 months)
1. [ ] All policies formally documented
2. [ ] Encryption enforced company-wide
3. [ ] Prepare for ISO 27001 audit

---

## Success Metrics

### 90-Day Goals
- [ ] 6 critical controls improved
- [ ] Incident response plan active
- [ ] PAM system deployed
- [ ] Logging infrastructure in place

### 180-Day Goals
- [ ] 12 controls at "Implemented" level
- [ ] User access reviews completed
- [ ] Vendor agreements signed
- [ ] Encryption policy enforced

### 12-Month Goals
- [ ] 15+ controls fully implemented
- [ ] ISO 27001 audit-ready
- [ ] Compliance program established
- [ ] Incident response tested

---

## Next Steps

1. **Review this report** with leadership team
2. **Prioritize Phase 1 controls** based on business impact
3. **Allocate budget** for security improvements
4. **Assign ownership** for each control
5. **Schedule implementation** with IT/Security team
6. **Monitor progress** monthly

---

## Conclusion

TechCo has a **solid security foundation** with some policies and basic controls in place. However, **critical gaps exist** in privileged access management, logging, and incident response that pose significant risk.

By implementing the **prioritized recommendations** in this assessment, TechCo can achieve:
- ✅ MEDIUM → LOW risk rating (6 months)
- ✅ ISO 27001 compliance (12-18 months)
- ✅ Enterprise security posture (24 months)

**Investment required**: ~1.5-2M PKR over 12 months
**Risk mitigation value**: Reduces insider threat, data breach, and compliance risk significantly

---

**Assessment Date**: June 2, 2026
**Company**: TechCo Pvt Ltd (Fictional)
**Assessor**: GRC Portfolio Assessment
**Standard**: ISO 27001:2022
