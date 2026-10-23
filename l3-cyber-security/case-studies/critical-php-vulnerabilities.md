# Critical PHP Vulnerabilities (2026)

## Overview

In October 2026, researchers identified two critical vulnerabilities affecting PHP, one of the world's most widely used web programming languages.

The vulnerabilities could potentially allow an attacker to achieve **unauthenticated Remote Code Execution (RCE)** on web servers running PHP. This means an attacker may be able to execute malicious commands on a server without requiring valid credentials.

The vulnerabilities were assigned the following CVE identifiers:

- CVE-2026-109618
- CVE-2026-109619

The discovery led organisations worldwide to take websites and services offline while patches were applied. The UK Government confirmed that 32 government services became unavailable as a precautionary measure.

---

## Learning Objectives

This case study demonstrates:

- Vulnerability Management
- Threat Intelligence
- CVE Analysis
- CVSS Assessment
- Risk Management
- Security by Design
- Incident Response
- Patch Management
- AI-Assisted Security Research

---

## What is PHP?

PHP (PHP Hypertext Preprocessor) is a server-side scripting language used to create dynamic websites and web applications.

PHP is commonly used for:

- WordPress websites
- E-commerce platforms
- Content Management Systems (CMS)
- Web applications
- Database-driven websites

The National Cyber Security Centre (NCSC) noted that PHP is widely used throughout the internet and is embedded in many third-party products and services.

---

## Technical Explanation

### CVE-2026-109618

This vulnerability occurs during an out-of-memory condition.

When PHP runs out of available memory while processing a request, internal data structures may only be partially initialised. During cleanup operations, invalid data may be incorrectly processed as legitimate data, resulting in memory corruption.

### CVE-2026-109619

This vulnerability involves stale internal state data.

PHP may continue using information that should have been removed from memory after a previous request. A later request handled by the same worker process could exploit this condition, leading to memory corruption and potentially Remote Code Execution.

---

## CVSS Severity Assessment

The two PHP vulnerabilities, **CVE-2026-109618** and **CVE-2026-109619**, were each reported as having a **CVSS score of 9.2 (Critical)**.

A CVSS score above 9.0 represents a critical vulnerability and indicates that immediate remediation is required.

### CVSS v4 Metrics

| Metric | Value | Explanation |
|----------|----------|----------|
| Attack Vector | Network | The vulnerability can be exploited remotely over a network. |
| Attack Complexity | High | Successful exploitation requires specific conditions and technical expertise. |
| Attack Requirements | Present | Certain environmental conditions must exist for exploitation to succeed. |
| Privileges Required | None | An attacker does not require a user account or prior access. |
| User Interaction | None | No action is required from a legitimate user. |
| Confidentiality Impact | High | Sensitive information could potentially be exposed. |
| Integrity Impact | High | Data, files, or configurations could be modified. |
| Availability Impact | High | Services could be disrupted or rendered unavailable. |
| Subsequent Confidentiality Impact | None | No direct impact is expected on connected systems. |
| Subsequent Integrity Impact | None | No direct impact is expected on connected systems. |
| Subsequent Availability Impact | None | No direct impact is expected on connected systems. |

### Analysis of the CVSS Score

Although the vulnerabilities have a **High Attack Complexity**, they remain critical because exploitation does not require authentication, elevated privileges, or user interaction. This means an attacker could potentially attempt exploitation remotely against internet-facing systems without assistance from a legitimate user.

The vulnerabilities have a **High impact across all three elements of the CIA Triad**:

- **Confidentiality** – attackers may gain access to sensitive information.
- **Integrity** – attackers may modify files, databases, or application content.
- **Availability** – attackers may disrupt or disable services.

The combination of remote exploitation, lack of authentication requirements, and high impact on confidentiality, integrity and availability contributed to the critical severity rating and explains why many organisations chose to temporarily remove services from the internet while security updates were applied.

### Relevance to Cyber Security

This incident demonstrates that vulnerability severity is not determined solely by exploit difficulty.

