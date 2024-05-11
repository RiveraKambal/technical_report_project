### **Ethical Hacking Technical Report**  
**Client: Philippine Health Insurance Corporation**  
**Date: May 11, 2024**  
**Prepared by: Marimar H. Rivera**  

  **Executive Summary:** This report presents the technical findings of the ethical hacking assessment conducted for Philippine Health Insurance Corporation website. The assessment aimed to identify vulnerabilities within the organization's network infrastructure, applications, and systems. Through various testing methodologies, including penetration testing and vulnerability scanning, critical and high-risk issues were discovered. This report provides detailed descriptions of these findings, along with actionable recommendations for remediation.

**Vulnerability Summary:**

**1. SQL injection**
-  Critical: Exploiting weaknesses in user input validation to inject malicious SQL code in forms like registration online of PhilHealth.

**2. Cross-Site Scripting (XSS)**
-  Critical: Injecting malicious scripts into web pages, allowing attackers to steal session cookies, log keystrokes, or redirect users to phishing sites like in user login page in PhilHealth.

**3. Server-Side Request Forgery (SSRF)**
-  Critical: Tricking the web server into making unauthorized requests to external servers is found.

**4. Remote Code Execution (RCE):**
-  Critical: Unpatched vulnerabilities allowing attackers to execute arbitrary code on the server, granting complete control for data theft, malware installation, or disrupting operations is found.

**5. Unvalidated Inputs**
- High: Failing to properly validate user input before processing, potentially allowing attackers to inject malicious code or data leading to XSS, SQLi, or other vulnerabilities is found.

**6. Broken Authentication:**
-  High: Weak password policies or lack of multi-factor authentication making it easier for attackers to steal user credentials and access accounts is found.

**7. Security Misconfiguration:**
-  High: Insecure configurations of web servers, databases, or other components leaving the system vulnerable (e.g., weak encryption, unnecessary services, permissive file permissions).

**8. Outdated Components:**
-  High: Using outdated software libraries or frameworks with known vulnerabilities, exposing the system to exploits is found.

**9. Insufficient Logging and Monitoring:**
-  High:  Lack of proper logging and monitoring making it difficult to detect and respond to security incidents is found.

**10: Insecure Direct Object References (IDOR):**
-  High: Unauthorized users potentially accessing other users' data by manipulating URLs or other identifiers is found.

**Recommendation:**

**Critical Vulnerabilities (SQLi, XSS, SSRF, RCE):**
- **Implement robust input validation:** Sanitize and validate all user input before processing it to prevent malicious code injection.
- **Regular security assessments:** Conduct regular penetration testing and vulnerability scans to identify and address security weaknesses.
- **Keep software updated:** Patch vulnerabilities promptly upon discovery in web servers, databases, frameworks, and libraries used on the PhilHealth website.
- **Enforce strong access controls:** Implement least privilege principle and restrict access to sensitive data based on user roles.
- **Utilize secure coding practices:** Developers should follow secure coding guidelines to minimize vulnerabilities during development.

**High Vulnerabilities (Unvalidated Inputs, Broken Authentication, Security Misconfiguration, Outdated Components, Insufficient Logging & Monitoring, IDOR):**
- **Implement input validation:** Sanitize and validate all user input to prevent malicious code injection.
- **Enforce strong password policies:** Require strong passwords with minimum length, complexity requirements, and regular password changes.
- **Enable multi-factor authentication (MFA):** MFA adds an extra layer of security by requiring a second verification factor beyond a password.
- **Review and harden configurations:** Review and adjust web server, database, and other system configurations to meet security best practices.
- **Maintain software updates:** Keep all software components updated with the latest security patches.
- **Implement comprehensive logging and monitoring:** Log user activity, security events, and system changes for better visibility and incident detection.
- **Address IDOR vulnerabilities:** Implement access controls to ensure users can only access their own data.

**Executive Summary:** The findings of the ethical hacking assessment highlight several critical vulnerabilities and  security weaknesses within Philippine Health Insurance Corporation organization's infrastructure and applications. By implementing the recommended remediation measures, Philippine Health Insurance Corporation can significantly enhance its security posture and mitigate the risk of cyber threats and data breaches.

**Signature:**  Marimar H. Rivera