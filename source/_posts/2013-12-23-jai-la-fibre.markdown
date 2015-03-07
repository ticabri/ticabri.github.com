---
layout: post
title: "Réveillez la fibre optique qui est en vous"
date: 2013-12-23 13:54
comments: true
categories: développement
---

{% img right http://www.speedtest.net/result/4195946321.png Speedtest carte réseau Gigabit %}

_Retour d'expérience sur la fibre optique fraichement installée chez moi._

Le NRA (nœud de raccordement) dans le quartier est à 3500m, soit 49 dB d’atténuation de signal. Pour l'expliquer à Madame Michu : je téléchargeais en moyenne à 400 ko/s (_~0.4 Mo/s_), soit un épisode de The Big Bang Theory (~ 350 Mo) – comment ça Madame Michu ne regarde pas TBBT ? – en 15 minutes. J’aime aussi préciser que malgré le décodeur numérique designé par Starck, je ne pouvais regarder la tv hd, ni surfer et regarder la tv basse définition simultanément.

<!-- more -->

La fibre en détails !
---

Il faut reprendre quelques habitudes. Cette fois pas de décodeur tv, économie sur la redevance, le temps de cerveau disponible et sur l’abonnement internet. Merci aux forfaits modulables de SFR. Mais est-ce que la technique suit ?

On peut le dire ! La fibre offre trois avantages :

- un ping resserré à 18 ms
- une bande passante descendante à 290 Mbps
- une bande passante montante à 50 Mbps

Ces mesures sont prises depuis un ordinateur avec une carte réseau Gigabit branchée à la box par un rj45 Gigabit. C’est vraiment pas mal, surtout pour l’upload : 50 Mbps, ça fait quand même des envois à 6 Mo/s contre 125 ko/s pour une ligne ADSL classique.
Le download sur la meilleure ligne ADSL que j’ai eue est monté à 1,5 Mo/s, soit du 12 Mbps. Les fournisseurs ADSL annoncent tout de même une technologie pouvant atteindre les 20 Mbps, passons.

Les débits n’ont absolument rien à voir avec de l’ADSL. Et même si un gros download est très agréable pour télécharger – sur une ligne ADSL de très bonne qualité, le même épisode de The Big Bang Theory ne prendrait que 4 minutes à être téléchargé – la différence se fait surtout sentir sur l’upload. L’upload est caché dans le A de ADSL, qui veut dire asymetric, point faible de la technologie ADSL.

{% img center http://www.speedtest.net/result/4195943939.png Speedtest carte réseau Gigabit %}

Bottleneck
---

Malheureusement le bottleneck se déplace. Désormais c’est la carte wifi ou le serveur ou le VPN qui limitent les débits. Sur une tablette Nexus 7, on ne dépasse pas les 20 Mbps en download (2,5 Mo/s), ~~via le wifi 802.11n on est limité à 50 Mbps (6,25 Mo/s)~~ le wifi 802.11n a des limites d'environ 100-150 Mbps. En revanche, même sur speedtest, les serveurs ont leurs propres limites et réseaux, aussi il faut regarder les chiffres avec une bonne marge.

Les limitations du VPN sont évidemment dépendantes de la solution choisie et des positions géographiques des serveurs. Mes tests s’effectuent à travers les serveurs de PrivateInternetAccess (ping ; download ; upload) :

ping    | download  | upload    | lieu                  | speedtest
---     | ---       | ---       | ---                   | ---
18 ms   | 3.813 Mo/s| 3.714 Mo/s| Toulouse, France      | ![image](http://www.speedtest.net/result/4195902546.png "Sans VPN")
31 ms   | 2.872 Mo/s| 2.792 Mo/s| Paris, France         | ![image](http://www.speedtest.net/result/4195924001.png "VPN Paris")
30 ms   | 0.608 Mo/s| 2.096 Mo/s| Amsterdam, Netherlands| ![image](http://www.speedtest.net/result/4195939338.png "VPN Netherlands")
170 ms  | 2.94 Mo/s | 0.94 Mo/s | San Jose, California  | ![image](http://www.speedtest.net/result/4195956371.png "Sans VPN California")
166 ms  | 0.928 Mo/s| 0.466 Mo/s| San Jose, California  | ![image](http://www.speedtest.net/result/4195934326.png "VPN California")
372 ms  | 1.93 Mo/s | 1.32 Mo/s | Sidney, Australia     | ![image](http://www.speedtest.net/result/4195950847.png "Sans VPN Australia")
350 ms  | 0.194 Mo/s| 0.078 Mo/s| Sidney, Australia     | ![image](http://www.speedtest.net/result/4195918955.png "VPN Australia")

etc…
