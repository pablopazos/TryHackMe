# Introduction to Cyber Security: Cyber Security 101

### Some important command lines in linux 

**`Usage of dirb`**: this command is used to discover hidden paths that could exist in a website, and we can know if they are protected 
or vulnerable.

**`Usage of ss`**: this command is used to monitor the different ports in our machine. It has several options like -t for TCP or -u for UDP.
Snake oil: This term is used when a business claims to have 'unbreakable' security by using custom or unproven encryption methods instead of industry standards like RSA or AES.

### Quick Summary: Google Advanced Search Operators
Search engines like Google allow the use of specific operators to perform Passive Reconnaissance (gathering information without interacting directly with the target).
"exact phrase": Use double quotes to find pages that contain a specific word or phrase in the exact same order.
site:: Limits the search to a specific domain or website (e.g., site:inditex.com).
-: Used to exclude specific words from the search results.
filetype: : Filters results to find specific file formats, such as PDF, DOC, XLS, or PPT. This is highly effective for finding exposed internal documents.

### Cyber Security important sites: 

- **`Shodan`**: a Google of internet devices. You can find almost everything with an IP and an open port.

- **`Censys`**: A search engine focused on Digital Certificates (SSL/TLS). It helps validate asset ownership and uncovers hidden subdomains or origin IPs.

- **`VirusTotal`**: A global Threat Intelligence aggregator. It checks if an IP or domain has a malicious reputation or is part of a known botnet.

- **`Have I Been Pwned`** (HIBP): The definitive database for Data Breaches. It tracks leaked corporate credentials to assess the risk of "Credential Stuffing" attacks.

- **`CVE`**: Common Vulnerabilities and Exposures= dictionary of vulnerabilities.

### Important vulnerabilies:
- The humans are the easiest way to get into a defensive system by exploiting human psichology
- Defending against threats involves two tasks, mitigation and detection, but one day, the defenses will get passed, so the labor of a SOC is having the skills to solve this.

### System Security & Vulnerabilities

* **The "Castle" Analogy:** Having a well-trained user (gatekeeper) who can spot phishing or deepfakes is not enough if the underlying system infrastructure (the lock) is fragile and weak. 
* **Direct Infrastructure Attacks:** Threat actors can bypass users entirely and attack insecure systems directly without anyone noticing.
* **Definition of System:** Systems include physical servers, lab machines, or cloud platforms (e.g., Microsoft 365). 
* **Impact of a System Breach:** Compromising a single user's mailbox (via phishing) only impacts that individual, but breaching a mail server grants the attacker control over thousands of mailboxes simultaneously.
* **Definition of Supply Chain in Cyber:** It includes any external software, hardware, or service provider your organization relies on, so an attack on the provider will affect you directly.

### Security Misconfigurations

* **Definition:** Human errors made during system setup for convenience (e.g., weak passwords, disabled firewalls), rather than actual software bugs.
* **The Breach Process:** A secure system receives sensitive data, IT introduces flaws (weak credentials/open ports), threat actors easily exploit it and steal data.
* **Proactive Defenses:**
  * **Penetration Testing:** Simulating attacks to find flaws.
  * **Vulnerability Scans:** Automated tools checking for default settings.
  * **Configuration Audits:** Reviewing settings against standards (like CIS benchmarks).
