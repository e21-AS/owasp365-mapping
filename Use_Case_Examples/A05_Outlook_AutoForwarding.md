# ⚙️ A05: Security Misconfiguration
## 📁 Use Case: Outlook mailbox rule auto-forwards all emails to external address

### 🎯 Scenario
A user creates an Outlook mailbox rule that automatically forwards all incoming emails to a personal Gmail account. The rule is neither reviewed nor restricted by administrators. Sensitive internal communications, including financial reports and client data, are continuously forwarded outside the organisation without detection.

### ⚠️ OWASP Risk
**A05: Security Misconfiguration**  
Security settings are left in insecure states or are misconfigured, allowing unintended data exposure or system behaviour.

### 🔍 Microsoft 365 Component
- **Platform:** Outlook
- **Feature at risk:** Mailbox Rules / External Forwarding
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/outlook/)

### 💥 Potential Impact  
- Continuous leakage of sensitive internal communications
- Breach of data protection policies or contractual obligations 
- Increased risk of phishing or business email compromise (BEC)

### 🛡️ Mitigation Strategies  
- Disable external auto-forwarding rules through Exchange Online transport settings
- Monitor mailbox rule creation and changes using audit logs (via Purview)
- Apply DLP policies to detect and block sensitive content from leaving the organisation
- Educate users on secure mailbox configurations and how to report suspicious rules (via Microsoft 365)

🔍 Search: Outlook mailbox forwarding restrictions site:learn.microsoft.com

🔍 Search: Exchange Online transport rules site:learn.microsoft.com

🔍 Search: Purview audit mailbox rules site:learn.microsoft.com

🔍 Search: Microsoft 365 DLP for email site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A05`  
See also: `OWASP_M365_Mapping.md → A05 / Outlook`
