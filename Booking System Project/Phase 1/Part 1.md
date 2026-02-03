# 1️⃣ Introduction

**Tester(s):**  
- Name:  Jimi Ikola

**Purpose:**  
- Describe the purpose of this test (e.g., identify vulnerabilities in registration and authentication flows).

**Scope:**  
- Tested components:  
- Exclusions:  
- Test approach: Gray-box / Black-box / White-box

**Test environment & dates:**  
- Start:  
- End:  
- Test environment details (OS, runtime, DB, browsers):

**Assumptions & constraints:**  
- e.g., credentials provided, limited time, etc.

---

# 2️⃣ Executive Summary

**Short summary (1-2 sentences):**  

**Overall risk level:** (Low / Medium / High / Critical)

**Top 5 immediate actions:**  
1.  Absence of Anti-CSRF Tokens
2.  Content Security Policy (CSP) Header Not Set (3)
3.  Cross-Domain Misconfiguration
4.  Format String Error
5.  Missing Anti-clickjacking Header(3)

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
| F-01 | 🟠 Medium | Absence of Anti-CSRF Tokens | No Anti-CSRF tokens were found in a HTML submission form | Screenshot or sqlmap result * |
| F-02 | 🟠 Medium | Content Security Policy (CSP) Header Not Set (3) | CSP is an added layer of security that helps to detect and mitigate certain types of attacks | Burp log or response headers * |
| F-03 | 🟠 Medium | Cross-Domain Misconfiguration | Web browser data loading may be possible, due to a Cross Origin Resource Sharing (CORS) misconfiguration on the web server | Screenshot of registration success * |
|||Format String Error...|||

---

> [!NOTE]
> Include up to 5 findings total.   
> Keep each description short and clear.

---

# 5️⃣ OWASP ZAP Test Report (Attachment)

**Purpose:**  
- Attach or link your OWASP ZAP scan results (Markdown format preferred).

---

**Instructions:**
1. Check lecture recordings
2. Save the report as `zap_report_round1.md` and link it below.

---
> [!NOTE]
> 📁 **Attach full report:** → `check itslearning` → **Add a link here**

---
