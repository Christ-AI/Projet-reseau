# Projet Réseau Cisco Packet Tracer – Lab 0 : Introduction

## 🚀 Présentation du projet

Ce projet personnel vise à maîtriser l’utilisation de **Cisco Packet Tracer** en créant une maquette réseau simple composée d’un routeur, d’un switch et de plusieurs postes clients. L’objectif est d’acquérir les compétences pratiques nécessaires pour configurer les équipements réseau via la ligne de commande, gérer la sécurité basique par mot de passe, et tester la connectivité entre les machines.

---

## 🎯 Objectifs techniques

- Reproduction fidèle d’une maquette réseau typique (routeur, switch, PCs).
- Configuration des équipements avec des noms clairs (`R1`, `SW1`, `PC1` à `PC3`).
- Mise en place de mots de passe sécurisés, avec chiffrement.
- Configuration d’adresses IP statiques sur les postes clients.
- Validation de la connectivité réseau via des tests ping.
- Utilisation avancée du mode simulation pour observer le trafic réseau et le comportement des équipements.
- Gestion des tables d’adresses MAC sur le switch.

---

## ⚙️ Détails de la configuration

- **Routeur (R1) et Switch (SW1)** :
  - Renommage via la commande `hostname`.
  - Configuration des mots de passe pour les modes EXEC utilisateur et privilégié.
  - Cryptage des mots de passe en configuration.
  - Sauvegarde des configurations.

- **Postes clients (PC1, PC2, PC3)** :
  - Configuration manuelle des adresses IP :
    - PC1 : 192.168.1.1
    - PC2 : 192.168.1.2
    - PC3 : 192.168.1.3

- **Tests de connectivité** :
  - Ping entre les PCs pour vérifier la communication.
  - Analyse du trafic réseau en mode simulation.

---

## 📂 Contenu du dépôt

- `Lab2_PacketTracer.pkt` : fichier Cisco Packet Tracer contenant la maquette complète et les configurations.
- `README.md` : ce document explicatif.

---

## 🔗 Utilisation

1. Téléchargez et ouvrez le fichier `Lab0_PacketTracer.pkt` avec **Cisco Packet Tracer**.
2. Explorez la configuration de chaque équipement via la CLI.
3. Testez les communications entre les PCs à l’aide de commandes ping.
4. Activez le mode simulation pour visualiser le trafic et le comportement des switches.

---

## 🛠️ Technologies utilisées

- Cisco Packet Tracer
- Protocoles réseau de base (Ethernet, IP)
- Commandes IOS Cisco pour configuration et gestion

---

## 📖 Notes

Ce projet est une base pour approfondir mes compétences réseau dans un environnement virtuel. Il peut évoluer vers des configurations plus avancées (VLANs, routage dynamique, sécurité renforcée, etc.).

---

## 📄 Licence

Projet personnel à usage d’apprentissage.

