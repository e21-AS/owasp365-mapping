# 🕵️ A09: Security Logging and Monitoring Failures
## 📁 Use Case: Purview audit logs not enabled for Microsoft 365 services

### 🎯 Scenario
An organisation uses Microsoft 365 services such as SharePoint, Outlook, and Teams for daily operations. However, Purview audit logging is not enabled or configured. Suspicious activities - including external sharing, mailbox rule changes, and unusual sign-in patterns - go undetected due to insufficient visibility and alerting.

### ⚠️ OWASP Risk
**A09: Security Logging and Monitoring Failures**  
Insufficient logging and monitoring prevent timely detection of, and response to, suspicious or malicious activity.

### 🔍 Microsoft 365 Component  
- **Platform:** Microsoft Purview
- **Feature at risk:** Audit Logging / Activity Monitoring
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/purview/audit-search)

### 💥 Potential Impact  
- Failure to detect data exfiltration or account compromise
- Inability to investigate incidents or meet compliance requirements
- Delayed response to insider threats or external attacks

### 🛡️ Mitigation Strategies
- Enable unified audit logging across all Microsoft 365 services (via Purview)
- Configure alerts for high-risk activities, such as external sharing or mailbox rule changes
- Integrate audit logs with Defender XDR or a SIEM solution for centralised monitoring
- Regularly review audit log retention settings and access controls

🔍 Search: Purview audit log configuration site:learn.microsoft.com

🔍 Search: Microsoft 365 unified audit logging site:learn.microsoft.com

🔍 Search: Defender XDR audit integration site:learn.microsoft.com

🔍 Search: Microsoft 365 SIEM integration site:learn.microsoft.com

### 📌 Related
See also: `Mitigation_Strategies.md → A09`  
See also: `OWASP_M365_Mapping.md → A09 / Purview`
