# TP2
*promis le 1 arrive vite* 

## 1 Simplest setup

topologie :

![topologie](https://github.com/Badjeck/TP_reseau/blob/master/TP2/images/2.1topo.PNG)

ping :

![Ping](https://github.com/Badjeck/TP_reseau/blob/master/TP2/images/2.1ping.PNG)

wireshark PC1 ping PC2 :

![](https://github.com/Badjeck/TP_reseau/blob/master/TP2/images/2.1wiresharkping.PNG)

Wireshark echange arp :

![](https://github.com/Badjeck/TP_reseau/blob/master/TP2/images/2.1arp.PNG)

### Étapes d'un ping
- pc1 envoie un requête arp en broadcast pour que tout le monde ai sont ip et sa MAC
- Pc2 le recoit et lui envoie sa mac et son ip en retour
- Pc1 envoi ping a pc2
- Pc2 lui répond

Un switch n'a pas d'ip car c'est juste une passerelle, par contre un pc lui doit recevoir et envoyer d'un info donc requière une ip.

## 2 More switch

Topologie :

![](https://github.com/Badjeck/TP_reseau/blob/master/TP2/images/2.2topo.PNG)

ping :

![](https://github.com/Badjeck/TP_reseau/blob/master/TP2/images/2.2ping.PNG)

mac : 

![](https://github.com/Badjeck/TP_reseau/blob/master/TP2/images/2.2mac.PNG)

On remarque que le switch1 coco les adresses mac du switch 2 et 3 ansi que sa propre mac mais pas celles des pc.

Le dieu wikipédia a dit dans sa clairvoyante bonté:
 "Le Cisco Discovery Protocol (CDP) est un protocole de découverte de réseau de niveau 2 développé par Cisco Systems qui permet, avec SNMP, de trouver d'autres périphériques voisins directement connectés (routeur, switch, pont, etc.). Il s'utilise avec des commandes IOS. CDP est indépendant des médias qu'il parcourt. Par défaut, les annonces CDP sont envoyées toutes les 60 secondes sur les interfaces qui prennent en charge SNAP, ce qui comprend les médias physiques comme les LAN Ethernet, le Frame Relay et l'Asynchronous transfer mode (ATM). Les informations sont envoyées par une adresse multicast. La version la plus récente est la CDPv2. "

et comme le disais un grand sage: "tout ce qui est sur internet est vrai"

