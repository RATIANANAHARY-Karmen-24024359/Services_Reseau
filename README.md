# 🌐 Projet SAE 2.03 – Mise en place d’un réseau local (LAN)

## 📖 Introduction

Dans le cadre de la SAE 2.03, nous avons réalisé un projet de configuration réseau avec pour objectif la mise en place d’un **réseau local complet** composé de **trois machines virtuelles (VM)**. Ce projet a été mené en trinôme dans le contexte pédagogique de notre formation.

## 🧩 Objectifs du projet

Le projet consistait à configurer trois services réseau répartis sur trois machines distinctes :

- 🌐 **Serveur Web Apache** : hébergeant un site statique personnalisé
- 📧 **Serveur de messagerie** : installation de Postfix (envoi) + Dovecot (réception) et configuration du DNS secondaire
- 🧠 **Serveur DNS primaire** : résolution des noms de domaine associés aux services internes

---

## 🖥️ Infrastructure mise en place

| Nom de la VM    | Rôle(s)                          | Adresse IP       | Nom DNS              |
|-----------------|----------------------------------|------------------|-----------------------|
| **VM1 - Alvins**   | Serveur Web                      | `192.168.0.173`  | `www.valorant.fr`     |
| **VM2 - Simons**   | Serveur DNS primaire             | `192.168.0.222`  | `dns1.valorant.fr`    |
| **VM3 - Theodores**| Serveur mail + DNS secondaire    | `192.168.0.229`  | `dns2.valorant.fr`    |

> 💡 Les noms choisis pour les machines (Alvins, Simons, Theodores) font référence aux célèbres personnages de **"Alvin et les Chipmunks"**.

---

## ⚙️ Technologies utilisées

- **Linux Debian** (machines virtuelles)
- **Apache2** – Serveur HTTP
- **Postfix + Dovecot** – Serveur mail (SMTP + IMAP)
- **Bind9** – Serveur DNS
- **Netplan / ifconfig** – Configuration réseau
- **VMWare** – Environnement de virtualisation
- **Client Mail** - Thunderbird 

---

## 🧪 Étapes principales

1. Mise à jour du système (`apt update && apt upgrade`)
2. Configuration des adresses IP statiques
3. Installation et configuration de chaque service :
   - Apache sur VM1
   - DNS primaire sur VM2
   - Postfix, Dovecot, DNS secondaire sur VM3
4. Tests de connectivité (ping, nslookup, dig)
5. Vérification du fonctionnement global

---

## 👥 Membres du groupe

- **MEKIDICHE Idris**
- **RATIANANAHARY Karmen**
- **RINALDI Antoine**

Encadrante : **Mme YAHI Safa**

---

## 📎 Rapport

🔗 Le rapport complet détaillant les configurations est disponible ici :  
**[📄 Télécharger le rapport PDF](./rapport.pdf)** *(à ajouter dans le dépôt GitHub)*


