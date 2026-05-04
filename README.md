# TP-TCP-UDP-README.md
# TP TCP vs UDP – Couche transport

## Objectif

Comprendre le rôle de la couche transport et différencier les protocoles TCP et UDP.

## Contexte

La couche transport permet aux applications de communiquer sur le réseau.  
Elle utilise principalement deux protocoles : TCP et UDP.

TCP privilégie la fiabilité, tandis qu’UDP privilégie la rapidité.

## TCP

TCP est un protocole orienté connexion.  
Avant l’échange de données, une connexion est établie avec une poignée de main en trois temps.

TCP garantit :

- la livraison des données ;
- l’ordre des segments ;
- la retransmission en cas de perte ;
- le contrôle de flux ;
- le contrôle de congestion.

Exemples d’utilisation :

- HTTP / HTTPS ;
- FTP ;
- SSH ;
- SMTP ;
- IMAP.

## UDP

UDP est un protocole sans connexion.  
Il envoie les datagrammes sans établir de session et sans garantie de livraison.

UDP est plus rapide, mais moins fiable.

Exemples d’utilisation :

- DNS ;
- VoIP ;
- streaming ;
- jeux en ligne ;
- DHCP.

## Comparaison

| Élément | TCP | UDP |
|---|---|---|
| Connexion | Oui | Non |
| Fiabilité | Élevée | Faible |
| Vitesse | Plus lent | Plus rapide |
| Ordre des paquets | Garanti | Non garanti |
| Retransmission | Oui | Non |
| Cas d’usage | Web, mail, SSH | DNS, VoIP, streaming |

## Résultat retenu

TCP est utilisé lorsque les données doivent arriver complètes et dans l’ordre.  
UDP est utilisé lorsque la vitesse et la faible latence sont prioritaires.

## Compétences mobilisées

- Compréhension de la couche transport
- Analyse TCP/UDP
- Choix du protocole selon le besoin
