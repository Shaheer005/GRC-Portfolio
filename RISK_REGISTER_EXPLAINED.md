# Risk Register - TechCo Pvt Ltd

## What You're Looking At

A professional **Risk Register** with:
- **10 organizational risks** (realistic for 50-person startup)
- **Likelihood × Impact scoring** (1-5 scale for each)
- **Risk scores** automatically calculated (L × I = 1-25)
- **Color-coded by severity** (Red=Critical, Orange=High, Yellow=Medium, Green=Low)
- **Treatment strategy** for each risk (Mitigate/Accept/Transfer/Avoid)
- **Owner assignment** (who's responsible)
- **Status tracking** (Not Started/In Progress/Planned/Monitored)

---

## The 10 Risks Explained

### Risk 1: Phishing Attack

| Component | Value | Why? |
|-----------|-------|------|
| **Asset at Risk** | Email System |  |
| **Threat** | Phishing Attack | Attackers send fake emails |
| **Vulnerability** | Employees unaware, no email filtering | Easy to trick someone |
| **Likelihood** | 4/5 | Phishing is VERY common |
| **Impact** | 4/5 | If successful = attacker has employee access |
| **Risk Score** | 4 × 4 = **16 (HIGH)** | 🟠 Medium-High risk |
| **Treatment** | **Mitigate** | Do something to reduce it |
| **Action** | Security training + email filtering |  |
| **Owner** | CISO | Responsible for implementation |
| **Status** | In Progress | Already being worked on |

**Why this matters**: Most common attack vector. Phishing emails trick employees into giving passwords.

---

### Risk 2: Unauthorized Database Access

| Component | Value |
|-----------|-------|
| **Asset** | Database (contains customer data) |
| **Threat** | Unauthorized Access |
| **Vulnerability** | No PAM, shared admin passwords, no logging |
| **Likelihood** | 4/5 | Anyone with admin password can access |
| **Impact** | 4/5 | Could steal all customer data |
| **Risk Score** | **16 (HIGH)** | 🟠 Critical |
| **Treatment** | **Mitigate** | Implement PAM system |
| **Owner** | CTO |
| **Status** | Not Started | Urgent |

**Why this matters**: Database has all customer data. If someone accesses it without permission = data breach.

---

### Risk 3: Unpatched Server Vulnerability

| Component | Value |
|-----------|-------|
| **Asset** | Web Servers |
| **Threat** | Unpatched Vulnerability |
| **Vulnerability** | No patch management process |
| **Likelihood** | 4/5 | Vulnerabilities found regularly |
| **Impact** | 3/5 | Attacker could break in, but not guaranteed |
| **Risk Score** | 4 × 3 = **12 (MEDIUM)** | 🟡 |
| **Treatment** | **Mitigate** | Patch management system |
| **Owner** | DevOps Lead |
| **Status** | In Progress |

**Why this matters**: Every month, new vulnerabilities found. If you don't patch, hackers use them.

---

### Risk 4: Data Breach via Third Party

| Component | Value |
|-----------|-------|
| **Asset** | Customer Data |
| **Threat** | Data Breach via Vendor |
| **Vulnerability** | Vendors have access but no agreements |
| **Likelihood** | 3/5 | Vendors get hacked sometimes |
| **Impact** | 5/5 | If vendor breached = YOUR customers' data stolen |
| **Risk Score** | 3 × 5 = **15 (HIGH)** | 🟠 |
| **Treatment** | **Mitigate** | Vendor agreements + monitoring |
| **Owner** | CISO |
| **Status** | Not Started |

**Why this matters**: Vendors have access to your systems. If THEY get hacked, you get hacked.

---

### Risk 5: Insider Threat

| Component | Value |
|-----------|-------|
| **Asset** | All Systems |
| **Threat** | Insider Threat/Data Theft |
| **Vulnerability** | Disgruntled employee with access |
| **Likelihood** | 2/5 | Rare but happens |
| **Impact** | 5/5 | Employee can steal everything |
| **Risk Score** | 2 × 5 = **10 (MEDIUM)** | 🟡 |
| **Treatment** | **Accept** | Living with it (hard to prevent 100%) |
| **Owner** | HR Manager |
| **Status** | Monitored |

**Why this matters**: You can't prevent every insider threat. Best you can do is monitor and respond.

---

### Risk 6: DDoS Attack

| Component | Value |
|-----------|-------|
| **Asset** | Web Service |
| **Threat** | DDoS Attack |
| **Vulnerability** | No DDoS protection |
| **Likelihood** | 2/5 | Possible but not common for small companies |
| **Impact** | 4/5 | Service goes down, customers can't use it |
| **Risk Score** | 2 × 4 = **8 (MEDIUM)** | 🟡 |
| **Treatment** | **Mitigate** | DDoS protection service (CloudFlare) |
| **Owner** | Infrastructure Team |
| **Status** | Not Started |

**Why this matters**: Attackers could take down your service by flooding it with traffic.

---

### Risk 7: Missing Security Headers

| Component | Value |
|-----------|-------|
| **Asset** | Web Application |
| **Threat** | Missing Security Headers |
| **Vulnerability** | XSS/Clickjacking vulnerabilities |
| **Likelihood** | 3/5 | Hackers look for this |
| **Impact** | 3/5 | Could steal user session/data |
| **Risk Score** | 3 × 3 = **9 (MEDIUM)** | 🟡 |
| **Treatment** | **Mitigate** | Add security headers |
| **Owner** | Dev Team |
| **Status** | In Progress |

**Why this matters**: Missing headers = attackers can do XSS attacks (steal user cookies/sessions).

---

### Risk 8: Weak Password Policy

| Component | Value |
|-----------|-------|
| **Asset** | User Accounts |
| **Threat** | Weak Password Policy |
| **Vulnerability** | No password complexity requirements |
| **Likelihood** | 4/5 | Employees use weak passwords like "password123" |
| **Impact** | 3/5 | Attacker can brute-force/guess password |
| **Risk Score** | 4 × 3 = **12 (MEDIUM)** | 🟡 |
| **Treatment** | **Mitigate** | Enforce strong passwords + MFA |
| **Owner** | CISO |
| **Status** | Not Started |

**Why this matters**: Weak passwords = easy for hackers to break in.

---

### Risk 9: No MFA on Critical Systems

| Component | Value |
|-----------|-------|
| **Asset** | Critical Systems (Admin/Database) |
| **Threat** | No MFA on Login |
| **Vulnerability** | Only password required |
| **Likelihood** | 3/5 | Attacker knows password (phishing/breach) |
| **Impact** | 4/5 | Without MFA, attacker gets in |
| **Risk Score** | 3 × 4 = **12 (MEDIUM)** | 🟡 |
| **Treatment** | **Mitigate** | Enable MFA (Google Authenticator, Authy) |
| **Owner** | CTO |
| **Status** | Planned |

**Why this matters**: Even if password stolen, MFA stops attacker (need phone to approve login).

---

### Risk 10: Outdated Dependencies

| Component | Value |
|-----------|-------|
| **Asset** | Application Code |
| **Threat** | Outdated Dependencies |
| **Vulnerability** | Old libraries with known vulnerabilities |
| **Likelihood** | 4/5 | Developers often use old libraries |
| **Impact** | 2/5 | Vulnerability in library but may not be exploited |
| **Risk Score** | 4 × 2 = **8 (MEDIUM)** | 🟡 |
| **Treatment** | **Mitigate** | Dependency scanning + updates |
| **Owner** | Dev Team |
| **Status** | In Progress |

**Why this matters**: Old libraries have known vulnerabilities. Hackers look for these.

---

## Risk Scoring Summary

### By Severity Level

| Level | Score | Count | Color | Action |
|-------|-------|-------|-------|--------|
| **Critical** | 21-25 | 0 | 🔴 Red | IMMEDIATE |
| **High** | 13-20 | 3 | 🟠 Orange | This Month |
| **Medium** | 6-12 | 7 | 🟡 Yellow | This Quarter |
| **Low** | 1-5 | 0 | 🟢 Green | Monitor |

**3 HIGH-RISK** items:
1. Phishing Attack (16)
2. Unauthorized Database Access (16)
3. Data Breach via Third Party (15)

**7 MEDIUM-RISK** items:
- Unpatched servers, Insider threat, DDoS, Missing headers, Weak passwords, No MFA, Outdated dependencies

---

## Treatment Strategy Distribution

| Treatment | Count | Meaning |
|-----------|-------|---------|
| **Mitigate** | 8 | Do something to reduce risk |
| **Accept** | 1 | Living with it (unavoidable) |
| **Transfer** | 0 | Buy insurance/outsource |
| **Avoid** | 1 | Stop the activity |

**Most risks are "Mitigate"** = TechCo is taking action to reduce risk.

---

## Implementation Status

| Status | Count | Meaning |
|--------|-------|---------|
| **Not Started** | 3 | Need to start immediately |
| **In Progress** | 4 | Already being worked on |
| **Planned** | 2 | Will start soon |
| **Monitored** | 1 | Ongoing monitoring |

**3 risks not started** (Unauthorized DB access, DDoS, Weak passwords) = URGENT

---

## Interview Line (Use This!)

**When they ask**: "How do you assess and manage risk?"

**Your answer**: 
"I create a risk register by identifying organizational threats and evaluating them using likelihood × impact scoring. For example, in my analysis of a 50-person software company:

- I identified 10 key risks
- Scored each by likelihood (1-5) and impact (1-5)
- Calculated risk scores (L × I = 1-25)
- Color-coded by severity (Red=Critical, Orange=High, Yellow=Medium)
- Assigned treatment (Mitigate/Accept/Transfer/Avoid)
- Identified owners for each risk

The analysis showed 3 high-risk items (unauthorized access, phishing, third-party breach) requiring immediate mitigation. This approach prioritizes security investments based on actual organizational risk."

**Boom.** That's how a GRC person talks. ✅

---

## Key Concepts You Now Understand

✅ **Likelihood** = How probable is the threat?
✅ **Impact** = How damaging would it be?
✅ **Risk Score** = Likelihood × Impact (prioritization)
✅ **Treatment** = What to do about it
✅ **Owner** = Who's responsible
✅ **Status** = Progress tracking

This is **core GRC risk management**.

---

## Next Steps

1. ✅ Review the Risk Register
2. ✅ Understand each risk
3. ✅ Note the color-coding (Red=Critical, Orange=High, Yellow=Medium)
4. ✅ See how risks are prioritized by score
5. 🚀 Upload to GitHub
6. 📚 Day 4: Security Policies

---

**You're building a complete GRC toolkit.** 💪

Gap Analysis ✅ → Risk Register ✅ → Security Policies (tomorrow) → Done!
