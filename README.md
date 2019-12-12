# Anon-Circuit-Libre-Infra

## Présentation
Nom de l'équipe : **github..**

Membre de l'équipe : **Yannick**, **John**, **Elie**

Théme : **Tor**, **VPN**, **Docker** 

## Contexte

## Répartition du travail :

**Circuit tor & hidden service** -> John Marx

**Déploiement de VPN sur conteneur Docker** -> Yannick Courrian

**Basculement d'VPN** -> Elie Benayoun

## Schéma: Circuit sécurisé pour attaque réseaux.
![](https://i.imgur.com/0hEEMhP.png)

## Exigence   

### Machines :

- Client
- Attaquant

### Systèmes :

- tor service
- vpn server

### Actions :

#### Création
- déploiement de la machine client 

OS : 

IP : 192.168.56.101

PAQUETS : ssh, torify

* déploiement de la machine tor service 
  * OS : 
  * IP : 192.168.69.102 
  * PAQUETS : tor, ssh
 
- déploiement de la machine attaquant 

OS :

IP :

PAQUETS: docker, wireguard, nmap, telnet hping, sqlmap etc ..  

#### Cas d'usage
- connexion ssh au service tor.
- connexion à ssh à la machine "attaquant".
- connexion au vpn server.

## Maintien en condition opérationnelles
