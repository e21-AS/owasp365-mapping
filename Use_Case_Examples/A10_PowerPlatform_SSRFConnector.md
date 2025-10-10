# 🌐 A10: Server-Side Request Forgery (SSRF)
## 📁 Use Case: Power Platform custom connector sends unvalidated request to internal API

### 🎯 Scenario
A developer creates a custom connector in Power Platform that integrates with an internal HR API. The connector accepts user-supplied URLs without proper validation. An attacker crafts a flow that sends requests to internal endpoints (e.g. metadata services or Azure instance metadata), potentially exposing sensitive configuration or tokens.

### ⚠️ OWASP Risk  
**A10: Server-Side Request Forgery (SSRF)**  
The server-side component makes requests to internal or external resources based on untrusted input, potentially exposing sensitive data or internal service endpoints.

### 🔍 Microsoft 365 Component
- **Platform:** Power Platform (Custom Connectors)
- **Feature at risk:** Connector Input Validation / API Gateway
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/connectors/custom-connectors/)

### 💥 Potential Impact
- Exposure of internal metadata or configuration endpoints
- Leakage of access tokens or service identities
- Lateral movement within internal infrastructure via trusted connectors

### 🛡️ Mitigation Strategies  
- Validate and sanitise connector inputs, especially URLs and endpoint parameters
- Restrict connector access to trusted domains using network rules or API Management
- Monitor connector usage and outbound requests through Defender for Cloud Apps or Azure Monitor
- Educate developers on SSRF risks in low-code integrations

🔍 Search: Power Platform custom connector SSRF site:learn.microsoft.com

🔍 Search: API management input validation site:learn.microsoft.com

🔍 Search: Defender for Cloud Apps connector monitoring site:learn.microsoft.com

🔍 Search: Azure instance metadata SSRF site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A10`  
See also: `OWASP_M365_Mapping.md → A10 / Power Platform`
