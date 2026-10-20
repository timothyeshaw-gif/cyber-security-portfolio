# ✈️ British Airways Data Breach (2018)

## 📌 Overview

The **British Airways data breach (2018)** is one of the most significant cyber incidents in UK history and is often cited as a textbook example of how **UK GDPR** and the **Data Protection Act 2018** are enforced in practice.

Between **June and September 2018**, attackers compromised British Airways' website and mobile application, exposing personal and financial data belonging to approximately **429,000 customers**.

---

## 📊 Incident Summary

| Category | Details |
|-----------|----------|
| Organisation | British Airways |
| Date | June–September 2018 |
| Attack Type | Website and mobile application compromise |
| Data Affected | Personal and financial data |
| Number of Individuals Affected | Approximately 429,000 customers |

The attackers injected malicious code into British Airways' booking systems, allowing customer information to be captured during transactions.

---

## 🔍 Cause of the Breach

The breach occurred because British Airways' website and mobile application were not adequately secured.

Attackers exploited vulnerabilities in third-party scripts used during payment processing and were able to skim sensitive customer information directly from transactions.

The attack highlighted weaknesses in:

- Third-party security management
- Website security controls
- Security monitoring
- Application protection

---

## ⚖️ Legal and Regulatory Outcome

The incident was investigated by the **Information Commissioner's Office (ICO)** under:

- UK GDPR
- Data Protection Act 2018

The ICO concluded that British Airways had inadequate security arrangements which contributed to the compromise of customer data.

Key findings included:

- Insufficient security monitoring
- Weak access controls
- Inadequate protection of customer information
- Lack of Multi-Factor Authentication (MFA)

### Enforcement Action

| Item | Result |
|---------|---------|
| Initial Proposed Fine | £183 million |
| Final Fine Issued | £20 million |
| Regulator | Information Commissioner's Office (ICO) |

At the time, the £20 million penalty was the largest fine ever issued by the ICO.

British Airways was also required to strengthen its cyber security controls and improve its breach-response procedures.

---

## 🧠 Key Lessons for Cyber Security

| Area | Lesson |
|---------|---------|
| Data Protection | Organisations must monitor and secure customer data throughout its lifecycle. |
| Third-Party Risk | Suppliers and external scripts must be assessed and secured appropriately. |
| Incident Response | Significant breaches must be identified, investigated, and reported promptly. |
| Accountability | Senior management must ensure effective governance and risk management. |

---

## ⏱ GDPR Breach Reporting Requirements

One of the key GDPR requirements highlighted by the incident is the obligation to report qualifying personal data breaches within **72 hours** of becoming aware of them.

Organisations should maintain:

- Incident response plans
- Escalation procedures
- Communication plans
- Regulatory reporting procedures

---

## 🌍 Impact on the Cyber Security Sector

The British Airways breach demonstrated that GDPR has genuine enforcement power.

The incident shifted cyber security from being viewed solely as a technical issue to being recognised as a broader:

- Legal issue
- Governance issue
- Risk management issue
- Compliance issue

Following the breach, many organisations reviewed:

- Data handling procedures
- Supplier risk management processes
- Security monitoring capabilities
- Breach reporting procedures

---

## 🔬 Technical Findings

Investigations identified several important technical details.

### Third-Party Script Compromise

Attackers compromised a third-party JavaScript library used by British Airways' website and mobile application.

### Malicious Modernizr File

The attackers injected malicious code into a modified **Modernizr** file.

The malicious script was only **22 lines long** but successfully captured customer payment card details.

### Data Exfiltration

The stolen information was sent to an attacker-controlled domain named:

```text
baways.com
```

The domain was designed to closely resemble British Airways branding and infrastructure.

### Missing Security Controls

Investigators found that British Airways lacked:

#### Subresource Integrity (SRI)

Subresource Integrity helps verify that externally loaded scripts have not been modified or tampered with.

#### Content Security Policy (CSP)

Content Security Policy helps prevent malicious scripts from loading or transmitting information to unauthorised destinations.

These controls may have helped detect or prevent the attack.

---

## 🛡️ Governance and Risk Management Perspective

The British Airways breach demonstrates that cyber security is not solely a technical issue.

The incident exposed weaknesses in:

- Security governance
- Third-party risk management
- Continuous monitoring
- Compliance oversight
- Security controls

The regulatory outcome showed that organisations can face serious legal, financial, and reputational consequences when appropriate controls are not in place.

---

## 📝 Key Learning Points

Through studying the British Airways breach I have learned that:

- Cyber security failures can result in significant regulatory penalties.
- Third-party systems and suppliers introduce additional security risks.
- Governance and compliance are essential components of cyber security.
- Effective monitoring is critical for detecting attacks.
- Security controls must be regularly reviewed and updated.
- GDPR compliance requires both technical and organisational security measures.

---

## 💡 Reflection

The British Airways data breach provides a practical example of how security failures, governance weaknesses, and poor risk management can lead to regulatory action.

This case study has strengthened my understanding of:

- Data Protection
- GDPR Compliance
- Third-Party Risk
- Security Governance
- Incident Response
- Risk Management

The lessons learned are particularly relevant to careers in:

- Governance, Risk and Compliance (GRC)
- Security Consultancy
- Information Security
- Security Operations (SOC)
- Risk Management
