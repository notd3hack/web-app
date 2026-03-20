Foundations & Red Teaming Core

Information Security Block (Theory)
•	CIA Triad (Confidentiality, Integrity, Availability)
•	Encryption / Decryption & Hashing
•	Zero Trust Model (MFA, Least Privilege, Segmentation, Automation)
•	Cybersecurity Frameworks (NIST, ISO, CIS, GDPR, MITRE ATT&CK, Cyber Kill Chain)
•	Authentication methods, 2FA, MFA, Honeypods
•	Red, Blue, Purple Teams, Threat Intelligence & OSINT
•	Flags & Ticketing (TN, FN, TP, FP)
•	AI in Cybersecurity (Defensive & Offensive: ChatGPT, EvilGPT, WormGPT, PentestGPT)
•	VMware / VirtualBox Setup & VM Deployment

Networking Block
•	TCP/IP & OSI Models, protocols (HTTP, HTTPS, FTP, DNS, DHCP)
•	Common Network Attacks (Spoofing, MITM, DoS, Hijacking, Injection)
•	Securing Networks (ACLs, encryption, monitoring, Wireshark basics)
•	Firewalls (NGFW, host-based firewalls like Portmaster, Comodo)
•	IDS/IPS & segmentation
•	Secure Communications (VPNs, TLS/SSL, SSH)
•	Logging & Incident Response basics (network logging, IR workflow)

GNU/Linux Fundamentals
•	Linux distros overview (Ubuntu, Kali)
•	Basic commands (ls, cd, pwd, cp, mv, rm) & filesystem structure (/etc, /var, /usr)
•	User & permission management (chmod, chown, groups, SUID)
•	Firewall setup (iptables, gufw)
•	Logs & monitoring (journalctl, dmesg, /var/log)
•	Security auditing tools (linPEAS, unix-privesc-check)
•	Systemctl, SSH hardening, patching, app management
•	Local Privilege Escalation theory

Windows OS & Endpoint Security
•	Networking Fundamentals (IP, MAC, subnetting, LAN/WAN, devices)
•	Windows OS Basics (architecture, programs, services, antivirus, AMSI, UAC, Windows Defender)
•	Windows Permissions (accounts, permission levels, practical labs)
•	PowerShell vs CMD (cmdlets, scripts, automation, pentesting playbook, file types)
•	Windows Power User Tools (Sysinternals, gpedit, secpol, automation with Task Scheduler)

Windows Targeting & Initial Exploitation
•	Reconnaissance & Resource Development (Meterpreter, reverse shell, payload delivery)
•	Anti-malware evasion basics
•	Exploit delivery via MS Office payloads
•	Local Privilege Escalation introduction (winPEAS)

Web Application Security (Intro)
•	Web architecture (client-server, URL, parameters, authentication/session)
•	OWASP Top 10 overview
•	BurpSuite CE basics
•	Manual detection: XSS, SQLi, file uploads, LFI/RFI, path traversal, OS command injection
•	Web Application Firewalls basics
 
Advanced Red Teaming & Infrastructure Attacks (Stage 2)

Windows Exploit Development & Advanced Persistence
•	Staged vs Stageless & Fileless Malware
•	Kernel Exploitation (intro level)
•	AlwaysInstallElevated abuse
•	DLL Hijacking
•	Service binPath & Registry Manipulation
•	Unquoted Service Paths
•	Autorun persistence
•	Scheduled Task exploitation
•	Startup application hijacking
•	Command & Control (C2) basics
•	Shellter.py & EvilSetup.exe

Advanced Linux Pentesting
•	Practical exploitation with linPEAS & Linux Exploit Suggester
•	GTFOBins abuse, Sudo escalation
•	Kernel exploits (DirtyCow, DirtyPipe, etc.)
•	Cron job exploitation
•	Capabilities exploitation
•	Container breakout & Docker escapes

Web Application Exploitation (Advanced)
•	SSRF, IDOR, JWT attacks, Race conditions, Deserialization
•	File Upload Bypass & Advanced RCE
•	Path Traversal chaining
•	Automation with tools: Subfinder, Sublist3r, httpx, nmap, dirb, gobuster, dirsearch, nikto, nuclei, ZAP, BurpSuite Pro
•	Extra tools: Katana, xss_vibes, wfuzz
•	Bug bounty style labs

Infrastructure & Active Directory Attacks
•	What is AD & why it matters (roles, FSMO, benefits, setup)
•	NTLM, Kerberos, OAuth theory
•	Attacks: NTLM Relay, Pass-the-Hash, LLMNR Poisoning
•	Kerberoasting & AS-REP Roasting
•	Password Spraying & Default Credentials
•	Hard-coded credential hunting
•	LDAP Recon & Enumeration
•	BloodHound/Sharphound for AD mapping
•	NTDS.dit Extraction
•	Mimikatz for credential dumping
•	Lateral movement (WinRM, evil-winRM)
•	Advanced AD Attacks: Shadow Credentials, RBCD, PrintNightmare, PetitPotam
•	Defender for Identity bypass techniques