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

