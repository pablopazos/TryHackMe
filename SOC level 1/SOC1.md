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

  ### Incident Response Lifecycle: SIEM Triage Process

The triage process is divided into three critical phases to ensure a professional and accurate investigation (from THM screen):

1. **Initial Actions (Ownership):** Assign the alert to yourself and move it to "In Progress". Familiarize yourself with the alert name, description, and key indicators to avoid interfering with other analysts.
2. **Investigation (Analysis):** The core step. Identify the "Who" (user/host) and the "What" (action/threat). Review surrounding events for context and use Threat Intelligence to verify if the activity is malicious. Use Playbooks/Workbooks if available.
3. **Final Actions (Verdict):** Decide if the alert is a **True Positive** (malicious) or **False Positive** (benign). Add a detailed comment explaining your reasoning and move the alert to "Closed" status.

###  Alert Management & Escalation

Once the investigation is complete, a SOC Analyst must follow a structured reporting and communication process:

* **Alert Reporting:** For every **True Positive**, a detailed report is required. Unlike a simple comment, this documentation must include all relevant evidence (logs, timestamps, IOCs). This ensures that the context is preserved for further action.
* **Alert Escalation:** If a threat is confirmed (True Positive) and requires deeper investigation or advanced response, it is escalated to **L2 Analysts**. A high-quality L1 report is critical here to minimize analysis time and allow L2 to act quickly.
* **Cross-Departmental Communication:** Analysis often requires external context.
    * **IT Team:** To verify if specific technical actions (like granting admin privileges) were authorized.
    * **HR Department:** To confirm employee status or background information (e.g., verifying a new hire's activity).
 

###  Criteria for Alert Escalation (L1 to L2)

Deciding when to escalate an alert is a key responsibility of the L1 Analyst. While procedures vary by team, these are the four standard scenarios for escalation:

1. **High-Impact Indicators:** When the alert suggests a major cyberattack or a sophisticated threat that requires a deeper, specialized investigation.
2. **Remediation Requirements:** If the incident requires active response actions that exceed L1 permissions, such as:
    * Malware removal.
    * Host isolation (quarantine).
    * Mandatory password resets across the domain.
3. **External Communication:** When the situation requires coordination with:
    * Customers or business partners.
    * Upper management or legal teams.
    * Law enforcement agencies.
4. **Technical Complexity:** If the alert is not fully understood or the analysis reaches a dead end, seeking guidance from senior (L2/L3) analysts is necessary to ensure no threat is overlooked.

