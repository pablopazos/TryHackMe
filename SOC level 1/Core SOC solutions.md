### SIEM (Security Information and Event Management)

A **SIEM** is a central tool used by security analysts (SOC) to collect, organize, and compare log data created by all devices on a network.

#### Key Points
* **Centralization & Ingestion:** Gathers logs from many sources (servers, firewalls, EDRs, applications) into one single place.
* **Overcoming Isolated Logs:** Solves the problem of checking logs on individual computers one by one, providing a full view of the whole network.
* **Event Correlation:** Connects the dots between different log sources to spot attack patterns or suspicious behavior.
* **Alerts & Analysis:** Automatically generates alerts to help analysts investigate security incidents much faster.

---

### Host-Centric vs. Network-Centric (Summary)

These are two complementary ways to monitor and protect a system:

* **Host-Centric:** Focuses on what happens **inside a single computer or server** (e.g., process execution, file changes, registry updates). Measured using tools like EDRs and OS logs.
* **Network-Centric:** Focuses on the **traffic moving between devices and the internet** (e.g., IP addresses, ports, protocols, domain requests). Measured using tools like Firewalls and Proxies.

### Core Capabilities of a SIEM

A **SIEM** enhances security operations by centralizing, standardizing, and analyzing logs across an entire organization.

---

#### 1. Centralized Log Collection
* **Definition:** Gathers log data from all network devices (endpoints, servers, firewalls, etc.) into a single location using lightweight agents or APIs.
* **Benefit:** Eliminates the need to log in to individual machines manually to analyze events.

---

#### 2. Normalization of Logs
* **Definition:** Converts raw logs from different operating systems and devices (e.g., Windows vs. Linux) into a unified, consistent format through parsing.
* **Benefit:** Makes log data easier to read, compare, and query across different sources.

---

#### 3. Correlation of Logs
* **Definition:** Connects disparate events happening across different systems within a specific timeframe to identify complex attack patterns.
* **Example:** Linking a suspicious VPN login from a new IP, access to shared drive files, execution of a PowerShell script, and an outbound network connection to reveal a single compromised account incident.

---

#### 4. Real-time Alerting
* **Definition:** Automatically triggers notifications for security analysts when ingested logs match predefined or custom detection rules.
* **Benefit:** Enables rapid response to ongoing security threats.

---

#### 5. Dashboards and Reporting
* **Definition:** Provides visual summaries and actionable insights from ingested and normalized log data.
* **Key Components:**
  * Alert Highlights
  * System Notifications & Health Alerts
  * Failed Login Attempts
  * Ingested Event Counts

