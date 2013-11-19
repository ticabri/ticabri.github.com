---
layout: post
title: "Utiliser Git pour deployer votre site web"
date: 2013-09-27 13:51
comments: true
categories: developpement
---

Git est désormais essentiel pour tout développement, y compris pour les sites web.

Pour ce genre de développement web, j'ai mis en place la configuration suivante :

- mes outils de développement sur ma machine physique.
- un hébergement chez gandi qui autorise la publication via git et ssh.
- une machine virtuelle avec LAMP pour le serveur de développement, test ou pré-prod.

L'idée ici est d'utiliser git pour _pusher_ le site vers les serveurs que ce soit celui de production chez gandi.net ou que ce soit celui de dev sur la machine virtuelle.

[Abhijit Menon-Sen](http://toroid.org/ams) nous explique comment faire dans [un article en anglais](http://toroid.org/ams/git-website-howto).

Les étapes sont assez simples :

- autoriser la connexion ssh entre la machine _host_ et la _guest_ (i.e. la machine virtuelle) ;
- configurer un repository ```--bare``` sur la machine _guest_ ;
- configurer un [hook git](http://git-scm.com/book/en/Customizing-Git-Git-Hooks)
- ajouter un _remote_ pour pouvoir _pusher_

Ensuite un simple ```git push web``` et c'est déployer.