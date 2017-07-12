# Guide de survie du Big Data

1. [Comprendre les limites des SGBDR](#comprendre-les-limites-des-sgbdr)
1. [Quand passer du SGBDR à un système NoSQL](#quand-passer-du-sgbdr-à-un-système-nosql)
1. [Systèmes NoSQL](#systèmes-nosql)
    1. [Théorème du CAP](#théorème-du-cap)
    1. [Différentes approches à la persistance](#différentes-approches-à-la-persistance)
1. [Paradigmes du Big Data](#paradigmes-du-big-data)
1. [Architectures](#architectures)
1. [Solutions Hadoop](#solutions-hadoop)
1. [Visualisation et exploration de la data](#visualisation-et-exploration-de-la-data)
1. [Contribuer à ce guide](#contribuer-à-ce-guide)

# Comprendre les limites des SGBDR

TODO

# Quand passer du SGBDR à un système NoSQL


- les coûts de la montée en charge verticale
- la montée en charge horizontale limitée à 10 nœuds, pour des contraintes techniques
- les coûts en ressources humaines pour mettre en place un tel matériel et assurer son bon fonctionnement, ce qui implique plus de coûts pour héberger plus de données
- les bases de données relationnelles ne sont pas adaptées pour les traitements temps réel
- les prix des licences de logiciels comme Oracle s'ajoutant au prix des machines spécifiques

# Systèmes NoSQL

## Théorème du CAP

- Cohérence
- Disponibilité
- Tolérance au Partitionnement

## Différentes approches à la persistance

### Clef / Valeur

- Voldemort
- Riak
- DynamoDB
- memcached
- Redis
- OrientDB

### Orienté document

- MongoDB
- [Elasticsearch](storage/elasticsearch.md)
- CouchDB
- RavenDB
- OrientDB
- DocumentDB 

### Orienté colonnes

- [Cassandra](storage/cassandra.md)
- HBase

### Graph

- neo4j

### Timeseries

- Druid

###  Grille de comparaisons des différent sysyèmes de stockage par rapport au CAP

TODO

# Paradigmes du Big Data

## MapReduce

Inspiré de la programmation fonctionnelle. 
Séparation des données et des traitements

Référence : https://blog.matthewrathbone.com/2013/04/17/what-is-hadoop.html

## Traitements en batch

- Job MapReduce Hadoop

## Traitements temps réels

- Spark
- Storm

# Architectures

## Architecture Lambda

## Architecture Kappa

# Solutions Hadoop

## Hadoop

### HDFS

#### Objectifs

- tolérant aux pannes 
- scalable
- modèle d'accès immuable 
- Déplacer les calculs vers les données
- simple à mettre en place 

#### Features

- gestion des fichiers par blocs
- réplication et distribution
- gestion des droits
- accès aux données en continu 
- stockage des grands jeux de données

#### API

- Bash
- Librairies pour chaque langages.
- Rest avec HttpFS et WebHDFS

### HBase

### Hive

### Pig

### Zookeeper

### Sqoop

### Oozie

### Flume

### Kafka

### Spark

### Distributions Hadoop

TODO

#### Hortonworks

TODO

#### MapR

TODO

#### Cloudera

TODO

### Retours d'expérience sur Hadoop

TODO

# Visualisation et exploration de la data

* [Tableau](https://www.tableau.com/)
* [Trifacta Wrangler](https://www.trifacta.com)

# Contribuer à ce guide

Ce guide est rédigé au format [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). N'hésiter pas à le corriger / complémenter par Pull Request.
