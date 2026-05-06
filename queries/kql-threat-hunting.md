# KQL Threat Hunting Queries

## Suspicious Email Investigation

```kql
EmailEvents
| where Subject contains "Depression Screening EDA"
| project Timestamp, SenderFromAddress, RecipientEmailAddress, Subject, DeliveryAction
```

---

## URL Investigation

```kql
UrlClickEvents
| where Url contains "ondemand.sas.com"
| project Timestamp, AccountUpn, Url, ActionType
```

---

## Similar Email Activity

```kql
EmailEvents
| where SenderFromAddress contains "replies-disabled@sas.com"
| summarize Count=count() by RecipientEmailAddress
```

---

## Endpoint Activity Validation

```kql
DeviceNetworkEvents
| where RemoteUrl contains "ondemand.sas.com"
| project Timestamp, DeviceName, InitiatingProcessFileName, RemoteUrl
```

---

## IOC Investigation

```kql
DeviceEvents
| where InitiatingProcessAccountName contains "user"
| where FileName contains ".html" or FileName contains ".zip"
```

---

## Investigation Purpose

These queries were used to:

- Identify recipients impacted by the email
- Review URL interaction activity
- Validate endpoint communication
- Investigate related email activity
- Perform IOC analysis
- Support phishing triage and containment actions
