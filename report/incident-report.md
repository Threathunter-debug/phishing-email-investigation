# Phishing Email Investigation Report

## Alert Summary

A phishing email investigation was initiated after multiple users received an email related to "Depression Screening EDA" originating from an external sender. The investigation focused on validating the legitimacy of the message, reviewing associated URLs, identifying impacted users, and determining whether malicious activity occurred.

---

# Investigation Details

## Initial Findings

- Multiple recipients received the email
- Email originated from an external source
- Embedded links redirected users to an external domain
- Similar emails were identified across the environment

---

# Analysis Performed

## Email Analysis

The email was reviewed within Microsoft Defender to analyze:

- Sender information
- Subject line
- Delivery action
- Authentication results
- Embedded URLs
- Related messages

---

## URL Investigation

URLs embedded within the email were reviewed for:

- Domain reputation
- Redirection behavior
- Potential phishing indicators
- User click activity

Additional validation was performed using threat intelligence and URL analysis platforms.

---

## Endpoint Investigation

Endpoint telemetry was reviewed using CrowdStrike Falcon to determine whether:

- Users accessed malicious content
- Suspicious processes executed
- Additional payloads were downloaded
- Network communication occurred

No evidence of malicious execution or secondary payload activity was identified during the investigation.

---

# IOC Review

The following indicators were reviewed:

- Sender email address
- Embedded URLs
- Associated domains
- Related email activity
- User interaction events

No confirmed malicious indicators were identified after analysis.

---

# Remediation Actions

The following actions were performed during containment and remediation:

- Investigated recipient exposure
- Reviewed related email activity
- Validated URL interaction events
- Performed endpoint review
- Documented findings and investigation results

---

# MITRE ATT&CK Mapping

| Technique | Description |
|---|---|
| T1566 | Phishing |
| T1204 | User Execution |
| T1071 | Application Layer Protocol |

---

# Final Determination

Investigation findings indicate the activity was reviewed and analyzed for phishing-related indicators. Based on available telemetry and endpoint analysis, no evidence of successful compromise or malicious payload execution was identified at the time of investigation.

---

# Analyst Notes

- Investigation performed using Microsoft Defender XDR, IBM QRadar, and CrowdStrike Falcon
- Threat hunting queries were used to validate user interaction and endpoint activity
- Screenshots and supporting investigation artifacts were documented within the repository
