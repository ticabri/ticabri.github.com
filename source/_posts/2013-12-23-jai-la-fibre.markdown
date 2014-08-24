---
layout: post
title: "Réveillez la fibre optique qui est en vous"
date: 2013-12-23 13:54
comments: true
categories: développement
---

{% img right http://cl.ly/image/3N3m0H1x1f1B/3182912188.png Speedtest carte réseau Gigabit %}

_Retour d'expérience sur la fibre optique fraichement installée chez moi._

Le NRA (nœud de raccordement) dans le quartier est à 3500m, soit 49 dB d’atténuation de signal. Pour l'expliquer à Madame Michu : je téléchargeais en moyenne à 400 ko/s, soit un épisode de The Big Bang Theory (~ 350 Mo) – comment ça Madame Michu ne regarde pas TBBT ? – en 15 minutes. J’aime aussi préciser que malgré le décodeur numérique designé par Starck, je ne pouvais regarder la tv hd, ni surfer et regarder la tv basse définition simultanément.

<!-- more -->

La fibre en détails !
---

Il faut reprendre quelques habitudes. Cette fois pas de décodeur tv, économie sur la redevance, le temps de cerveau disponible et sur l’abonnement internet. Merci aux forfaits modulables de SFR. Mais est-ce que la technique suit ?

On peut le dire ! La fibre offre trois avantages :

- un ping resserré à 14 ms
- une bande passante descendante à 290 Mbps
- une bande passante montante à 50 Mbps

Ces mesures sont prises depuis un ordinateur avec une carte réseau Gigabit branchée à la box par un rj45 Gigabit. C’est vraiment pas mal, surtout pour l’upload : 50 Mbps, ça fait quand même des envois à 6 Mo/s contre 125 ko/s pour une ligne ADSL classique.
Le download sur la meilleure ligne ADSL que j’ai eue est monté à 1,5 Mo/s, soit du 12 Mbps. Les fournisseurs annoncent tout de même une technologie pouvant atteindre les 20 Mbps, passons.

Les débits n’ont absolument rien à voir avec de l’ADSL. Et même si un gros download est très agréable pour télécharger – sur une ligne ADSL de très bonne qualité, le même épisode de The Big Bang Theory ne prendrait que 4 minutes à être téléchargé – la différence se fait surtout sentir sur l’upload. L’upload est le A de ADSL, qui veut dire asymetric, point faible de la technologie ADSL.

{% img center http://cl.ly/image/3N3m0H1x1f1B/3182912188.png Speedtest carte réseau Gigabit %}

Bottleneck
---

Malheureusement le bottleneck se déplace. Désormais c’est la carte wifi ou le serveur ou le VPN qui limitent les débits. Sur une tablette Nexus 7, on ne dépasse pas les 20 Mbps en download (2,5 Mo/s), ~~via le wifi 802.11n on est limité à 50 Mbps (6,25 Mo/s)~~ le wifi 802.11n a des limites d'environ 100-150 Mbps. En revanche, même sur speedtest, les serveurs ont leurs propres limites et réseaux, aussi il faut regarder les chiffres avec une bonne marge.

Les limitations du VPN sont évidemment dépendantes de la solution choisie et des positions géographiques des serveurs. Mes tests s’effectuent à travers les serveurs de VyprVPN (ping ; download ; upload) :

ping    | download  | upload  | lieu              | speedtest
---     | ---       | ---     | ---               | ---
100 ms  | 22 Mbps   | 5 Mbps  | Washington, USA   | ![image](http://cl.ly/image/1W17191N3I3w/3182943632.png "VyprVPN USA")
62 ms   | 12 Mbps   | 11 Mbps | Reykjavik, Island | ![image](http://cl.ly/image/02292G0r2p34/3182947376.png "VyprVPN Island")
40 ms   | 23 Mbps   | 19 Mbps | Paris, France     | ![image](http://cl.ly/image/0c1G2r1h281p/3182950615.png "VyprVPN Paris")
58 ms   | 46 Mbps   | 12 Mbps | Vienna, Autria    | ![image](http://cl.ly/image/1U3v2i3a1X1c/3182955706.png "VyprVPN Autria")

etc…
