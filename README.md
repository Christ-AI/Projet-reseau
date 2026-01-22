# Projet Réseau — Cisco Packet Tracer (Labs)

Ce dépôt regroupe mes **maquettes réseau Cisco Packet Tracer**.  
Objectif : consolider mes bases en **configuration IOS**, **adressage IPv4**, **switching**, **tests de connectivité** et utilisation du **mode Simulation**.

---

## Structure actuelle du dépôt
Projet-reseau/
├─ labs/

│ └─ lab-01/

│ └─ (fichiers du lab, dont topology.pkt)

├─ LAB 2 cisco git.pkt

├─ README.md

├─ .gitignore

└─ .gitattributes

### À propos des fichiers `.pkt`
- `labs/lab-01/` contient le **Lab 01** (organisation recommandée : un dossier par lab).
- `LAB 2 cisco git.pkt` (à la racine) est une **maquette Packet Tracer** supplémentaire ou une version/variante.
  - Si c’est un doublon, il pourra être supprimé plus tard.
  - Si c’est un autre lab, il sera déplacé dans `labs/lab-02/` quand tu voudras ranger proprement.

---

## Lab 01 — Introduction (Routeur + Switch + postes)
### Objectifs
- Créer une topologie simple (routeur, switch, PCs)
- Configurer les équipements via la CLI :
  - `hostname`
  - mots de passe (mode utilisateur / privilégié)
  - chiffrement des mots de passe
  - sauvegarde de configuration
- Configurer un plan IP statique sur les postes
- Valider la connectivité via **ping**
- Observer le trafic (ARP/ICMP) via le **mode Simulation**
- Comprendre l’apprentissage MAC côté switch

### Plan d’adressage (exemple)
- PC1 : `192.168.1.1`
- PC2 : `192.168.1.2`
- PC3 : `192.168.1.3`

> Si une passerelle est configurée (ex: interface LAN du routeur), la préciser dans la doc du lab.

---

## Commandes de vérification utiles
### Switch
- Table MAC : `show mac address-table`
- État ports : `show interfaces status`

### Routeur
- Interfaces : `show ip interface brief`
- Routes : `show ip route`
- Config : `show running-config`

### Tests
- Ping entre les postes (PC1 ⇄ PC2 ⇄ PC3)

---

## Comment utiliser ce dépôt
1. Ouvrir le fichier `.pkt` souhaité dans **Cisco Packet Tracer**
2. Pour le Lab 01 : ouvrir le dossier `labs/lab-01/` et charger la topologie
3. Tester la connectivité (ping) et vérifier les configurations via CLI
4. Passer en **Simulation mode** pour observer les échanges (ARP, ICMP)

---

## Bonnes pratiques (évolution future)
Pour rendre le dépôt plus lisible et “portfolio-ready”, l’idée est d’ajouter au fil du temps :
- `configs/` : exports `running-config` en `.txt` (R1, SW1, etc.)
- `screenshots/` : captures de validation (ping OK, table MAC, routes, etc.)
- un `README.md` par lab dans `labs/lab-01/README.md`

---

## Licence
Projet personnel à usage d’apprentissage.
