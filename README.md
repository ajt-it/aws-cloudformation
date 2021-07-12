![Apache 2.0](https://img.shields.io/badge/apache-2.0-orange)


# aws-cloudformation

Administration d'une infrastructure cloud (AWS) grâce à l'automatisation de la création de l’ensemble des ressources via un stack de CloudFomation. 


## Représentation de l'infrastructure

![Infra (cloud_aws) - p10aic - wordpress](https://user-images.githubusercontent.com/46109209/125218939-80a12580-e2b3-11eb-9156-36740de4ee7b.png)


## Langage

 - :white_check_mark: YAML


## Pré-requis
Vous aurez besoin d'un compte AWS : https://aws.amazon.com/fr/


## Objectifs

À l'aide d'un template (script) '.yml'; mettre en place d'un serveur WordPress sur AWS en utilisant :
  - RDS pour le stockage de la base de données
  - S3 pour le stockage des médias (via le plugin amazon-web-services)
  - EC2 et Docker pour le serveur web
  - ELB pour distribuer les requêtes sur les instances EC2
  - CloudFormation pour automatiser la création de l’infrastructure

Tous les éléments de l'infrastructure publique sont répartis sur plusieurs zones de disponibilité (multi-AZ). La répartition des requêtes vers les différentes zones de disponibilité (AZ) est effectuée avec ELB (Elastic Load Balancer).
