---
layout: post
title: "Docker: quelques astuces"
date: 2015-03-15 13:32:58 +0100
comments: true
categories:
published: false
---

J'ai un peu joué avec docker via boot2docker et voilà mes quelques astuces pour se créer sa flotte de serveur, machine, environnements différents.

# Comprendre boot2docker

C'est une petite VM ubuntu permettant de faire tourner docker. Les commandes utiles de boot2docker :

```
# set env variables to use docker
$(boot2docker shellinit)

# curl a docker port
curl -i $(boot2docker ip):<port>
```

# Créer son cloud

[…]

# Des commandes Docker sympas

## Faire le ménage

```
# supprimer tous les containers
docker rm $(docker ps -q -a)

# supprimer les containers stoppés
docker rm $(docker ps -q -a -f status=exited)

# supprimer les images temporaires
docker rmi $(docker images -q -a -f dangling=true)
```

## Ça tourne

Lancer un serveur nginx standard – depuis le _public registry_ de Docker.

```
docker run -p 8080:80 -d --name nginx nginx
docker port nginx
boot2docker ip
curl -i $(boot2docker ip):8080
docker stop nginx
curl -i $(boot2docker ip):8080 # curl: (7) Failed to connect to 192.168.59.103 port 8080: Connection refused
docker ps
docker ps -a | grep nginx
docker start nginx
docker ps
```
