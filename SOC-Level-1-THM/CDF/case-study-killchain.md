# 🔗 Cyber Kill Chain Case Study

## Overview

In this case study, I explored the **Cyber Kill Chain Framework**, developed by **Lockheed Martin** in 2011.  
Originally a **military concept** describing the stages of an attack, the framework was adapted to cybersecurity to help analysts understand and disrupt digital intrusions.

The Cyber Kill Chain outlines the **seven key phases** of a cyberattack:

1. Reconnaissance  
2. Weaponization  
3. Delivery  
4. Exploitation  
5. Installation  
6. Command & Control  
7. Actions on Objectives  

Understanding these stages allows analysts to detect, disrupt, and defend against cyberattacks — especially **ransomware campaigns**, **breaches**, and **Advanced Persistent Threats (APTs)**.

---

## 🧠 What I Did

I started by reviewing how the **Cyber Kill Chain** translates the attacker’s workflow into identifiable stages.  
The goal was to learn how each step leaves behind digital footprints that can be detected and mitigated by defenders.

Throughout this project, I examined each phase through the lens of a fictional attacker named **“Megatron”**, using simulated scenarios to understand how adversaries plan, execute, and maintain cyber operations.

---

## 🕵️‍♂️ Phase 1: Reconnaissance

I began with **reconnaissance**, where attackers gather information about their target using **OSINT (Open Source Intelligence)**.  
This involves studying company infrastructure, identifying employees, and collecting contact data.

I explored tools that attackers commonly use for this phase:
- **theHarvester** – gathers emails, subdomains, and IPs.  
- **Hunter.io** – finds publicly available email addresses.  
- **OSINT Framework** – a web-based interface that organizes reconnaissance tools.  

I learned how attackers perform **email harvesting** — the process of collecting email addresses to prepare for phishing campaigns.  
This stage emphasized the importance of limiting public exposure of sensitive company information and training staff against social engineering.

✅ **Key Takeaways**
- Reconnaissance is about preparation and research.  
- OSINT data is a goldmine for attackers — and a red flag for defenders to monitor exposure.

---

## ⚔️ Phase 2: Weaponization

Once reconnaissance is complete, I studied how attackers **build their weapon** — combining **malware** and **exploits** into a payload.

I analyzed:
- **Malware**: software designed to damage or infiltrate systems.  
- **Exploit**: code that leverages a system vulnerability.  
- **Payload**: the malicious code executed on a system.  

Attackers often embed **macros** inside Office documents, using **VBA scripts** to automate infection upon opening.  
More advanced groups might build custom malware or purchase it on the **Dark Web** to evade detection.

✅ **Key Takeaway:**  
Even something as common as a Word document can be weaponized using malicious macros — a reminder of why email attachments remain a major attack vector.

---

## 📧 Phase 3: Delivery

Next, I learned how attackers deliver their weapon to the victim.  
This is where social engineering meets technical exploitation.

Common delivery methods include:
- **Phishing emails** (including spearphishing for targeted attacks)  
- **Infected USB drives** (e.g., “USB drop” attacks)  
- **Watering hole attacks**, where a trusted website is compromised to serve malware  

I discovered that the **watering hole attack** is particularly dangerous since it targets websites that victims frequently visit, making it a stealthy and effective delivery strategy.

✅ **Key Takeaway:**  
Delivery is where human psychology becomes part of the attack surface — education and awareness are critical defenses.

---

## 💣 Phase 4: Exploitation

In this phase, I analyzed how attackers exploit system vulnerabilities to execute the payload.  
This can happen when victims click malicious links or open infected attachments.

I learned about **zero-day exploits**, which target unknown vulnerabilities — giving defenders no time to prepare or patch.

Attackers might:
- Trigger exploits via malicious attachments or web links.  
- Use server-based vulnerabilities for remote access.  
- Exploit both software and human errors.

✅ **Key Takeaway:**  
Exploitation is where prevention and detection overlap — strong patch management and endpoint protection are vital.

---

## 🧬 Phase 5: Installation

Once access is gained, attackers aim for **persistence** — ensuring they can return even after a reboot or cleanup.

I learned about persistence techniques such as:
- Deploying **web shells** on servers for remote access.  
- Installing **backdoors** using tools like **Meterpreter**.  
- Modifying Windows services or **registry run keys** for automatic execution.  
- Using **Timestomping** to alter file timestamps and avoid forensic detection.

✅ **Key Takeaway:**  
Persistence techniques allow attackers to blend in with legitimate processes. Detecting unusual registry changes or service modifications is essential.

---

## 🌐 Phase 6: Command & Control (C2)

I then explored how attackers establish a **C2 channel** to control infected systems remotely.  
This is where malware begins communicating with the attacker’s infrastructure.

Common methods include:
- **HTTP/HTTPS beaconing** on ports 80 or 443 (to blend with normal web traffic).  
- **DNS Tunneling**, where DNS queries are used to hide communication.

Once the connection is established, the attacker can issue commands, move laterally, and deploy additional payloads.

✅ **Key Takeaway:**  
Monitoring outbound traffic and unusual DNS activity can reveal C2 communications before major damage occurs.

---

## 🎯 Phase 7: Actions on Objectives

Finally, I reached the last phase — where attackers achieve their original goals.  
This can include:

- **Credential theft**  
- **Privilege escalation**  
- **Internal reconnaissance**  
- **Data exfiltration**  
- **Deleting backups and shadow copies**  

I studied how **Shadow Copy**, a Windows feature for creating system snapshots, is often deleted by attackers to prevent recovery during ransomware attacks.

✅ **Key Takeaway:**  
The attacker’s final actions reveal intent — whether espionage, data theft, or sabotage. Protecting backups and monitoring exfiltration channels is critical.

---

## 🧩 Practice Analysis: Target Data Breach

To put theory into practice, I analyzed the **2013 Target data breach**, one of the largest in history.  
I completed the interactive Cyber Kill Chain simulation by matching attack components to each phase:

| Phase | Example from Case Study |
|-------|--------------------------|
| **Weaponization** | PowerShell |
| **Delivery** | Spearphishing attachment |
| **Exploitation** | Exploit public-facing application |
| **Installation** | Dynamic linker hijacking |
| **Command & Control** | Fallback channels |
| **Exfiltration** | Data from local system |

After correctly completing the chain, the flag revealed was:
THM{7HR347_1N73L_12_4w35om3}


✅ **Key Insight:**  
By mapping each event to the Kill Chain, I could visualize how a single compromise evolved into a full-scale breach — reinforcing how breaking any one phase can stop the attack.

---

## 🧩 What I Learned

This case study strengthened my understanding of:
- How attackers move through a structured set of phases.  
- How defenders can “break the chain” by detecting indicators early.  
- The strengths and limitations of the traditional **Lockheed Martin Cyber Kill Chain**.  

I also recognized that while the model is powerful, it has limitations — especially in detecting **insider threats** or **multi-vector attacks**.  
That’s why modern defenders complement it with **MITRE ATT&CK** and the **Unified Kill Chain** for a more comprehensive approach.

---

## 🧭 Conclusion

The **Cyber Kill Chain** remains a foundational framework for threat detection and response.  
By understanding each stage, I learned how to:
- Identify attacker intent  
- Map threat behaviors  
- Strengthen organizational defenses  

Although cybersecurity threats continue to evolve, this structured framework helps analysts think like attackers — and defend more effectively.


---

**Tools & References Used:**
- OSINT Framework  
- theHarvester  
- Hunter.io  
- MITRE ATT&CK Framework  
- TryHackMe: Cyber Kill Chain Room



