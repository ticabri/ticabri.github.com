---
layout: post
title: "Déployer son site octopress depuis une nouvelle machine"
date: 2014-06-09 13:16
comments: true
categories: [blog, développement]
---

[Ce blog tourne avec Octopress](http://blog.ticabri.com/blog/2013/05/28/zombie-ninjas-attack-a-survivors-retrospective/), un framework pour Jekyll et la mise en ligne d'un nouveau contenu se fait [grâce à Git](http://blog.ticabri.com/blog/2013/09/27/utiliser-git-pour-deployer-votre-site-web/).

Pour autant la stratégie de déploiement des sources de la branche `source` vers la branche `master` du repo github utilise un répertoire dans `source` nommé `_deploy` dans lequel est stocké tout ce qui va être pushé sur la branche`master`. Et si vous utilisez plusieurs machines, cela peut vite devenir un cass-tête.

La marche à suivre est pourant simple. Sur la nouvelle machine :

* récupérez les sources ;
```
git clone -b source git@github.com:username/username.github.com.git octopress
```
* récupérez l'état à jour de `_deploy` ;
```
git clone git@github.com:username/username.github.com.git _deploy
```
* _faites vos modifications_
* faites un `rake generate` pour mettre à jour `_deploy` ;
* pushez vos modifications sur la branche `source` de github ;
* faites un `rake deploy` pour envoyer tout ça sur la branche master de github.

Toutes ces infos viennent du billet de blog de [0# (zerosharp)](http://blog.zerosharp.com/clone-your-octopress-to-blog-from-two-places/).