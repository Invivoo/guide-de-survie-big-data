# Comprendre les limites des SGBDR

Si SGBDR OK, on reste sur du SGBDR

# Quand lâcher les systèmes SGBDR (à éditer)

- les coûts de la montée en charge verticale
- la montée en charge horizontale limitée à 10 nœuds, pour des contraintes techniques
- les coûts en ressources humaines pour mettre en place un tel matériel et assurer son bon fonctionnement, ce qui implique plus de coûts pour héberger plus de données
- les bases de données relationnelles ne sont pas adaptées pour les traitements temps réel
- les prix des licences de logiciels comme Oracle s'ajoutant au prix des machines spécifiques

# Alternatives aux systèmes SGBDR, NoSQL

## CAP Theorem

- Cohérence
- Disponibilité
- Tolérance au Partitionnement

## Différente approche au stockage

### Clef / Valeur

- Voldemort
- Riak
- DynamoDB
- memcached
- Redis
- OrientDB

### Orienté document

- MongoDB
- Elasticsearch
- CouchDB
- RavenDB
- OrientDB
- DocumentDB 

### Orienté colonnes

- Cassandra
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

#### Hortonworks

#### MapR

#### Cloudera

### Retour d'expérience sur Hadoop

- Criteo et leurs cluster
