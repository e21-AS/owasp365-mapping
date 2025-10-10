# 🧠 A03: Injection ([LLM01:2025 Prompt Injection](https://genai.owasp.org/llmrisk/llm01-prompt-injection/))  
## 📁 Use Case: Copilot receives a manipulated prompt from Teams message

### 🎯 Scenario  
A user sends a Teams message containing a crafted instruction designed to manipulate Copilot's behaviour. When another user invokes Copilot in the same context, the injected prompt may cause Copilot to reveal internal instructions or perform unintended actions, such as summarising confidential content or suggesting inappropriate responses.

### ⚠️ OWASP Risk  
**A03: Injection**  
Untrusted input is interpreted as part of a command or instruction, leading to unintended behaviour. In this case, prompt injection targets the logic of a large language model (LLM).

### 🔍 Microsoft 365 Component  
- **Platform:** Copilot (via Teams)  
- **Feature at risk:** Prompt Context Injection  
- **Documentation:** [Microsoft](https://learn.microsoft.com/en-us/copilot/)

### 💥 Potential Impact  
- Disclosure of internal Copilot instructions or system behaviour  
- Exposure of sensitive data through manipulated summarisation  
- Reputational damage or regulatory non-compliance

### 🛡️ Mitigation Strategies  
- Sanitise and delimit user-generated prompts before passing to Copilot (via Teams / Copilot API)  
- Restrict Copilot's access to sensitive content by applying Purview DLP policies  
- Monitor Copilot interactions for anomalous behaviour (via Defender XDR or audit logs)

🔍 Search: Copilot prompt injection site:learn.microsoft.com

🔍 Search: Purview DLP for Copilot site:learn.microsoft.com

🔍 Search: Teams message sanitization site:learn.microsoft.com

🔍 Search: Defender XDR Copilot monitoring site:learn.microsoft.com

### 📌 Related  
See also: `Mitigation_Strategies.md → A03`  
See also: `OWASP_M365_Mapping.md → A03 / Copilot`
