# 🧩 Diamond Model of Intrusion Analysis

## Overview

In this case study, I explored the **Diamond Model of Intrusion Analysis**, a framework that provides a structured way to understand and communicate about cyber intrusions. Developed by **Sergio Caltagirone, Andrew Pendergast, and Christopher Betz (2013)**, the Diamond Model connects key components of an intrusion event to help analysts visualize the relationships between threat actors, their tools, and their victims.

---

## 🧠 What I Did

I began by studying the **core structure** of the Diamond Model, which is built around four fundamental features:

- **Adversary** – The individual or group conducting the attack.  
- **Infrastructure** – The systems, domains, or networks used by the adversary.  
- **Capability** – The tools and techniques (TTPs) leveraged during the intrusion.  
- **Victim** – The individual, system, or organization targeted.

These four nodes form the “diamond,” with relationships represented by the edges. The framework helps visualize **how the attacker interacts with their tools and targets**, and how those relationships evolve during an intrusion.

I explored how the model introduces **two axes** for context:

- **Social-Political Axis** – Represents the adversary’s motivations, goals, or external pressures.  
- **Technology Axis** – Represents the technical link between capability and infrastructure.

---

## 🧩 Breaking Down the Components

### Adversary

I learned that an **adversary** is not always a single hacker but can represent multiple roles:

- **Adversary Operator:** The individual executing the attack.  
- **Adversary Customer:** The entity benefiting from it.

Understanding this distinction helps analysts assess **intent, persistence, and adaptability**.  
Through exercises, I identified these roles in simulated attacks and learned how intelligence analysts can use collected indicators to link campaigns back to specific threat actors.

---

### Victim

Next, I studied how the model classifies **victims** into:

- **Victim Personae** (people, organizations, or industries targeted)
- **Victim Assets** (systems, networks, or email accounts exploited)

I saw how this framework helps analysts trace the adversary’s intent — whether they aim to steal data, disrupt operations, or infiltrate a specific sector.

---

### Capability

In this part, I analyzed **capability**, which covers the adversary’s tools, malware, and techniques.

I learned two key subcomponents:
- **Capability Capacity** – The vulnerabilities or weaknesses exploited.  
- **Adversary Arsenal** – The full collection of tools available to the attacker.

By reviewing case data, I recognized how mapping out an adversary’s arsenal (like malware families or exploit kits) can show how their sophistication evolves over time.

---

### Infrastructure

Here, I explored the systems used to launch or manage attacks.  
The model distinguishes between:

- **Type 1 Infrastructure** – Controlled directly by the adversary.  
- **Type 2 Infrastructure** – Managed by intermediaries (knowingly or unknowingly), often to hide attribution.

Through examples like **malicious domains, C2 servers, and compromised email accounts**, I learned how these infrastructure layers support the attack lifecycle and how analysts use DNS or IP analysis to uncover them.

---

## ⚙️ Meta Features

The Diamond Model also includes **six meta-features** that add analytical depth:

- **Timestamp:** Helps track when and how attacks occur.  
- **Phase:** Links to the **Cyber Kill Chain** stages.  
- **Result:** Indicates whether the attacker succeeded or failed.  
- **Direction:** Defines the flow (e.g., Victim → Infrastructure).  
- **Methodology:** Describes the intrusion type (phishing, DDoS, etc.).  
- **Resources:** Identifies what the attacker needed (software, credentials, funds).

I learned how these features allow analysts to document intrusions systematically, making them easier to share and compare across incidents.

---

## 🕵️‍♂️ Practice Analysis

Finally, I completed the **interactive diamond analysis exercise**.  
Using the provided case study, I analyzed a simulated intrusion involving a ransomware attack:

- **Adversary:** APT2166  
- **Timestamp:** 2021-10-23 15:45:00  
- **Victim:** Corporation IT Systems  
- **Capability:** Use of stolen credentials via phishing  
- **Resources:** OneTrick malware campaign  
- **Methodology:** Internal pivoting and lateral movement  
- **Result:** Data exfiltration and sale on underground forums  
- **Framework:** Lockheed Martin’s Cyber Kill Chain  

After filling in all sections, the flag displayed was:

---

## 🎯 What I Learned

This exercise gave me a **stronger understanding of structured intrusion analysis**.  
I learned how to:

- Break down complex attack data into **clear, relational elements**.  
- Identify how adversaries connect their **tools, infrastructure, and objectives**.  
- Use the model to improve **communication and intelligence sharing** within SOC environments.  
- Apply theoretical frameworks like the **Diamond Model** and **Kill Chain** to real-world threat analysis.

In summary, I discovered how the Diamond Model acts as a **bridge between raw incident data and actionable intelligence**, making it a valuable framework for any security analyst or threat hunter.



