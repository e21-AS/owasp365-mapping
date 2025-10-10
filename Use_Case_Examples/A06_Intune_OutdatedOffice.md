# 🧱 A06: Vulnerable and Outdated Components
## 📁 Use Case: User device runs outdated Office version lacking recent security patches

### 🎯 Scenario
An employee uses a personal laptop to access Microsoft 365 services. The device runs an outdated version of Microsoft Office that has not received recent security updates. Owing to missing patches, the system becomes vulnerable to known exploits targeting Office macros and legacy components.
### ⚠️ OWASP Risk
**A06: Vulnerable and Outdated Components**
Failure to update software components exposes systems to known vulnerabilities that may be exploited by attackers.

### 🔍 Microsoft 365 Component
- **Platform:** Microsoft Office (via Intune / Microsoft 365 Apps)
- **Feature at risk:** Office Version / Update Compliance
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/microsoft-365/?view=o365-worldwide)

### 💥 Potential Impact
- Exploitation of known vulnerabilities in Office macros or legacy features
- Unauthorized access to sensitive documents or credentials
- Lateral movement within the organisation through compromised endpoints

### 🛡️ Mitigation Strategies
- Enforce automatic updates for Microsoft 365 Apps for Enterprise (via Intune)
- Set minimum supported Office version using compliance policies (via Microsoft 365)
- Monitor update status and patch compliance across all enrolled devices
- Restrict access to Microsoft 365 services from non-compliant or unmanaged devices using Conditional Access policies
  
🔍 Search: Intune Office update compliance site:learn.microsoft.com

🔍 Search: Microsoft 365 Apps minimum version policy site:learn.microsoft.com

🔍 Search: Intune patch management site:learn.microsoft.com

🔍 Search: Conditional access for unmanaged devices site:learn.microsoft.com

### 📌 Related
See also: `Mitigation_Strategies.md → A06`  
See also: `OWASP_M365_Mapping.md → A06 / Microsoft Office`
