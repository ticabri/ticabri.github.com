---
layout: post
title: "Start a Simple Web Server"
date: 2013-08-31 00:03
comments: true
categories: developpement
---

Je viens de découvrir qu'il était simplissime de démarrer un petit serveur web sous UNIX avec python.

```
$ cd MyWebSite
$ python -m SimpleHTTPServer 8000
Serving HTTP on 0.0.0.0 port 8000 ...

```

Il suffit de lancer cette ligne de commande dans le répertoire qui contient votre html/js/css et c'est tout. Je le note comme ça tout le monde pourra s'en rappeler, moi le premier.

source: http://lifehacker.com/start-a-simple-web-server-from-any-directory-on-your-ma-496425450