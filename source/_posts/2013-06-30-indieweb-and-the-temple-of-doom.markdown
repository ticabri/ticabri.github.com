---
layout: post
title: "IndieWeb and the Temple of Doom"
date: 2013-06-30 15:39
comments: true
categories: 
---

Hangouts Won’t Hangout With Other
---------------------------------

{% img left http://upload.wikimedia.org/wikipedia/commons/thumb/b/b0/Vittala_Temple's_Gopuram.JPG/320px-Vittala_Temple's_Gopuram.JPG Par Aravindreddy.d (Travail personnel) [CC-BY-SA-3.0], via Wikimedia Commons %}

Laurent Eschenauer revient sur les annonces de Google à la conférence annuel Google I/O : [la fin de XMPP chez Hangouts](http://eschnou.com/entry/whats-next-google--dropping-smtp-support--62-24930.html). Le nouveau produit de Google permettant de communiquer avec ses amis abandonne le support du protocole de messagerie instantané XMPP. XMPP faisait partie intégrante de Google Talk depuis plus de dix ans. XMPP permet l'envoi de messages instantanés entre clients desktop, comme Pidgin, et permet la communication entre les utilisateurs des différents réseaux de messagerie instantanée.

{% blockquote Unknown Lamer http://tech.slashdot.org/story/13/05/20/2315216/google-drops-xmpp-support Google Drops XMPP Support %}
Unfortunately, the new product drops support for the XMPP instant messaging protocol, which has been an integral part of Talk for over ten years. XMPP delivers instant messages to desktop clients, like Pidgin, and enables communication between users on different instant messaging networks.
{% endblockquote %}

Laurent Eschenauer se/nous demande quel est la prochaine étape de Google ? Supprimer le support de SMTP, le protocole des emails (qui permet de la même façon que XMPP de partager des emails à travers différents services reposant sur SMTP) ?

Il illustre son propos en rappelant [l'excellente illustration](http://aaronparecki.com/notes/2013/03/31/2/this-is-what-email-would-have-looked-like) de [@aaronpk](https://twitter.com/aaronpk). Et nous rappelle les solutions possibles pour éviter le pire et rester maitre de ses données et donc de l'Internet. Parmi celles-ci, je me permets d'insister sur IndieWeb.

{% img center http://aaronparecki.com/files/want-to-reply-join-gmail.png This is what email would have looked like if it were invented in the Web 2.0 era. Par Aaron Parecki %}

IndieWeb and the Last Crusade
-----------------------------

J'avais déjà entendu parler d'[IndieWebCamp](http://indiewebcamp.com/Main_Page) grâce [aux amis du Code And Coffee](https://twitter.com/AntoineCezar/status/347689992467922944). J'avais alors été voir le site et puis c'est tout. Maintenant que je suis mieux préparé, j'ai découvert un lien : Getting Started. On se sent moins perdu, moins idiot quand on a un lien Getting Started. Mais alors, de quoi ça cause ?

{% img center http://indiewebcamp.com/images/a/a6/indiewebcamp_logo.svg IndieWebCamp logo %}

### Première étape : un nom de domaine

IndieWeb recommande de se faire conseiller un registrar par un ami qui a confiance dans le sien. Je ne vais pas m'éterniser : [no bullshit avec gandi.net](https://www.gandi.net/). Je vous laisse découvrir pourquoi ils se labellisent dans le [no bullshit](https://www.gandi.net/no-bullshit).

Mais alors pourquoi faire un nom de domaine ?

### Possible étape : personnaliser ses services

Vous avez un compte blogger ? Un compte wordpress ? IndieWeb vous recommande de personnaliser les adresses à vos services avec votre nom de domaine tout neuf et surtout à vous. C'est ainsi que désormais vous pouvez retrouver ce blog sur le sous-domaine [blog.ticabri.com](http://blog.ticabri.com).

IndieWeb fait la distinction entre les redirections vers les [silo](http://indiewebcamp.com/silo) et les services hébergé. Un silo c'est facebook, google/google+, flickr, twitter. Un service hébergé c'est wordpress, blogger ou tumblr qui peuvent être mis en place pour servir votre domaine personnel pour vous. Autrement dit, avec un silo, vous proposez une redirection depuis [facebook.ticabri.com](http://facebook.ticabri.com) vers [facebook.com/ticabri](http://www.facebook.com/ticabri) et les visiteurs voient alors dans leur navigateur l'adresse du silo. Avec un service hébergé, vos visiteurs ont l'impression d'être chez vous, comme pour blogger.ticabri.com.

Évidemment vos contenus sont quand même hébergé chez un tiers qui peut à tout moment supprimer, perdre, effacer, utiliser vos données.

### Deuxième étape : héberger ses données

{% img right http://upload.wikimedia.org/wikipedia/commons/thumb/9/97/Toda_Hut.JPG/320px-Toda_Hut.JPG Par Pratheepps [CC-BY-SA-3.0], via Wikimedia Commons %}

Il est clair que vous n'avez pas les moyens de monter un serveur chez vous : non pas que ce soit trop cher, non pas que ce soit compliqué, mais si vous lisez ça, c'est que cette solution a déjà été un échec (probablement à cause de la maintenance) ou qu'elle ne vous est jamais venue à l'esprit.

Personnellement j'ai tenté l'expérience et c'est quand même pas si pratique que ça. Dans ce cas, dirigez vous vers un provider, un hébergeur. Gandi propose des forfaits d'hébergement, [AlwaysData](https://www.alwaysdata.com/) offre même un hébergement gratuit, pour les autres, je vous laisse faire vos recherches.

Une fois l'hébergeur sélectionné, le prix payé et les identifiants de connexion obtenus (control panel, ftp, sql), vous pouvez commencer à mettre en place l'ensemble des solutions proposées par IndieWeb dont la première, importante mais certainement pas finale : un fichier index.html avec votre hCard et les liens vers vos autres profils de réseaux sociaux.

Par la suite, vous transférerez tranquillement vos données vers [des services auto-hébergés](http://indiewebcamp.com/Projects), vous créerez votre propre raccourcisseur d'url, etc...

[Tous les détails sont fournis par IndieWeb](http://indiewebcamp.com/Getting_Started#Web_Hosting) et je ne manquerai pas de faire une petite traduction lorsque j'en serai moi-même à cette étape.
