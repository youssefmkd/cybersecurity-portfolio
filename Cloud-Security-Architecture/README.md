# Architecture Cloud Sécurisée & Gouvernance des Identités

## Présentation

Dans le cadre de ce projet, j'ai conçu, déployé et sécurisé une infrastructure cloud multi-tiers reproduisant un environnement d'entreprise. L'objectif était de mettre en œuvre une architecture robuste intégrant les principaux mécanismes de sécurité cloud afin de protéger les identités, les données, les ressources et les services tout au long de leur cycle de vie.

Au-delà de l'implémentation technique, ce projet m'a permis d'adopter une approche orientée Cloud Security, Zero Trust, Identity & Access Management (IAM) et défense en profondeur, tout en développant une sensibilité aux enjeux de souveraineté numérique. Bien que l'environnement ait été déployé sur Microsoft Azure, les principes de sécurité appliqués sont transposables aux plateformes de cloud souverain telles qu'OVHcloud, Scaleway ou 3DS OUTSCALE.

---

## Architecture de l'infrastructure 

L'infrastructure est organisée selon une architecture multi-tiers afin de séparer les différentes couches de l'application et de réduire la surface d'attaque.

Elle comprend notamment :

- Un réseau virtuel segmenté en plusieurs sous-réseaux
- Des machines virtuelles réparties par rôle
- Une séparation des couches Web, Application, Données et Administration
- Des contrôles réseau via les Network Security Groups (NSG)
- Une gestion centralisée des identités
- Des mécanismes de chiffrement et de supervision

<p align="center"> <img src="screenshots/Architecture.png" width="100%"> </p>

---

## Déploiement de l'infrastructure

