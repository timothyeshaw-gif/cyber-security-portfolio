# Incident Response Plan: Critical PHP Vulnerabilities (CVE-2026-109618 & CVE-2026-109619)

## Scenario

An organisation has identified that its public-facing web servers are running vulnerable versions of PHP affected by critical remote code execution vulnerabilities.

The vulnerabilities could allow unauthenticated attackers to execute malicious code on affected systems, potentially leading to:

- Unauthorised system access
- Data theft
- Service disruption
- Malware installation
- Website defacement

The organisation activates its Incident Response Plan following notification from the National Cyber Security Centre (NCSC) and the PHP Security Team.

Reference:
- https://www.ncsc.gov.uk/news/critical-security-issue-affecting-php

---

# Incident Response Checklist

- [ ] Review NCSC and vendor security advisories
- [ ] Identify affected systems
- [ ] Assess business impact
- [ ] Collect evidence
- [ ] Implement containment measures
- [ ] Apply security patches
- [ ] Verify remediation
- [ ] Restore services
- [ ] Complete incident report
- [ ] Conduct lessons learned review

---

# 0. Preparation

## Objectives

Ensure the organisation is ready to respond before exploitation occurs.

## Actions

1. Review NCSC guidance and vendor advisories.
2. Confirm asset inventories are up to date.
3. Verify vulnerability scanning coverage.
4. Review the Incident Response Plan and associated checklists.
5. Confirm contact details for key responders.
6. Validate backup integrity and recovery procedures.
7. Brief management and technical teams on the potential risk.
8. Ensure monitoring and alerting systems are functioning correctly.

## Evidence to Collect

- Asset inventory records
- Vulnerability management reports
- Backup validation reports
- Security monitoring dashboards
- Incident response procedures

---

# 1. Identification

## Objectives

Determine:

- Whether vulnerable PHP versions are present
- Which systems are affected
- Whether exploitation has occurred
- The potential business impact

## Actions

1. Review NCSC and vendor security advisories.
2. Identify all systems running PHP.
3. Review software inventory records.
4. Prioritise internet-facing services.
5. Check server logs for suspicious activity.
6. Review threat intelligence sources.
7. Assess vulnerability severity using CVSS scores.
8. Notify management and the cyber security team.

## Evidence to Collect

- Asset inventory
- Vulnerability scan reports
- Web server logs
- Security monitoring alerts
- Threat intelligence reports
- Screenshots of findings
- Audit records

---

# 2. Containment

## Objectives

Prevent attackers from exploiting affected systems while remediation activities take place.

## Short-Term Containment

Short-term containment actions are designed to quickly reduce risk and prevent further compromise.

### If patching can be completed quickly

- Apply security updates immediately.
- Restrict access to administration interfaces.
- Increase monitoring of affected systems.

### If patching cannot be completed immediately

- Remove affected services from the internet.
- Disable vulnerable applications.
- Apply temporary vendor mitigations.
- Implement firewall restrictions.
- Restrict administrative access.

## Long-Term Containment

Long-term containment measures allow business operations to continue while reducing risk.

Examples include:

- Moving systems into isolated network segments.
- Increasing monitoring and logging.
- Implementing temporary security controls.
- Restricting access to vulnerable services.

## Trade-Off Considerations

Incident responders often need to balance security against business needs.

Examples include:

| Option | Benefit | Trade-Off |
|----------|----------|----------|
| Shut down a compromised web server | Prevents further exploitation | Service becomes unavailable |
| Leave service running under enhanced monitoring | Maintains availability | Increased risk of compromise |
| Restrict access to administrative interfaces | Reduces attack surface | Reduced operational flexibility |

For example, a healthcare organisation such as the NHS may need to balance the need to protect systems against the need to maintain access to critical patient services.

## Roles and Responsibilities

| Role | Responsibility |
|---------|---------|
| Incident Manager | Coordinates response |
| System Administrator | Applies patches |
| SOC Analyst | Monitors activity |
| Communications Lead | Internal updates |
| Senior Management | Risk decisions |

---

# 3. Eradication

## Objectives

Remove vulnerabilities and any evidence of compromise.

## Actions

