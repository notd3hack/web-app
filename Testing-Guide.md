# Web Application Penetration Testing Checklist

## PRE-ENGAGEMENT
- [ ] **Define Scope & Rules of Engagement**
- [ ] Obtain written authorization
- [ ] Set testing windows
- [ ] Establish communication channels
- [ ] Define sensitive data handling procedures

## RECONNAISSANCE & INFORMATION GATHERING
- [ ] **Passive Reconnaissance**
  - [ ] WHOIS lookup
  - [ ] DNS enumeration (subdomains, records)
  - [ ] Search engine dorking
  - [ ] Archive.org historical data
  - [ ] Social media/OSINT gathering

- [ ] **Active Reconnaissance**
  - [ ] Port scanning (Nmap)
  - [ ] Service fingerprinting
  - [ ] Web server/technology identification
  - [ ] Directory/file brute forcing
  - [ ] Virtual host enumeration

## AUTHENTICATION & AUTHORIZATION
- [ ] **Authentication Testing**
  - [ ] Default/weak credentials
  - [ ] Credential brute forcing (with lockout testing)
  - [ ] Password policy bypass
  - [ ] Password reset flaws
  - [ ] Remember me functionality
  - [ ] Session fixation
  - [ ] Logout functionality effectiveness

- [ ] **Authorization Testing**
  - [ ] Horizontal privilege escalation
  - [ ] Vertical privilege escalation
  - [ ] Insecure direct object references (IDOR)
  - [ ] Missing function level access control
  - [ ] Parameter tampering for privilege changes

## SESSION MANAGEMENT
- [ ] **Session Handling**
  - [ ] Session token analysis (predictability, entropy)
  - [ ] Cookie attributes (Secure, HttpOnly, SameSite)
  - [ ] Session expiration testing
  - [ ] Concurrent session handling
  - [ ] Session hijacking vulnerabilities

## INPUT VALIDATION & OUTPUT ENCODING
- [ ] **Cross-Site Scripting (XSS)**
  - [ ] Reflected XSS
  - [ ] Stored XSS
  - [ ] DOM-based XSS
  - [ ] Blind XSS

- [ ] **SQL Injection**
  - [ ] Error-based SQLi
  - [ ] Union-based SQLi
  - [ ] Boolean-based blind SQLi
  - [ ] Time-based blind SQLi
  - [ ] Out-of-band SQLi

- [ ] **Other Injections**
  - [ ] Command injection
  - [ ] LDAP injection
  - [ ] XML injection (XXE)
  - [ ] HTML injection
  - [ ] Template injection (SSTI)
  - [ ] CSV injection

## SECURITY MISCONFIGURATIONS
- [ ] **Server/Application Config**
  - [ ] Default files/pages
  - [ ] Directory listing enabled
  - [ ] Verbose error messages
  - [ ] Unnecessary HTTP methods
  - [ ] CORS misconfigurations
  - [ ] Clickjacking/X-Frame-Options
  - [ ] Security headers missing (CSP, HSTS, etc.)
  - [ ] Backup files exposed

## BUSINESS LOGIC VULNERABILITIES
- [ ] **Logic Flaws**
  - [ ] Price manipulation
  - [ ] Negative quantities/values
  - [ ] Workflow bypass
  - [ ] Time-of-check vs time-of-use (TOCTOU)
  - [ ] Repudiation issues

## CLIENT-SIDE TESTING
- [ ] **Client-Side Security**
  - [ ] JavaScript source code review
  - [ ] Sensitive data in client-side storage
  - [ ] Client-side validation bypass
  - [ ] WebSocket security
  - [ ] PostMessage security
  - [ ] CORS implementation review

## FILE & RESOURCE HANDLING
- [ ] **File Upload Vulnerabilities**
  - [ ] File type restriction bypass
  - [ ] Malicious file upload
  - [ ] Path traversal in file names
  - [ ] Overwriting existing files

- [ ] **Path Traversal**
  - [ ] Directory traversal
  - [ ] Local file inclusion (LFI)
  - [ ] Remote file inclusion (RFI)

## API TESTING (REST/SOAP/GraphQL)
- [ ] **API Security**
  - [ ] Authentication/authorization bypass
  - [ ] Excessive data exposure
  - [ ] Missing rate limiting
  - [ ] Mass assignment
  - [ ] Broken object level authorization
  - [ ] Improper assets management

## THIRD-PARTY COMPONENTS
- [ ] **Dependency Analysis**
  - [ ] Known vulnerabilities in frameworks/libraries
  - [ ] Outdated components
  - [ ] Unsupported software versions

## CRYPTOGRAPHY
- [ ] **Cryptographic Issues**
  - [ ] Weak encryption algorithms
  - [ ] Insufficient entropy
  - [ ] Improper certificate validation
  - [ ] Sensitive data in transit (TLS testing)
  - [ ] Sensitive data at rest

## MISCELLANEOUS
- [ ] **Other Tests**
  - [ ] Denial of Service (DoS) vulnerabilities
  - [ ] Race conditions
  - [ ] Server-Side Request Forgery (SSRF)
  - [ ] Host header injection
  - [ ] Open redirects
  - [ ] Content spoofing

## POST-TESTING
- [ ] **Cleanup & Reporting**
  - [ ] Remove test accounts/files
  - [ ] Clear test data
  - [ ] Document all findings with:
    - [ ] Clear vulnerability descriptions
    - [ ] Proof of concept
    - [ ] Risk assessment (CVSS scoring)
    - [ ] Remediation recommendations
  - [ ] Executive summary for management
  - [ ] Technical details for developers
  - [ ] Retest critical findings after fixes

## TOOLS TO CONSIDER
- **Proxy/Intercept:** Burp Suite, OWASP ZAP, Fiddler
- **Scanners:** Nuclei, Nikto, Nessus, OpenVAS
- **Fuzzers:** ffuf, wfuzz, Burp Intruder
- **Specialized:** sqlmap, NoSQLMap, XSStrike, SSRFmap
- **Manual Testing:** Browser DevTools, curl, custom scripts

## IMPORTANT NOTES:
1. **Manual testing > Automated scanning** - Tools miss business logic flaws
2. **Get proper authorization** - Always have written permission
3. **Document everything** - Screenshots, requests/responses, timestamps
4. **Don't assume** - Test everything, even "secure" configurations
5. **Consider impact** - Don't cause production issues during testing
6. **Retest fixes** - Verify remediation actually works