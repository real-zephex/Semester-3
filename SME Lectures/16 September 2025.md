## OSI Layer
- stands for `Open Systems Interconnection`
- It is a conceptual framework used to understand and standardize how different networking technologies and protocols communicate. 
- It breaks the down the complex process of network communication into seven distinct layers:

| Layer | Layer Name   | Function                                                                                                                                |
| ----- | ------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| 7     | Application  | **The User Interface**<br>Provides services directly to the user's software. This is what the user sees and interacts with.             |
| 6     | Presentation | **Translation and Security**<br>Translates data into a common format. It's the translator of the model.                                 |
| 5     | Session      | **Connection Control**<br>Manages the establishment, maintenance, and termination of sessions between applications.                     |
| 4     | Transport    | **End to End Connections and Reliability**<br>Ensures complete data transfer. Manages error correction, flow control, and segmentation. |
| 3     | Network      | **Logical Addressing and Path Determination.**<br>Moves data packets across different networks using logical addresses (IP Addresses)   |
| 2     | Data Link    | **Physical Addressing and Error Detection.**<br>Moves data within the same network (LAN) using physical addresses. (MAC Addresses)      |
| 1     | Physical     | **The Raw Hardware.**<br>Transmits the raw bit stream over the physical medium (cables, radio, waves)                                   |

#### What is the importance of OSI model?

1. **Standardization** - It provides a universal language for engineers and developers to design and discuss networks. A router vendor and a software developer can both refer to "Layer 3" and know exactly what they're talking about.
2. **Troubleshooting** - It allows you to isolate problems. If a website isn't loading, you can methodically check layer: Is the cable plugged in?, Can you ping the server IP?, Is the web service running on the server?
3. **Interoperability** - Because each layer has a defined function, different companies can create hardware and software for specific layers, and they will still work together as long as the adhere to the protocols.

---

## SOC
- stands for Security Operations Center.
- It is a centralized team and facility dedicated to monitoring, detecting, analyzing, and responding to cybersecurity incidents and threats in real time.

#### Functions of a SOC
1. **Continuous Monitoring**: 24/7 surveillance of networks, servers, endpoints, and applications for suspicious activity.
2. **Threat Detection**: Using advanced tools (SIEM, EDR, IDS, IPS) to identify potential threats from logs and network traffic.
3. **Incident Response**: The team springs into action to contain and eradicate a threat once identified. (e.g.: isolating infected machines, blocking malicious IP addresses)
4. **Forensic Analysis**: Investigating incidents after they occur to understand the "how" and "why" and to prevent future occurrences.
5. **Compliance Management**: Ensuring the organization meet regulatory requirements for data security and reporting.
6. **Threat Intelligence**: Staying updated on the latest hacker tactics, techniques, and procedures to anticipate new attacks.

#### What makes up a SOC team?
1. **SOC Manager**: Leads the team and strategy
2. **Security Analysts** (Tiers 1, 2, and 3): Triage alerts, **investigate incidents**, and perform deep-dive analysis.
3. **Incident Responders** - Specialists who lead the charge during a major security breach.
4. **Threat Hunters** - Proactively search for hidden threats that evade automated detection.

#### SIEM (Security Incident and Event Management)
- It is a security technology that collects, monitors, and analyzes log data from an organization's systems, applications, and devices in real time. 
- It acts as a centralized detective for the entire system.


###### Key Functions of SIEM
1. **Data Collection** - Gathers logs from servers, firewalls, antivirus software, and more.
2. **Monitoring** - Watches for unusual patterns, or behaviors that might indicate an attack.
3. **Event correlation** - Connect the dots between different events to spot potential threats.
4. **Alerting** - Sends notifications to security teams when something suspicious is detected.

Some of the popular SIEM tools are:
1. Splunk
2. QRadar (IBM)
3. Arc Sight (Micro Focus)
4. LogRhythm
5. ELK (Elastic Search, Logstash, Kibana)

---

#### CAM
- containable address memory

#### ARP
- address resolution protocol

