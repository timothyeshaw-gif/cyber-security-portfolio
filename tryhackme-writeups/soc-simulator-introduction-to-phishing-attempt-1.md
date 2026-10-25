# TryHackMe SOC Simulator - Phishing Alert Investigation

## Overview

This SOC Simulator exercise provided hands-on experience investigating and classifying security alerts within a simulated Security Operations Centre (SOC) environment.

The scenario required analysing multiple alerts, distinguishing true positives from false positives, assessing the severity of identified threats, and documenting findings to support security operations and incident response.

The investigation focused primarily on phishing-related activity, alongside the analysis of a high-severity firewall alert.

---

## Investigation Objectives

The objectives of the exercise were to:

- Analyse and investigate security alerts.
- Determine whether alerts represented genuine threats.
- Differentiate true positives from false positives.
- Assess the severity and potential impact of identified threats.
- Document investigation findings.
- Recommend appropriate actions and escalation decisions.

---

## Scenario Results

### Investigation Outcome

✅ Security Breach Prevented

### Detection Accuracy

| Metric | Result |
|----------|----------|
| True Positive Identification Rate | 100% |
| False Positive Identification Rate | 100% |

### Operational Metrics

| Metric | Result |
|----------|----------|
| Alerts Investigated | 4 |
| Mean Time To Resolve (MTTR) | 3 Minutes |
| Mean Dwell Time | 12 Minutes |

---

## Alerts Investigated

| Alert ID | Alert Description | Severity | Category | Result |
|-----------|-------------------|------------|-----------|----------|
| 8816 | Access to Blacklisted External URL Blocked by Firewall | High | Firewall | Correctly Classified |
| 8815 | Inbound Email Containing Suspicious External Link | Medium | Phishing | Correctly Classified |
| 8817 | Inbound Email Containing Suspicious External Link | Medium | Phishing | Correctly Classified |
| 8814 | Inbound Email Containing Suspicious External Link | Medium | Phishing | Correctly Identified as False Positive |

---

## Skills Demonstrated

- Alert triage
- Security event investigation
- Phishing analysis
- Firewall alert analysis
- Threat detection
- Evidence gathering
- Security reporting
- Incident classification
- Escalation decision making
- Risk assessment

---

## Investigation Process

### Alert Review

Each alert was reviewed to understand the nature of the reported activity and identify potential indicators of compromise.

### Evidence Analysis

Available evidence was analysed to determine whether activity was malicious, suspicious or benign.

### Threat Validation

Alert data was assessed against investigation findings to establish whether alerts represented genuine security threats.

### Classification

Alerts were accurately classified as either true positives or false positives based on the evidence available.

### Reporting

Investigation outcomes were documented and recommendations were provided to support security operations and incident response activities.

---

## Feedback and Lessons Learned

The simulator feedback identified several strengths:

- Strong identification of true positive alerts.
- Strong identification of false positive alerts.
- Accurate alert classification.
- Effective investigation methodology.

The feedback also highlighted opportunities for improvement in:

- Remediation recommendations.
- Escalation justification.
- Report depth and context.
- Completion of recommended actions within investigation reports.

These findings provided valuable insight into the importance of effective communication and reporting within a SOC environment.

---

## Reflection

This was my first SOC Simulator investigation and provided practical experience analysing and responding to security alerts in a realistic SOC environment.

I successfully achieved a 100% true positive identification rate and a 100% false positive identification rate across all alerts within the scenario. The exercise involved investigating phishing-related activity and a high-severity firewall event while applying a structured approach to alert triage and incident classification.

During the investigation I used the DetectMe guidance feature when required. Rather than relying on guesswork, I used the available guidance to better understand the investigation workflow and reinforce good analytical practices. This helped me understand how playbooks and analyst guidance can support junior analysts when handling unfamiliar alerts.

The exercise also reinforced the importance of strong documentation and reporting. Whilst the alert classifications were accurate, the feedback demonstrated that remediation recommendations and escalation reasoning can be improved. This highlighted the need to communicate findings clearly and provide actionable recommendations for follow-on teams.

Overall, the simulation increased my confidence in alert triage, phishing investigations and security event analysis while identifying clear areas for continued development.

---

## Key Learning Outcomes

After completing this exercise I can:

- Investigate phishing-related security alerts.
- Differentiate true positives from false positives.
- Follow a structured alert triage process.
- Assess the severity and impact of security events.
- Analyse firewall and phishing alerts.
- Document investigation findings.
- Understand the importance of remediation recommendations.
- Support incident response through accurate reporting.

---

## Workplace Application

The skills demonstrated during this exercise are directly applicable to the responsibilities of a Tier 1 SOC Analyst, including:

- Monitoring security alerts.
- Investigating suspicious activity.
- Analysing phishing threats.
- Identifying indicators of compromise (IOCs).
- Determining escalation requirements.
- Supporting incident response processes.
- Maintaining investigation records and audit trails.

---

## Next Steps

Following this exercise I plan to continue developing practical SOC analyst skills through:

- Splunk SIEM investigations
- Alert triage scenarios
- Threat hunting exercises
- Phishing analysis investigations
- MITRE ATT&CK mapping
- Cyber Kill Chain analysis
- Incident response exercises
- Security reporting and documentation

My goal is to improve both the technical and reporting aspects of investigations while developing proficiency with Splunk and other SOC tooling.

---

## Technologies and Concepts

- Security Operations Centre (SOC)
- Phishing Analysis
- Alert Triage
- Security Monitoring
- Firewall Investigation
- Incident Response
- Threat Detection
- Security Reporting
- Evidence Gathering
- Risk Assessment

---

## Career Relevance

This exercise provided practical experience aligned with the responsibilities of:

- SOC Analyst
- Cyber Security Analyst
- Incident Response Analyst
- Blue Team Analyst
- Security Monitoring Analyst

The simulation offered hands-on experience investigating alerts, validating threats and documenting findings, mirroring the activities commonly performed within operational security teams.
