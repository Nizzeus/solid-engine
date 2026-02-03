# 1️⃣ Introduction

**Tester(s):**  
- Name:  Jimi Ikola

**Purpose:**  
- Identify vulnerabilities in user registration and authentication.

**Scope:**  
- Tested components:  
- Exclusions:  
- Test approach: Gray-box

**Test environment & dates:**  
- Start:  1.2.2026
- End:  3.2.2026
- Test environment details (OS, runtime, DB, browsers):

**Assumptions & constraints:**  
- e.g., credentials provided, limited time, etc.

---

# 2️⃣ Executive Summary

**Short summary (1-2 sentences):**  

**Overall risk level:** High

**Top 5 immediate actions:**  
1.  Implement allow list and deny list for input validation in URL and files
2.  Implement Anti-CSRF tokens
3.  Set the Content Security Policy header
4.  Improve error/warning messages
5.  Set the X-Content-Type-Options header to 'nosniff'

---

# 3️⃣ Severity scale & definitions

|  **Severity Level**  | **Description**                                                                                                              | **Recommended Action**           |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
|      🔴 **High**     | A serious vulnerability that can lead to full system compromise or data breach (e.g., SQL Injection, Remote Code Execution). | *Immediate fix required*         |
|     🟠 **Medium**    | A significant issue that may require specific conditions or user interaction (e.g., XSS, CSRF).                              | *Fix ASAP*                       |
|      🟡 **Low**      | A minor issue or configuration weakness (e.g., server version disclosure).                                                   | *Fix soon*                       |
| 🔵 **Info** | No direct risk, but useful for system hardening (e.g., missing security headers).                                            | *Monitor and fix in maintenance* |


---

# 4️⃣ Findings (filled with examples → replace)

> Fill in one row per finding. Focus on clarity and the most important issues.

| ID | Severity | Finding | Description | Evidence / Proof |
|------|-----------|----------|--------------|------------------|
| F-01 | 🔴 High | Path Traversal | Attackers could manipulate the URL to execute or reveal contents of files anywhere on the web server |  |
| F-02 | 🔴 High | SQL Injection | Can input " AND 1=1 --" and " AND 1=2 --" |  |
| F-03 | 🟠 Medium | Absence of Anti-CSRF Tokens | No Anti-CSRF tokens were found in a HTML submission form |  |
| F-04 | 🟠 Medium | Content Security Policy (CSP) header not set (3) | Site is vulnerable to Cross Site Scripting (XSS) and data injection attacks |  |
| F-05 | 🟠 Medium | Missing Anti-clickjacking header (3) | The response does not protect against "ClickJacking" attacks |  |
| F-06 | 🟡 Low | Application Error Disclosure | Error/warning messages disclose sensitive information |  |
| F-07 | 🟡 Low | X-Content Type-Options Header Missing (Systemic) | The Anti-MIME-Sniffing header X-Content-Type-Options was not set to 'nosniff' |  |

---

# 5️⃣ OWASP ZAP Test Report (Attachment)


---
