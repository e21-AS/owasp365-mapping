# 🧪 A08: Software and Data Integrity Failures
## 📁 Use Case: Power Automate flow uses unapproved connector to send data externally

### 🎯 Scenario
A user creates a Power Automate flow that collects data from a SharePoint list and sends it to an external service using an unapproved third-party connector. The connector bypasses internal validation, sending sensitive project data outside the organisation. No DLP policies or connector restrictions are in place.

### ⚠️ OWASP Risk
**A08: Software and Data Integrity Failures**  
Use of untrusted or unverified components in workflows may allow data manipulation or leakage without proper validation.

### 🔍 Microsoft 365 Component
- **Platform:** Power Automate
- **Feature at risk:** Connectors / Flow Governance
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/power-automate/)

### 💥 Potential Impact
- Exposure of sensitive business data to untrusted external services
- Breach of data handling policies or contractual obligations
- Loss of control over data flow and auditability

### 🛡️ Mitigation Strategies
- Restrict usage to approved connectors through Data Loss Prevention (DLP) policies (via Purview)
- Regularly review and monitor flow ownership and connector usage (via Power Platform Admin Center)
- Educate users on safe automation practices and connector governance (via Microsoft 365)

🔍 Search: Power Automate connector governance site:learn.microsoft.com

🔍 Search: Purview DLP for Power Platform site:learn.microsoft.com

🔍 Search: Power Platform Admin Center flow monitoring site:learn.microsoft.com

🔍 Search: Microsoft 365 automation security site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A08`  
See also: `OWASP_M365_Mapping.md → A08 / Power Automate`
