---
layout: post
title: "Comment prédire le futur de la programmation"
date: 2015-07-31 16:48:15 +0200
comments: true
categories: [développement]
---

_Cet article est une traduction de l'article de [Justin Weiss](https://twitter.com/justinweiss), [How to predict the future of programming](http://www.justinweiss.com/blog/2015/07/28/how-to-predict-the-future-of-programming/) publié sur son blog le 28 juillet 2015. [J'attends son approbation](https://twitter.com/ticabri/status/626668884343566336)_

---

Pourquoi Rails est devenu si populaire, si vite ?

Sa simplicité a aidé, particulièrement si vous venez du java, du XML, du monde
de l'entreprise. [Il a aussi été parfaitement vendu](https://www.youtube.com/watch?v=Gzj723LkRJY). Mais ça n'est pas tout.

**Une grosse partie du succès de Rails dans le monde des startups vient d'un simple fait : les problèmes que rencontrent les entreprises ne sont pas uniques**. Rails était très efficace pour créer des sites [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete), tout en restant flexible. Et c'est là un des besoins les plus rencontrés par les entreprises. Surtout au début.

Mais ce n'est pas vrai seulement pour les entreprises. **Beaucoup de problèmes que nous rencontrons en tant que développeurs de logiciel ne changent pas**.
Bien sûr les solutions évoluent. Elles bouclent. Nous nous améliorons.
Mais les mêmes solutions découvertes par la dernière génération de
développeurs peuvent toujours nous aider aujourd'hui.

Donc, voulez-vous savoir les réponses aux problèmes que vous rencontrerez
dans le futur ? La meilleure chose que vous pouvez faire est de regarder
dans le passé.

## Regardez dans le passé

**Sur [son site web](http://martinfowler.com/), Martin Fowler a une incroyable collection de bonnes solutions à des problèmes communs**. Avez-vous [écouté
des présentations de dévs au sujet de l'event sourcing](http://blog.arkency.com/2015/03/fast-introduction-to-event-sourcing-for-ruby-programmers/) ?
Il a écrit [l'article parfait](http://www.martinfowler.com/eaaDev/EventSourcing.html) à ce sujet il y a 10 ans. Chasser les problèmes de performance et de
fiabilité avec votre nouvelle API REST ou votre [architecture orientée service](https://en.wikipedia.org/wiki/Service-oriented_architecture) ?
C'est [sa première loi des objets distribués](http://www.drdobbs.com/errant-architectures/184414966), qui a environ 15 ans.

[Avdi Grimm](http://avdi.org/) me disait que "si tu veux mener la courbe de la technologie,
commence par enquêter sur ce que Martin Fowler a écrit il y a une décennie."
Et c'est tout à fait vrai. **Le temps que vous passez [sur son site](http://martinfowler.com/) à lire les articles au sujet des procédés (NDT : 'patterns' dans le texte) est un très bon investissement pour vos futurs développement**. Et sans même parler [des techniques de refactoring](http://refactoring.com/catalog/).

Pour aller plus loin, n'importe quel livre ou article écrit
par [les auteurs du Manifeste Agile](http://www.agilemanifesto.org/) vaut le coup d'être lu -- il y a 15 ans, ils
rencontraient les mêmes problèmes d'architecture que nous rencontrons
aujourd'hui.

**Vous pouvez trouver tout un tas de discussions sur le [wiki de C2](http://www.c2.com/cgi/wiki)**. Les débats que nous avons pour savoir [quand faire du TDD est le plus sensé](http://www.c2.com/cgi/wiki?TestDrivenDevelopment) ? Ils sont tous là. Et l'ont toujours été. Ce wiki est là depuis longtemps, et c'est toujours une ressource fantastique.

Les livres de la fin des années 90 au début des années 2000 sont aussi utiles.Je souriais continuellement avec [Smalltalk Best Practice Patterns](http://www.amazon.com/Smalltalk-Best-Practice-Patterns-Kent/dp/013476904X) et [Patterns of Enterprise Application Architecture](http://www.amazon.com/Patterns-Enterprise-Application-Architecture-Martin/dp/0321127420) (qui a été une grosse influence pour Rails), car ils décrivaient des problèmes que j'avais _si souvent_.

Comme la mode, les pratiques de développement logiciel bouclent. De distribué à centralisé, de côté client à côté serveur, de dynamique à statique.

Voulez-vous être en avance, comprendre ce qui va venir, et peut-être même être à l'initiative de ce qui viendra ensuite ? Regardez dans le passé. **Recherchez les solutions aux problèmes que les solutions actuelles causeront**. Et aider à divulguer les bonnes pratiques de l'ancienne génération des développeurs logiciel à la suivante.
