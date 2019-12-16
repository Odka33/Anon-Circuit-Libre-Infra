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
* déploiement de la machine client 
  * OS : 
  * IP : 192.168.59.101
  * PAQUETS : torify, ssh

* déploiement de la machine tor service 
  * OS : 
  * IP : 192.168.69.102 
  * PAQUETS : tor
 
* déploiement de la machine attaquant 
  * OS :
  * IP : 192.168.79.103
  * PAQUETS: docker, wireguard-client, nmap, telnet hping, sqlmap etc ..  

* déploiement de conteneur docker
  * OS :
  * IP :192.168.79.104,105,106
  * PAQUETS: wireguard-server
  
#### Cas d'usage
* connexion ssh au service tor.
  * ```torify ssh user@abcdefghijklmnop.onion```
* connexion à ssh à la machine "attaquant".
  * ```ssh user@192.168.79.103```
* connexion au vpn server.
  * ```sudo wg```
  
## Maintien en condition opérationnelles

## Sources :

* https://medium.com/@tzhenghao/how-to-ssh-over-tor-onion-service-c6d06194147