1. Upgrade PHP to a secure supported version.
2. Remove temporary workarounds that are no longer required.
3. Review web server configurations.
4. Remove unauthorised accounts.
5. Scan for malware and web shells.
6. Review scheduled tasks and persistence mechanisms.
7. Verify the integrity of critical files.
8. Reassess systems using vulnerability scanning tools.

## Validation

Confirm:

- Vulnerabilities are no longer detected.
- Systems pass security scans.
- No indicators of compromise remain.
- Security controls are operating correctly.

---

# 4. Recovery

## Objectives

Safely return systems to normal operation.

## Actions

1. Restore services in stages.
2. Continuously monitor logs.
3. Validate system functionality.
4. Verify customer access.
5. Test business processes.
6. Confirm backups remain valid.
7. Monitor for signs of reinfection or further malicious activity.

## Re-Testing

Before the incident can be formally closed, systems should be re-tested to ensure:

- Vulnerabilities have been successfully addressed.
- Security controls are functioning correctly.
- Business services operate as expected.
- No indicators of compromise remain.

This creates a continuous improvement cycle and helps verify that remediation activities have been effective.

## Success Criteria

- Website operational
- No signs of exploitation
- Security monitoring functioning
- Business services restored
- Vulnerabilities no longer detected

---

# 5. Lessons Learned

## Objectives

Review the incident, identify improvements, and strengthen future resilience.

## Post-Incident Review Questions

### What worked well?

- Rapid identification?
- Accurate asset inventory?
- Effective communication?
- Successful patch deployment?

### What could be improved?

- Patch deployment speed?
- Vulnerability scanning coverage?
- Monitoring capability?
- Incident communications?

### Long-Term Improvements

- Improve asset management.
- Reduce technical debt.
- Implement automated patching.
- Enhance vulnerability scanning.
- Improve monitoring and alerting.
- Review incident response procedures.
- Update incident response checklists.

This reflects the NCSC observation that organisations must maintain visibility of vulnerable assets and address technical debt to improve resilience.

## Documentation

Following the incident, the organisation should produce:

- Incident report
- Timeline of events
- Audit trail of decisions and actions
- Lessons learned report
- Updated Incident Response Plan
- Updated response checklists

---

# Mapping to Cyber Security Concepts

## CIA Triad

### Confidentiality

Prevent attackers from accessing sensitive information.

### Integrity

Prevent unauthorised modification of website code, data, and configurations.

### Availability

Maintain services where safe to do so, or temporarily remove systems from operation to protect the wider environment.

---

## NIST Incident Response Lifecycle

| Stage | Example Activities |
|---------|---------|
| Preparation | Asset inventory, monitoring, backups, response planning |
| Detection and Analysis | Identify vulnerable systems, assess impact |
| Containment, Eradication and Recovery | Restrict access, patch vulnerabilities, restore services |
| Post-Incident Activity | Lessons learned review, reporting, process improvements |

---

## PICERL Mapping

| Stage | Actions |
|---------|---------|
| Preparation | Asset inventory, monitoring, response procedures |
| Identification | Identify vulnerable systems |
| Containment | Restrict access and isolate systems |
| Eradication | Patch vulnerabilities and remove threats |
| Recovery | Restore services and monitor systems |
| Lessons Learned | Conduct reviews and update procedures |

---

# Skills Demonstrated

- Incident response planning
- Vulnerability management
- Threat intelligence analysis
- Security monitoring
- Evidence collection
- Audit trail management
- Risk assessment
- Patch management
- Recovery planning
- Lessons learned reviews

---

# Reflection

This incident demonstrates the importance of having an effective incident response capability and a well-maintained Incident Response Plan supported by detailed checklists. The organisation was required to identify vulnerable systems, assess business risk, collect evidence, apply mitigations, and restore services whilst maintaining security and business continuity.

The incident also highlights the importance of vulnerability management, asset discovery, security monitoring, and patch management as key components of organisational cyber resilience. Maintaining accurate inventories and reducing technical debt makes it significantly easier to identify affected systems and respond quickly when critical vulnerabilities are disclosed.

Finally, this scenario demonstrates the importance of following guidance from trusted sources such as the National Cyber Security Centre (NCSC) and maintaining a security-by-design mindset throughout the software lifecycle.
