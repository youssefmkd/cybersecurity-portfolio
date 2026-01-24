---
layout: default
title: TryHackMe SOC Niveau 1
---

# 🛡️ TryHackMe SOC Niveau 1

Ce dossier contient mes **labs, exercices et études de cas TryHackMe SOC Niveau 1**, couvrant les fondamentaux du SOC, les investigations SIEM, la chasse aux menaces et la réponse aux incidents.

---

## 📂 Sections TryHackMe SOC Niveau 1

### 1. [Cadres de Défense Cyber](CDF/README.md)
- **Modules complétés:** Introduction Analyste Sécurité Junior, Pyramid of Pain, Cyber Kill Chain, Unified Kill Chain, Diamond Model, MITRE, Summit, Eviction  
- **Études de cas :**  
  1. [Cartographie MITRE ATT&CK](CDF/case-study-mitre.md) – Cartographie d’incidents réels sur les tactiques et techniques MITRE ATT&CK pour identifier les lacunes de détection.  
  2. [Simulation Cyber Kill Chain](CDF/case-study-killchain.md) – Analyse des étapes d’attaque dans un environnement simulé pour pratiquer la détection précoce et les stratégies de réponse.  

---

### 2. [Renseignement sur les Menaces Cyber (CTI)](CTI/README.md)
- **Modules complétés :** Introduction au Cyber Threat Intelligence, Outils de Threat Intelligence, Yara, OpenCTI, MISP, Friday Overtime, Trooper  
- **Études de cas :**  
  1. [Détection de Menaces avec YARA](CTI/case-study-yara.md) – Création et application de règles YARA pour détecter des motifs malware et des indicateurs de compromission.  
  2. [Investigation OpenCTI](CTI/case-study-opencti.md) – Suivi des TTP des acteurs malveillants avec OpenCTI, identification d’informations exploitables pour la défense.  

---

### 3. [Sécurité Réseau & Analyse du Trafic](Network/README.md)
- **Modules complétés :** Bases de l’Analyse du Trafic, Snort, Snort Challenge, NetworkMiner, Zeek, Wireshark, TShark, Brim  
- **Études de cas :**  
  1. [Challenge Attaques en Direct avec Snort](Network/case-study-snort-live.md) – Détection et analyse d’attaques réseau simulées à l’aide des règles IDS Snort et des modèles d’alerte.  
  2. [Analyse de Trafic Wireshark](Network/case-study-wireshark.md) – Examen des captures de paquets pour identifier des anomalies, protocoles suspects et potentielles exfiltrations de données.  

---

### 4. [Surveillance des Endpoints](Endpoint/README.md)
- **Modules complétés :** Processus Windows de Base, Sysinternals, Journaux Windows, Sysmon, Osquery, Wazuh  
- **Études de cas :**  
  1. [Analyse des Événements Sysmon](Endpoint/case-study-sysmon.md) – Création de détections et investigation des comportements suspects à partir des logs Sysmon.  
  2. [Détection Endpoint avec Wazuh](Endpoint/case-study-wazuh.md) – Utilisation de Wazuh pour collecter et analyser les logs des endpoints pour la détection et la surveillance des intrusions.  

---

### 5. [SIEM (Security Information and Event Management)](SIEM/README.md)
- **Modules complétés :** Introduction au SIEM, ELK101, ItsyBitsy (Splunk), Bases Splunk, Gestion des Incidents avec Splunk, Investigations avec Splunk  
- **Études de cas :**  
  1. [Gestion des Incidents avec Splunk](SIEM/case-study-incident-handling.md) – Investigation complète d’incident incluant détection, analyse et reporting.  

---

### 6. [Forensique Digitale & Réponse aux Incidents (DFIR)](DFIR/README.md)
- **Modules complétés :** Forensique Windows, Forensique Linux, Autopsy, Redline, Volatility, Velociraptor, TheHive, Introduction à l’Analyse Malware, Unattended, Disgruntled, Critical, Secret Recipe  
- **Études de cas :**  
  1. [Secret Recipe](DFIR/case-study-secret-recipe.md) – Cas DFIR complet incluant malware, activités internes et mouvements latéraux.  

---

### 7. [Analyse & Prévention du Phishing](PHISHING/README.md)
- **Modules complétés :** Fondamentaux du Phishing, Outils de Phishing, Greenholt Phish, Snapped Phish, Phishing Unfolding  
- **Études de cas :**  
  1. [Campagne Greenholt Phish](PHISHING/case-study-greenholt.md) – Analyse d’une campagne de phishing simulée pour identifier des emails malveillants, extraire des IOC et recommander des mesures de mitigation.  

---

### 8. [Défis Capstone SOC Niveau 1](SOC/README.md)
- **Modules complétés:** Tempest, Boogeyman Series (1–3), Upload and Conquer, Hidden Hooks, BlackCat  
- **Études de cas :**  
  1. [Tempest Challenge : Investigation complète](SOC/case-study-tempest.md) – Investigation SOC complète incluant triage des alertes, analyse d’activité PowerShell et identification de communications command-and-control.

---

## 📌 Compétences démontrées
- **SIEM & Analyse de Logs** : Splunk, ELK  
- **Réponse aux Incidents & DFIR** : Volatility, Autopsy, Redline  
- **Surveillance des Endpoints** : Sysmon, Sysinternals, Wazuh  
- **Analyse du Phishing** : Analyse des en-têtes et pièces jointes emails  
- **Défense Réseau** : Snort, Zeek, Wireshark  
- **Threat Intelligence** : Yara, OpenCTI, MISP

---

## Navigation
- Retour à [Accueil du Portfolio](../index.md)
