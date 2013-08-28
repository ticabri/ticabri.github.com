---
layout: post
title: "Zombie Ninjas Attack: A survivor's retrospective"
date: 2013-05-28 21:03
comments: true
categories: blog
---

ticablog tente une migration sur octopress, un framework pour Jekyll (le générateur de blog pour github). Les premiers pas sont assez faciles à faire tant la documentation est claire et précise.

Pourquoi ce titre ?!
--------------------

C'est l'exemple donné dans la documentation pour créer un nouveau billet. Le billet est généré par une ligne de commande :

```
rake new_post["Zombie Ninjas Attack: A survivor's retrospective"]
```

Il suffit ensuite d'écrire son billet en respectant la syntaxe markdown (ou une autre si ça vous chante). Dans le fichier, une petite configuration Yaml permet de définir les quelques meta information du billet : titre, date, catégories, etc.

{% img left http://www.octopress.org/images/logo.png %}

Le billet est écrit, il ne reste plus qu'à générer le code html avec un `rake generate` puis un `rake deploy` pour déployer le blog sur github.

Bref, c'est vraiment sympa comme façon d'écrire, j'utilise les mêmes outils que pour travailler et c'est vraiment très rapide. On verra plus tard pour la customisation et l'utilisation plus avancée des outils.

Je ne ferai pas la migration des billets de http://ticabri.blogspot.fr vers octopress tout de suite. Il sera toujours temps plus tard, quand j'aurai trouvé une méthode raisonnable.