# Labo 3 - Load Balancing

> Auteurs: Gwendoline Dössegger, Noémie Plancherel, Gaby Roch

## Introduction

## Tâches

### 1 Installation des outils

Nous avons déjà installé `Docker` et `Docker-compose` avant le laboratoire. Nous devons uniquement installer `JMeter`.

Nous l'installons directement avec le paquet Debian:

```sh
sudo apt install jmeter 'jmeter-*'
```

Nous allons à présent créer les 3 containers à l'aide de la commande `docker-compose up` qui va se référer au `Dockerfile`

```sh
docker-compose build
# Nous avons dû désactiver un service car le port 80 était déjà occupé
docker-compose up
```

Nous pouvons à présent vérifier que les 3 containers tournent avec la commande:

```sh
docker ps
```

Nous constatons q'il y a un réseau virtuel qui a été créé pour le labo 3 avec la commande:

```sh
docker network ls
```

Une fois toute la mise en place faite, nous pouvons nous rendre sur le load balancer via l'adresse `http://192.168.42.42`.

Nous constatons que le `NODESESSID` est bien envoyé à notre navigateur:

#### 1.1

cookie envoyé à chaque fois

#### 1.2

#### 1.3

#### 1.4

#### 1.5

### 2 La persistence des sessions

#### 2.1 

#### 2.2

#### 2.3

#### 2.4

#### 2.5

#### 2.6

### 3 Le drainage des connexions

### 4 Le mode dégradé avec Round Robin

### 5 Les stratégies de load balancing

## Conclusion

## Annexes

