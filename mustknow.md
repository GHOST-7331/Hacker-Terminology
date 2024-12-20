# Must-Know Hacker Terminology for Advanced Penetration Testers

- **Privilege Escalation**: The process of gaining higher-level access or permissions on a system, often through exploiting vulnerabilities or misconfigurations.
- **Command Injection**: A vulnerability that allows an attacker to execute arbitrary commands on a system or network, often through user input fields.
- **SQL Injection**: A vulnerability in web applications where malicious SQL code is inserted into an input field, allowing an attacker to manipulate the database.
- **Cross-Site Scripting (XSS)**: A vulnerability where attackers inject malicious scripts into web pages viewed by other users, enabling data theft or session hijacking.
- **Buffer Overflow**: A condition where a program writes more data to a buffer than it can hold, potentially allowing attackers to execute arbitrary code or crash the program.
- **Reverse Shell**: A shell session initiated by a compromised machine back to an attacker’s system, allowing remote control over the victim machine.
- **Post-Exploitation**: The phase of penetration testing where the attacker maintains access, escalates privileges, and gathers further intelligence after initial compromise.
- **Man-in-the-Middle (MITM)**: An attack where an attacker intercepts and potentially alters communication between two parties without their knowledge.
- **Reconnaissance (Recon)**: The process of gathering information about a target system or network, often using OSINT tools and techniques.
- **Phishing**: A form of social engineering that involves tricking users into providing sensitive information, such as login credentials or personal data.
- **Zero-Day Vulnerability**: A previously unknown vulnerability that is exploited by attackers before the vendor has issued a patch or fix.
- **Privilege Escalation**: Gaining higher system privileges (e.g., root or admin access) through exploiting bugs, configuration errors, or other weaknesses.
- **CVE (Common Vulnerabilities and Exposures)**: A public database of known cybersecurity vulnerabilities and exposures.
- **Keylogging**: The act of recording keystrokes on a device to capture sensitive information like passwords or credit card numbers.
- **Social Engineering**: Manipulating people into divulging confidential information or performing actions that undermine security, often involving psychological manipulation.
- **DNS Spoofing**: A technique where an attacker corrupts DNS records to redirect traffic to malicious websites.
- **DDoS (Distributed Denial of Service)**: A large-scale attack that involves flooding a target server or network with traffic from multiple sources to make it unavailable to users.
- **RAT (Remote Access Trojan)**: A type of malware that gives an attacker remote control over an infected system, often used in post-exploitation phases.
- **Exploit**: A piece of code or a technique used to take advantage of a vulnerability to compromise a system or application.
- **Lateral Movement**: Moving within a network from one compromised system to others to gain more control or escalate privileges.
- **Tactics, Techniques, and Procedures (TTPs)**: The methods and behaviors used by attackers during an attack, often analyzed to understand their approach and predict future actions.
- **Asymmetric Encryption**: A form of encryption using a pair of public and private keys to encrypt and decrypt data, typically used in secure communications.
- **Command and Control (C2)**: The infrastructure used by attackers to maintain communication with compromised systems during an attack.
- **Rootkit**: A type of malware designed to hide its presence by subverting the operating system’s normal operations.
- **Exploit Kit**: A collection of software designed to exploit known vulnerabilities in systems and applications, often used in automated attacks.
- **Denial of Service (DoS)**: An attack that aims to make a system or service unavailable by overwhelming it with excessive requests or traffic.
- **Session Hijacking**: The act of stealing a user’s session token to impersonate them and gain unauthorized access to a web application.
- **Cryptojacking**: A type of attack where an attacker secretly uses a victim’s system to mine cryptocurrency without their consent.
- **Web Shell**: A script placed on a web server that gives attackers remote control over the server, often used in post-exploitation.
- **OSINT (Open Source Intelligence)**: The process of gathering publicly available information from the internet and other open sources for intelligence purposes.
- **Red Team**: A group of ethical hackers who simulate adversary attacks to test an organization’s security posture.
- **Blue Team**: A group responsible for defending an organization’s systems and networks from attacks, often performing defensive penetration testing.
- **Pharming**: A form of attack that redirects legitimate website traffic to fraudulent sites by altering DNS settings or other network configurations.
- **Path Traversal**: A vulnerability that allows attackers to access files and directories stored outside the web server’s root directory, often through URL manipulation.
- **Privilege Abuse**: The improper or excessive use of elevated privileges, often for malicious purposes, to gain unauthorized access or control over systems.
- **Exfiltration**: The act of transferring data from a compromised system to a location controlled by an attacker, often to steal sensitive information.
- **Injection Attacks**: A class of attacks that involve injecting malicious code into a program, such as SQL injection, command injection, and LDAP injection.
- **Sandboxing**: A technique used to isolate and test untrusted code in a controlled environment to prevent it from affecting the broader system.
- **Data Breach**: The unauthorized access or acquisition of sensitive data, often resulting in its theft, exposure, or compromise.
- **Cross-Site Request Forgery (CSRF)**: An attack that tricks a user into performing unintended actions on a website where they are authenticated, potentially leading to unauthorized actions.
- **DNS Tunneling**: A method used by attackers to encode data into DNS queries and responses to bypass firewalls or other security measures.
- **Firewall Evasion**: The process of bypassing or disabling security controls like firewalls, IDS/IPS, or VPNs to gain unauthorized access to a system or network.
- **Cyber Kill Chain**: A model developed by Lockheed Martin that breaks down the stages of a cyberattack into seven steps: 
   1. **Reconnaissance**: Information gathering about the target.
   2. **Weaponization**: Creating malicious payloads (e.g., malware) based on the gathered intelligence.
   3. **Delivery**: Transmitting the weaponized payload to the target.
   4. **Exploitation**: Exploiting vulnerabilities to execute the payload.
   5. **Installation**: Installing the malware on the target system.
   6. **Command and Control (C2)**: Establishing communication with the compromised system.
   7. **Actions on Objectives**: Executing the attacker's ultimate goals (e.g., exfiltrating data, damaging the system, etc.).
