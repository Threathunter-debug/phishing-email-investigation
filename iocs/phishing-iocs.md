# Indicators of Compromise (IOCs)

## Investigation Overview

The following indicators were identified and reviewed during the phishing email investigation.

---

# Email Indicators

| Indicator Type | Value | Status |
|---|---|---|
| Subject | Depression Screening EDA | Reviewed |
| Sender Address | replies-disabled@sas.com | Reviewed |
| Delivery Method | External Email | Reviewed |

---

# URL Indicators

| Indicator Type | Value | Status |
|---|---|---|
| URL | ondemand.sas.com | Analyzed |
| URL Reputation | No confirmed malicious activity identified | Reviewed |

---

# Domain Indicators

| Indicator Type | Value | Status |
|---|---|---|
| Domain | sas.com | Reviewed |
| External Redirection | Observed during investigation | Reviewed |

---

# User Activity Indicators

| Indicator Type | Status |
|---|---|
| URL Click Activity | Reviewed |
| Endpoint Activity | Reviewed |
| Related Email Activity | Reviewed |

---

# Endpoint Investigation

The following endpoint telemetry was reviewed during the investigation:

- Network communication events
- Process execution activity
- User interaction events
- Related security telemetry

No confirmed malicious payload execution or persistence activity was identified.

---

# IOC Analysis Outcome

Investigation findings determined that the reviewed indicators did not demonstrate evidence of confirmed malicious execution or compromise at the time of analysis.

All findings were documented and validated through Microsoft Defender XDR, CrowdStrike Falcon, and SIEM investigation workflows.
