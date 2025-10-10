# 🛑 A01: Broken Access Control  
## 📁 Use Case: OneDrive file shared via "Anyone with the link"

### 🎯 Scenario  
An HR employee uploads a document containing salary data to OneDrive and shares it using the "Anyone with the link" option. The link is accidentally forwarded outside the organisation, exposing sensitive information to unauthorised parties.

### ⚠️ OWASP Risk  
**A01: Broken Access Control**  
Improper access configuration allows unauthorised users to retrieve sensitive data.

### 🔍 Microsoft 365 Component  
- **Platform:** OneDrive
- **Feature at risk:** Anonymous Sharing
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/onedrive/)

### 💥 Potential Impact  
- Exposure of confidential HR data  
- Violation of internal data handling policies  
- Potential GDPR or compliance breach

### 🛡️ Mitigation Strategies  
- Enforce device-based access authentication and make it available only for approved guest users or security groups (via Entra ID / Microsoft 365) 
- Disable "Anyone with the link" sharing organisation-wide (via OneDrive)
- Monitor external sharing with Audit Logs and Sharing Alerts at scale (via Purview)

🔍 Search: Entra ID access authentication site:learn.microsoft.com

🔍 Search: OneDrive shareable links site:learn.microsoft.com  

🔍 Search: OneDrive anonymous sharing site:learn.microsoft.com

🔍 Search: Purview monitoring external sharing site:learn.microsoft.com

🔍 Search: Purview Audit Log site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A01`  
See also: `OWASP_M365_Mapping.md → A01 / OneDrive`
