# 🔗 Étude de Cas : Cyber Kill Chain

## Vue d’ensemble

Dans cette étude de cas, j’ai exploré le **framework Cyber Kill Chain**, développé par **Lockheed Martin** en 2011.  
Initialement un **concept militaire** décrivant les étapes d’une attaque, ce framework a été adapté à la cybersécurité pour aider les analystes à comprendre et interrompre les intrusions numériques.

La Cyber Kill Chain décrit **sept phases clés** d’une cyberattaque :

1. Reconnaissance  
2. Weaponization (Préparation de l’attaque)  
3. Livraison (Delivery)  
4. Exploitation  
5. Installation  
6. Command & Control (C2)  
7. Actions sur les objectifs  

Comprendre ces étapes permet aux analystes de **détecter, perturber et se défendre** contre les cyberattaques — en particulier les campagnes de **ransomware**, les **intrusions** et les **APT (Advanced Persistent Threats)**.

---

## 🧠 Mon approche

J’ai commencé par étudier comment la **Cyber Kill Chain** traduit le workflow de l’attaquant en étapes identifiables.  
L’objectif était de comprendre comment chaque phase laisse des **empreintes numériques** détectables et exploitables par les défenseurs.

Pour ce projet, j’ai analysé chaque étape via un scénario fictif avec un attaquant nommé **“Megatron”**, afin de comprendre comment les adversaires planifient, exécutent et maintiennent leurs opérations cyber.

---

## 🕵️‍♂️ Phase 1 : Reconnaissance

La **reconnaissance** consiste à collecter des informations sur la cible via **OSINT (Open Source Intelligence)** :  
- Analyse de l’infrastructure de l’entreprise  
- Identification des employés  
- Collecte des contacts  

Outils couramment utilisés par les attaquants :
- **theHarvester** – collecte d’e-mails, sous-domaines et IP.  
- **Hunter.io** – recherche d’adresses e-mail publiques.  
- **OSINT Framework** – interface web organisant les outils de reconnaissance.  

Cette étape montre l’importance de **limiter l’exposition publique des informations sensibles** et de former le personnel contre le **social engineering**.

✅ **Points clés :**  
- La reconnaissance prépare et guide l’attaque.  
- Les données OSINT constituent une mine d’informations pour les attaquants et un indicateur à surveiller pour les défenseurs.

---

## ⚔️ Phase 2 : Weaponization (Préparation de l’attaque)

Une fois la reconnaissance terminée, les attaquants créent leur **charge utile** combinant **malware** et **exploits**.

J’ai analysé :
- **Malware** : logiciel visant à endommager ou infiltrer des systèmes.  
- **Exploit** : code exploitant une vulnérabilité.  
- **Payload** : code malveillant exécuté sur le système.  

Les attaquants peuvent intégrer des **macros** dans des documents Office via des **scripts VBA** pour automatiser l’infection.  
Les groupes avancés créent parfois des malwares sur mesure ou les achètent sur le **Dark Web** pour échapper à la détection.

✅ **Point clé :**  
Même un document Word peut devenir une arme via des macros malveillantes — d’où l’importance de rester vigilant avec les pièces jointes.

---

## 📧 Phase 3 : Livraison (Delivery)

C’est la phase où la charge utile atteint la victime.  
Les méthodes courantes incluent :  
- **Emails de phishing** (y compris spearphishing pour attaques ciblées)  
- **Clés USB infectées** (attaques de type « USB drop »)  
- **Watering hole** : site de confiance compromis pour livrer le malware  

Le **watering hole** est particulièrement dangereux car il cible des sites visités fréquemment par les victimes, rendant l’attaque discrète et efficace.

✅ **Point clé :**  
La livraison combine psychologie humaine et exploitation technique — la sensibilisation reste une défense essentielle.

---

## 💣 Phase 4 : Exploitation

Les attaquants exploitent les vulnérabilités pour exécuter la charge utile.  
Exemples : clic sur un lien malveillant ou ouverture d’une pièce jointe infectée.

- **Zero-day exploits** : vulnérabilités inconnues, laissant peu de temps pour patcher.  
- Exploitation de failles logicielles ou erreurs humaines pour accès distant.

✅ **Point clé :**  
L’exploitation est là où **prévention et détection se croisent** — gestion des patches et protection des endpoints sont cruciales.

---

## 🧬 Phase 5 : Installation

Une fois l’accès obtenu, les attaquants cherchent à assurer la **persistance** : revenir après redémarrage ou nettoyage.

Techniques courantes :
- Déploiement de **web shells**  
- Installation de **backdoors** via **Meterpreter**  
- Modification des services Windows ou **clés de registre** pour exécution automatique  
- **Timestomping** pour masquer les traces

✅ **Point clé :**  
La persistance permet aux attaquants de se fondre parmi les processus légitimes. Détecter des modifications inhabituelles est essentiel.

---

## 🌐 Phase 6 : Command & Control (C2)

Création d’un canal **C2** pour contrôler les systèmes infectés.

Méthodes typiques :
- **Beaconing HTTP/HTTPS** (ports 80/443)  
- **DNS Tunneling** pour masquer la communication  

Une fois établi, l’attaquant peut donner des commandes, se déplacer latéralement et déployer des charges supplémentaires.

✅ **Point clé :**  
Surveiller le trafic sortant et les anomalies DNS peut révéler les communications C2 avant des dommages majeurs.

---

## 🎯 Phase 7 : Actions sur les Objectifs

Phase finale : réalisation des objectifs initiaux de l’attaquant, par exemple :  
- Vol de credentials  
- Escalade de privilèges  
- Reconnaissance interne  
- Exfiltration de données  
- Suppression de sauvegardes ou Shadow Copies  

✅ **Point clé :**  
Les actions finales révèlent l’intention : espionnage, vol de données ou sabotage. Protéger les sauvegardes et surveiller l’exfiltration est crucial.

---

## 🧩 Analyse Pratique : Fuite de données Target 2013

Simulation pratique de la **Cyber Kill Chain** avec la fuite Target, l’une des plus grandes de l’histoire.

| Phase | Exemple |
|-------|---------|
| **Weaponization** | PowerShell |
| **Delivery** | Pièce jointe spearphishing |
| **Exploitation** | Application publique vulnérable |
| **Installation** | Dynamic linker hijacking |
| **Command & Control** | Canaux de fallback |
| **Exfiltration** | Données locales |

✅ **Point clé :**  
Cartographier chaque événement sur la Kill Chain permet de visualiser comment une intrusion unique évolue en une brèche complète — interrompre n’importe quelle phase peut stopper l’attaque.

---

## 🧩 Leçons Apprises

Cette étude a renforcé ma compréhension de :  
- La progression des attaquants à travers des phases structurées  
- Comment les défenseurs peuvent **interrompre la chaîne** en détectant tôt les indicateurs  
- Les forces et limites de la **Lockheed Martin Cyber Kill Chain**  

Elle montre aussi la nécessité de compléter le modèle avec **MITRE ATT&CK** ou la **Unified Kill Chain** pour une vision plus complète.

---

## 🧭 Conclusion

La **Cyber Kill Chain** reste un cadre fondamental pour la détection et la réponse aux menaces.  
Elle permet de :  
- Identifier l’intention des attaquants  
- Cartographier les comportements malveillants  
- Renforcer les défenses organisationnelles  

Bien que les menaces évoluent, ce cadre aide les analystes à **penser comme les attaquants** et à défendre plus efficacement.

---

**Outils & Références :**
- OSINT Framework  
- theHarvester  
- Hunter.io  
- MITRE ATT&CK Framework  
- TryHackMe : Cyber Kill Chain Room
