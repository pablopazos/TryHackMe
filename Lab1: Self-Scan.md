# FIRST SMALL LAB 1 FROM CYBER SECURITY 1

In first place, I get my public IP using the command line: **`curl ipconfig.me`**. 
After getting my IP, I'm using **`Shodan`** to know if I'm exposed through my router and document the results.
The result was: 
Note: No results found
In conclusion, there is no visible information leaked from my ISP or indexed data for my regarding my public IP.

In second place, I tried some filters, like city: "A Coruña" country: "ES" and I find a lot to see:
-I identified specific software versions, such as PowerDNS 4.9.5. Knowing the exact version is the first step for a **`Vulnerability Assessment`**.
-IoT Exposure: Found RTSP banners, which likely belong to IP cameras or surveillance systems.
-Infrastructure Management: Detected SNMP protocols active on corporate networks (El Corte Inglés), providing hardware details like Engine Boots and Up-time, **the last with like 1000 days without a reboot,
what could be a danger**.

To finalize, I saw a Hikvision IP camera, from Telefonica, exposing its web management interface on port 81 and its real-time streaming protocol on port 554, so the risk was that
we could **direct access** to the management login portal.
