---

# Mitigation Strategies for OWASP Top 10 in Microsoft 365

This document provides practical mitigation strategies for each [OWASP Top 10](https://owasp.org/www-project-top-ten/) risk, adapted to Microsoft 365 use cases. Each section includes recommended actions and search keywords to find official Microsoft documentation.

---
## A01: Broken Access Control

- OneDrive: Restrict sharing to specific individuals 

  🔍 Search: OneDrive shareable links site:learn.microsoft.com
  
- OneDrive: Disable "Anyone with the link" sharing  

  🔍 Search: OneDrive anonymous sharing site:learn.microsoft.com

- OneDrive\SharePoint: Enable external sharing alerts
  
  🔍 Search: OneDrive\SharePoint sharing alerts site:learn.microsoft.com

- Azure AD: Use Role-Based Access Control (RBAC) to enforce the Principle of Least Privilege (PoLP)
  
  🔍 Search: Azure AD RBAC config site:learn.microsoft.com

---

## A02: Cryptographic Failures

- Purview: Use Sensitivity Labels to encrypt emails and documents

  🔍 Search: Purview sensitivity labels site:learn.microsoft.com
  
- Outlook: Ensure TLS is enabled for email transport

  🔍 Search: Outlook enabling TLS site:learn.microsoft.com

- Microsoft 365: Implement Customer Key for customer-managed encryption keys

  🔍 Search: Microsoft 365 customer key site:learn.microsoft.com

---

## A03: Injection (includes LLM01:2025 Prompt Injection)

- Copilot: Sanitise user prompts before submission to input boxes

  🔍 Search: Copilot security site:learn.microsoft.com

- Copilot: Educate users on secure prompt design

  🔍 Search: Secure prompting site:learn.microsoft.com

---

## A04: Insecure Design

- Teams: Apply guest access policies and conduct regular review

  🔍 Search: Teams guest access site:learn.microsoft.com

- Teams: Use dedicated Teams for external collaboration

  🔍 Search: Teams collaboration teams site:learn.microsoft.com

- Teams: Disable private channel creation for guests

  🔍 Search: Teams private channels settings site:learn.microsoft.com

- Purview: Use Sensitivity Labels for Teams

  🔍 Search: Sensitivity Labels for Teams site:learn.microsoft.com

---

## A05: Security Misconfiguration

- Defender for Office 365: Disable external email forwarding and use outbound spam policies to restrict risky behaviour
  
  🔍 Search: Defender 365 external mail forwarding site:learn.microsoft.com
  
- Purview: Audit mailbox rules regularly

  🔍 Search: Purview mailbox auditing site:learn.microsoft.com

- Exchange Online: Use Microsoft 365 mail flow rules to block, warn, or moderate messages containing sensitive data - Data loss prevention (DLP)

  🔍 Search: Exchange Online managing mail flow rules site:learn.microsoft.com

---

## A06: Vulnerable and Outdated Components

- Intune: Enforce automatic updates for all applications
  
  🔍 Search: Intune automatic updates site:learn.microsoft.com
  
- Intune: Set minimum version requirements

  🔍 Search: Intune setting minimum version site:learn.microsoft.com
  
- Intune/Endpoint Manager: Monitor update compliance across all devices

  🔍 Search: Intune/Endpoint Manager monitoring devices site:learn.microsoft.com

---

## A07: Identification and Authentication Failures

- Entra ID: Enforce multi-factor authentication (MFA)

  🔍 Search: Entra ID MFA configuration site:learn.microsoft.com
    
- Microsoft 365: Apply robust password policies

  🔍 Search: Microsoft 365 passwords policies site:learn.microsoft.com
  
- Entra ID: Use conditional access rules as part of a Zero-Trust policy

  🔍 Search: Entra ID conditional access rules site:learn.microsoft.com

---

## A08: Software and Data Integrity Failures

- Power Automate: Use only approved connectors

  🔍 Search: Power Automate certified connectors and data policies site:learn.microsoft.com
  
- Power Automate: Review flow permissions and ownership

  🔍 Search: Power Automate flow permissions and ownership site:learn.microsoft.com

- Purview: Apply Data Loss Prevention (DLP) policies

  🔍 Search: Purview DLP policies site:learn.microsoft.com

---

## A09: Security Logging and Monitoring Failures

- Purview: Enable audit logging in Microsoft 365

  🔍 Search: Purview audit solutions site:learn.microsoft.com
  
- Defender XDR: Configure alerts for suspicious activity

  🔍 Search: Defender XDR alerts settings site:learn.microsoft.com

- Defender XDR: Use Microsoft Secure Score to identify and remediate gaps

  🔍 Search: Defender XDR secure score recommendations site:learn.microsoft.com

---

## A10: Server-Side Request Forgery (SSRF)

- Microsoft Forms: Validate user input to prevent injection of malicious URLs

  🔍 Search: Microsoft Forms input validation site:learn.microsoft.com

- Power Automate: Sanitise and validate dynamic inputs before using them in HTTP actions

  🔍 Search: Power Automate HTTP action input validation site:learn.microsoft.com
  
- Power Automate: Restrict use of HTTP actions and custom connectors to trusted domains

  🔍 Search: Power Automate HTTP connector domain restrictions site:learn.microsoft.com