Although the attack complexity was classified as High, the vulnerabilities remained critical because no authentication, user interaction, or prior compromise was required. If exploitation was successful, an attacker could potentially impact confidentiality, integrity and availability simultaneously.

This demonstrates why cyber security professionals must consider both the likelihood and potential impact of exploitation when assessing risk.

---

## Why Was This So Serious?

This incident was significant because:

- PHP powers a substantial proportion of the internet.
- The vulnerabilities existed within PHP itself rather than a single application.
- Exploitation could occur without authentication.
- Attackers could potentially gain control of affected servers.
- Many organisations were unaware of where PHP was being used within their environment.
- Both vulnerabilities were assigned a **CVSS score of 9.2 (Critical)**.

This created a supply-chain-style challenge because organisations had to identify both direct PHP installations and products that used PHP as an underlying component.

---

## Artificial Intelligence in Vulnerability Research

One of the most significant aspects of this incident was that the vulnerabilities were reportedly discovered with the assistance of advanced AI systems.

Researchers used AI-assisted techniques to identify flaws that may have existed within PHP for many years. This gave defenders time to produce patches and mitigation measures before any widespread exploitation was identified.

### Benefits

- Faster vulnerability discovery
- Enhanced code analysis
- Earlier defensive action
- Improved vulnerability research

### Risks

- Criminals may use AI to identify vulnerabilities.
- Exploit development may become increasingly automated.
- Vulnerabilities may be weaponised more quickly.
- Security teams may have shorter response windows.

---

## Cyber Security Principles Demonstrated

### Vulnerability Management

Organisations were required to:

- Identify affected systems
- Assess risk exposure
- Apply security updates
- Monitor for signs of compromise

This is a practical example of vulnerability management in action.

### Defence in Depth

Many organisations reduced risk by:

- Temporarily taking systems offline
- Restricting public access
- Monitoring exploitation attempts
- Implementing additional mitigations

This demonstrates multiple layers of security controls rather than relying solely on patching.

### Security by Design

The incident highlights the importance of:

- Secure coding practices
- Memory safety
- Secure software development
- Continuous security testing

Had these vulnerabilities been identified earlier during development, the impact could have been significantly reduced.

### Risk Management

Some organisations chose to temporarily reduce availability in order to protect confidentiality and integrity.

#### CIA Triad

| Principle | Example |
|------------|------------|
| Confidentiality | Preventing unauthorised server access |
| Integrity | Preventing malicious modification of systems |
| Availability | Temporary service disruption while security updates were applied |

---

## Impact on the United Kingdom

According to public reports:

- 32 Government services became unavailable.
- 4 Government services operated with reduced functionality.
- Several local authorities took websites offline.
- NHS and other public-sector organisations implemented precautionary measures.
- No confirmed successful breaches were reported during the initial response period.

---

## Lessons Learned

This incident demonstrates that organisations should:

1. Maintain accurate asset inventories.
2. Understand software dependencies.
3. Apply security patches promptly.
4. Monitor threat intelligence sources such as the NCSC.
5. Develop incident response plans.
6. Reduce technical debt where possible.
7. Adopt Security by Design principles throughout the software lifecycle.

---

## Personal Reflection

This incident demonstrates how vulnerabilities within widely used technologies can create global consequences within a short period of time.

The PHP vulnerability event reinforced the importance of vulnerability management, threat intelligence, risk assessment, patch management, and incident response. It also highlighted the growing role of Artificial Intelligence within cyber security, both as a defensive capability and as a potential force multiplier for attackers.

From a cyber security perspective, this case study demonstrates the importance of maintaining visibility of organisational assets, understanding software dependencies, and responding rapidly to emerging threats.

---

## References

1. National Cyber Security Centre (NCSC) - Critical Security Issue Affecting PHP
2. BBC News - Websites Worldwide Taken Offline Following Critical PHP Vulnerabilities
3. Digital Health News - Cyber Alert Forces NHS Scotland Websites Temporarily Offline
4. PHP Foundation Security Advisory
