/robots.txt
/sitemap.xml
DNS Records -------------->> ip addr
:>SAST ------------------->> Static Analysis
:>Input valid test ------->> XSS
:>Query and Param enum --->> SQLi, XSS
:>Automated Scans:
::::>Well Known Tools:
      Subfinder ------>> Subdomain Enum
      Sublist3r ------>> Subdomain Enum
      httpx ---------->> HTTP Status Client
      Nmap ----------->> Port & Vuln Scan
      dirb ----------->> Directory Discovery
      gobuster ------->> Directory Discovery
      dirsearch ------>> Directory Discovery
      Nessus --------->> Vuln Scan
      Nikto ---------->> Vuln Scan
      nuclei  -------->> Vuln Scan
      OWASP ZAP ------>> Vuln Scan
      BurpSuiteCom --->> Intercept
      SQLMap --------->> SQL Injection <-Exploitation
::::>Other type Tools:
      katana --------->> Web Crawl (Parameter Scanner)
      xss_vibes ------>> XSS Validator <-Exploitation
      wfuzz ---------->> Fuzzing
      RustScan ------->> Port Scanner
::::>Licensed Automated Tools:
      BurpSuite Pro -->> Web Crawl & Audit & Vuln Scanner
      MetaSploit Pro ->> Scan and Weaponization
      Acunetix Pro --->> Web Application and Enterprise Audit
      Invicti Pro ---->> Automated Web Application and Enterprise Audit
