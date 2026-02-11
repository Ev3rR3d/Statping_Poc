# Statping-ng v0.91.0 - Vulnerability Research Case Study

This repository contains technical documentation and Proof of Concept (PoC) materials for multiple security vulnerabilities identified in **Statping-ng v0.91.0**. These findings range from broken access control to local code execution.

## Summary of Findings

| CVE ID | Vulnerability Type | Impact | Technical Detail |
| :--- | :--- | :--- | :--- |
| **[CVE-2024-26477](./CVE-2024-26477/)** | CWE-250: Privilege Escalation | **Critical** | Remote Admin Creation via API |
| **[CVE-2024-26478](./CVE-2024-26478/)** | Account Takeover | **High** | Admin Password Reset via API |
| **[CVE-2024-26479](./CVE-2024-26479/)** | CWE-200: Info Disclosure | **Medium** | Unauthorized API Endpoint Access |
| **[CVE-2024-26480](./CVE-2024-26480/)** | Local Privilege Escalation | **High** | Arbitrary Code Execution |

## Research Overview
The research focused on the API security model and permission validation logic of the Statping-ng framework. The identified flaws allow an attacker to escalate privileges from a low-privileged API token to full system/application administrative control.

### Discovery Credits
* **Bruno Javarez (Ev3rR3d)** - Security Researcher
* **Gustavo Mugnatto (mugnatto)** - Security Researcher

## Disclaimer
These PoCs are provided for educational and authorized research purposes only. The vendor has been informed of these issues to facilitate the development of necessary patches.

---
*Status: CVE IDs Reserved. Documentation submitted for public disclosure.*
