# FIRST SMALL LAB 1 FROM CYBER SECURITY 1

In first place, I get my public IP using the command line: **`curl ipconfig.me`**. 
After getting my IP, I'm using **`Shodan`** to know if I'm exposed through my router and document the results.
The result was: 
Note: No results found
<img width="1920" height="382" alt="Screenshot From 2026-03-30 16-38-32" src="https://github.com/user-attachments/assets/f0171581-7a12-4f33-8184-11e609e570c8" />

In conclusion, there is no visible information leaked from my ISP or indexed data for my regarding my public IP.

In second place, I tried some filters, like city: "A Coruña" country: "ES" and I find a lot to see:
-I identified specific software versions, such as PowerDNS 4.9.5. Knowing the exact version is the first step for a **`Vulnerability Assessment`**.
-IoT Exposure: Found RTSP banners, which likely belong to IP cameras or surveillance systems.
-Infrastructure Management: Detected SNMP protocols active on corporate networks (Business A), providing hardware details like Engine Boots and Up-time, **the last with like 1000 days without a reboot,
what could be a danger**.

To finalize, I saw an IP camera, from Business B, exposing its web management interface on port 81 and its real-time streaming protocol on port 554, so the risk was that
we could **direct access** to the management login portal.
