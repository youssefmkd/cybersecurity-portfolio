# Architecture Cloud Sécurisée & Gouvernance des Identités

## Présentation

Dans le cadre de ce projet, j'ai conçu, déployé et sécurisé une infrastructure cloud multi-tiers reproduisant un environnement d'entreprise.

L'objectif était de mettre en œuvre une architecture intégrant plusieurs mécanismes de sécurité permettant de protéger les ressources, les données, les identités et les services, tout en améliorant la résilience de l'infrastructure.

Au cours de ce projet, j'ai travaillé sur différentes dimensions de la sécurité cloud : segmentation réseau, contrôle des flux, protection des applications, sécurité des machines virtuelles, gestion des identités, Zero Trust, contrôle d'accès, analyse des risques et protection contre les attaques DDoS.

Ce projet m'a également permis de développer une première sensibilisation aux enjeux de souveraineté numérique et de gouvernance des données. Bien que l'environnement ait été déployé sur Microsoft Azure, les principes de sécurité étudiés sont transposables à des environnements proposés par des acteurs du cloud souverain tels qu'OVHcloud, Scaleway ou 3DS OUTSCALE.

---

## Architecture de l'infrastructure 

J'ai commencé par concevoir une architecture cloud structurée autour de plusieurs composants réseau et services applicatifs.

L'objectif était de reproduire une infrastructure d'entreprise dans laquelle les différents services sont protégés et contrôlés selon leur rôle.

J'ai notamment travaillé sur :

- La création et la configuration de réseaux virtuels
- La segmentation des ressources réseau
- La mise en place de règles de sécurité réseau
- La protection des flux entrants
- Le déploiement d'une Application Gateway
- L'intégration d'un serveur Web IIS
- La surveillance des flux réseau

Cette approche permet de limiter la surface d'attaque et de contrôler les communications entre les différentes ressources de l'infrastructure.

<p align="center"> <img src="screenshots/Architecture.png" width="600"> </p>
*Figure 1 — Architecture globale de l'infrastructure cloud conçue avec Microsoft Visio.*

<p align="center"> <img src="screenshots/1-1.png" width="500"> </p>
*Figure 2 — Configuration des règles de sécurité entrantes du Network Security Group associé à la ressource SQL.*

<p align="center"> <img src="screenshots/1-2.png" width="500"> </p>
*Figure 3 — Règle de sécurité permettant l'accès RDP depuis la JumpBox.*

### Résultat
L'infrastructure dispose d'une première couche de segmentation et de filtrage permettant de contrôler les accès réseau et de limiter les flux entrants aux communications nécessaires.

---

## Surveillance et analyse des flux réseau

J'ai utilisé les fonctionnalités de surveillance réseau afin d'analyser les flux circulant dans l'environnement cloud.

L'objectif était de mieux comprendre les communications entre les différentes ressources et de disposer d'une visibilité sur les flux réseau autorisés ou bloqués.

J'ai notamment utilisé Network Watcher pour consulter les informations relatives aux flux réseau.

Cette approche permet d'améliorer la visibilité sur le comportement du réseau et facilite l'identification d'éventuels problèmes de connectivité ou de configurations réseau incorrectes.

<p align="center"> <img src="screenshots/2-1.png" width="500"> </p>
*Figure 4 — Analyse des flux réseau à l'aide de Network Watcher Flow Logs.*

### Résultat
La surveillance des flux permet d'obtenir une meilleure visibilité sur les communications réseau et de faciliter l'analyse des événements liés à la connectivité.

---



