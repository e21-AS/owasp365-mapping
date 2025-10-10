# 🔐 A02: Cryptographic Failures  
## 📁 Use Case: Outlook email with confidential contract sent without encryption

### 🎯 Scenario  
A legal advisor sends a draft contract containing sensitive client data via Outlook without applying encryption or Sensitivity Labels. The email may be intercepted during transit or forwarded to unintended recipients, exposing confidential information.

### ⚠️ OWASP Risk  
**A02: Cryptographic Failures**  
Failure to encrypt sensitive data in transit or at rest can result in data leakage and regulatory non-compliance.

### 🔍 Microsoft 365 Component  
- **Platform:** Outlook  
- **Feature at risk:** Email Transport / Sensitivity Labels  
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/outlook/)

### 💥 Potential Impact  
- Exposure of confidential legal or financial data  
- Breach of contractual confidentiality  
- Breach of GDPR or other data protection regulations

### 🛡️ Mitigation Strategies  
- Apply Sensitivity Labels to enforce encryption for sensitive emails and attachments (via Purview)
- Enforced TLS is enabled for email transport (via Outlook) 
- Educate users on secure email-handling practices (via Microsoft 365)

🔍 Search: Purview sensitivity labels site:learn.microsoft.com

🔍 Search: Outlook enabling TLS site:learn.microsoft.com

🔍 Search: Microsoft 365 email encryption site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A02`  
See also: `OWASP_M365_Mapping.md → A02 / Outlook`
