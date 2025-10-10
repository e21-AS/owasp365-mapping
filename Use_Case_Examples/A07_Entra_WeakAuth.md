# 🧾 A07: Identification and Authentication Failures  
## 📁 Use Case: User logs in with weak password and no MFA

### 🎯 Scenario  
An employee accesses Microsoft 365 services using a weak password that has been reused across multiple platforms. The account is not protected by multi-factor authentication (MFA). An attacker obtains the password through a credential-stuffing attack and successfully logs in, gaining access to sensitive emails and SharePoint files.

### ⚠️ OWASP Risk
**A07: Identification and Authentication Failures**
Weak or missing authentication mechanisms allow attackers to compromise accounts and access protected resources.

### 🔍 Microsoft 365 Component
- **Platform:** Entra ID
- **Feature at risk:** Password Policy / Multi-Factor Authentication  
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/entra/identity/)

### 💥 Potential Impact
- Unauthorised access to sensitive emails, documents, and Teams conversations
- Data leakage or manipulation
- Escalation to privileged roles or lateral movement across services

### 🛡️ Mitigation Strategies  
- Enforce MFA for all users through Conditional Access policies (via Entra ID)
- Apply strong password policies and block known compromised passwords (via Entra ID)
- Monitor sign-in activity and risky logins through Entra ID Identity Protection 
- Educate users on secure authentication practices and phishing awareness (via Microsoft 365)

🔍 Search: Entra ID MFA enforcement site:learn.microsoft.com

🔍 Search: Microsoft 365 password policy site:learn.microsoft.com

🔍 Search: Entra ID risky sign-ins site:learn.microsoft.com

🔍 Search: Microsoft 365 phishing protection site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A07`  
See also: `OWASP_M365_Mapping.md → A07 / Entra ID`
