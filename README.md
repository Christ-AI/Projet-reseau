# Projet Réseau — Cisco Packet Tracer (Labs)

Ce dépôt regroupe mes **labs Cisco Packet Tracer** (topologies `.pkt` + documentation).  
Objectif : consolider mes bases en **adressage IP, switching, configuration IOS, tests de connectivité** et observation du trafic en simulation.

---

## Structure du dépôt
Projet-reseau/

├─ labs/

│ └─ lab-01/

│ ├─ topology.pkt

│ ├─ Lab2_PacketTracer.pkt

│ ├─ README.md

│ ├─ configs/ (optionnel)

│ └─ screenshots/ (optionnel)


├─ assets/ (optionnel)

├─ .gitattributes (Git LFS pour .pkt/.pka)

├─ .gitignore

└─ README.md

### Pourquoi 2 fichiers `.pkt` ?
- `topology.pkt` : version **standardisée** (nom générique, facile à retrouver)
- `Lab2_PacketTracer.pkt` : version **originale** (nom d’origine du fichier)

> Recommandation : garder **un seul fichier `.pkt`** par lab (idéalement `topology.pkt`) et supprimer/archiver l’autre pour éviter la confusion.

---

## Lab 01 — Introduction (Routeur + Switch + 3 PCs)

### Objectifs
- Construire une topologie simple (R1, SW1, PC1–PC3)
- Configurer des paramètres de base via Cisco IOS (hostname, mots de passe, chiffrement)
- Attribuer des adresses IP statiques aux PCs
- Valider la connectivité via `ping`
- Observer le trafic en **Simulation mode** (ARP, ICMP)
- Comprendre la table MAC du switch

### Plan d’adressage (exemple)
- PC1 : `192.168.1.1`
- PC2 : `192.168.1.2`
- PC3 : `192.168.1.3`

> Si une passerelle est configurée, la préciser dans `labs/lab-01/README.md`.

---

## Commandes de vérification utiles
### Switch (SW1)
- Table MAC : `show mac address-table`
- Interfaces : `show interfaces status`

### Routeur (R1)
- Interfaces : `show ip interface brief`
- Configuration : `show running-config`

### Tests
- Ping entre PC1 ⇄ PC2 ⇄ PC3

---

## Utilisation
1. Ouvrir un fichier `.pkt` avec **Cisco Packet Tracer**
2. Lire la documentation du lab : `labs/lab-01/README.md`
3. Tester la connectivité (ping)
4. Passer en mode simulation pour observer les échanges

---

## Bonnes pratiques (portfolio)
Pour rendre le dépôt plus “recruteur-friendly” :
- Exporter les configurations en `.txt` dans `labs/lab-01/configs/` :
  - `R1_running-config.txt`
  - `SW1_running-config.txt`
- Ajouter 2–3 captures dans `labs/lab-01/screenshots/` (ping OK, table MAC, etc.)

---

## Licence
Projet personnel à usage d’apprentissage.
