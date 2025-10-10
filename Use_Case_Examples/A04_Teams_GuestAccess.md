# 🧩 A04: Insecure Design  
## 📁 Use Case: External guest added to internal Teams channel with access to sensitive files

### 🎯 Scenario  
A project manager adds an external guest to an internal Microsoft Teams channel used for strategic project planning. The guest gains access to shared files in SharePoint and OneDrive, including confidential financial forecasts and internal presentations. No granular access restrictions are applied.

### ⚠️ OWASP Risk  
**A04: Insecure Design**  
Failure to design systems with security controls that anticipate misuse or abuse, particularly in collaborative environments.

### 🔍 Microsoft 365 Component  
- **Platform:** Microsoft Teams  
- **Feature at risk:** Guest Access / File Sharing  
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/microsoftteams/)

### 💥 Potential Impact  
- Exposure of internal strategic documents  
- Loss of confidentiality or competitive advantage  
- Breach of internal collaboration policies or non-disclosure agreements (NDAs)

### 🛡️ Mitigation Strategies  
- Apply guest access policies to limit the scope of access (via Entra ID / Microsoft Teams)  
- Use dedicated Teams or channels for external collaboration, configured with restricted permissions 
- Monitor guest activity and sharing behaviour through audit logs and alerts (via Purview)
- Apply Sensitivity Labels to automatically restrict guest sharing within SharePoint teams and sites that contain sensitive data (via Purview)

🔍 Search: Teams guest access policies site:learn.microsoft.com

🔍 Search: Entra ID guest restrictions site:learn.microsoft.com

🔍 Search: Purview audit logs for Teams site:learn.microsoft.com

🔍 Search: Purview Sensitivity Labels for Teams site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A04`  
See also: `OWASP_M365_Mapping.md → A04 / Teams`
