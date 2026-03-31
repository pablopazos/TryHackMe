# SOC L1 ANALYST
### Important topics:
**` SIEM (Security Information and Event Management)`**: Acts as the central nervous system of a SOC. It collects and aggregates log data from multiple sources (firewalls, servers, endpoints) into a single platform. This centralization allows analysts to perform correlation analysis to identify complex attack patterns that would be invisible in isolation.

**` EDR (Endpoint Detection and Response)`**: An advanced security solution that monitors end-user devices (endpoints) like laptops, workstations, and servers in real-time. Unlike traditional Antivirus (AV), which looks for known file signatures, EDR focuses on behavioral analysis.

**`SOAR (Security Orchestration, Automation, and Response)`**: It is a solution that orchestrates different security tools and automates incident response. Instead of a human doing everything manually, the SOAR uses Playbooks (pre-defined rules) to detect a threat (from the SIEM), enrich the data by checking if an IP is malicious, contain the danger by automatically blocking a malicious IP in the Firewall, and finally inform the analyst by creating a detailed report or ticket.

### DIfference between internal SOC and an MSSP:
<img width="1289" height="550" alt="image" src="https://github.com/user-attachments/assets/30af286f-f12f-4d92-9fc6-609a5fdbc71a" />

### Key Learnings: Incident Response & Alert Prioritization 

In this section, I learned that a SOC analyst must handle threats using a structured methodology rather than a random approach. This process is essential for efficient "Triage":

* **Order of Severity:** This is the most critical factor. Alerts are categorized by severity levels (**Critical, High, Medium, Low**). Critical and High-priority alerts must be addressed first because they represent a higher probability of being a **True Positive** (a real attack) and pose a greater risk of data exposure or system compromise.
* **Timeline (FIFO):** While severity is the priority, analysts also consider the age of the alert. Generally, older threats should be addressed before newer ones within the same severity level to ensure no window of opportunity is left open for the attacker.
* **Goal:** By prioritizing based on severity, we minimize the impact of a potential hack and ensure that the most dangerous threats are contained as quickly as possible.
