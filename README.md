# Infrastructure LAN sécurisée – Cisco Packet Tracer

Ce projet est une simulation réseau réalisée avec Cisco Packet Tracer. Il met en place une infrastructure LAN sécurisée avec :

- 3 VLANs (Admin, RH, Visiteurs)
- Routage inter-VLAN via un routeur
- Règles ACL pour filtrer les communications

## Objectifs pédagogiques
- Comprendre le fonctionnement des VLANs
- Apprendre à configurer le routage inter-VLAN
- Mettre en œuvre des ACL pour la sécurité réseau

## Schéma réseau
![Schéma réseau](captures/schema-vlan.png)

## Configuration utilisée

- **Switch 2960** :
  - VLAN 10 : Admin
  - VLAN 20 : RH
  - VLAN 30 : Visiteurs

- **Routeur 2911** :
  - Sous-interfaces configurées pour chaque VLAN
  - ACL pour interdire l'accès du VLAN 30 vers le VLAN 10

## Test
- Ping réussi entre Admin et RH
- Ping bloqué entre Visiteurs et Admin (grâce aux ACL)

## À venir
- Ajout de DHCP
- Ajout de monitoring via SNMP

## Auteur
Thomas Makosso
