![Apache 2.0](https://img.shields.io/badge/apache-2.0-orange)


# AWS-Infrastructure as Code (IaC)

Administration d'une infrastructure cloud (AWS) grâce à l'automatisation de la création de l’ensemble des ressources via un stack CloudFormation.

Souvent plébiscité dans le cadre du cloud computing, l'infrastructure as code offre aux développeurs 
la possibilité d'automatiser leurs déploiements de manière à éviter les tâches manuelles ou encore de 
devoir écrire d'eux-mêmes les appels aux interfaces de programmation. 
Cette technologie constitue une réponse aux besoins des entreprises en termes de mise à l'échelle des 
applications axée sur l'automatisation et la simplification de l'infrastructure de projets informatiques. 


## Représentation de l'infrastructure

![Infra - p10aic - wordpress](https://user-images.githubusercontent.com/46109209/128689693-04376346-147a-40f9-93e9-b8e874b1b371.png)

## Langage

 - :white_check_mark: YAML


## Pré-requis
Vous aurez besoin d'un compte AWS : https://aws.amazon.com/fr/


## Objectifs

À l'aide d'un template (.yaml) mettre en place d'un serveur WordPress sur AWS en utilisant :
  - RDS pour le stockage de la base de données
  - S3 pour le stockage des médias (via le plugin amazon-web-services)
  - EC2 et Docker pour le serveur web
  - ELB pour distribuer les requêtes sur les instances EC2
  - CloudFormation pour automatiser la création de l’infrastructure

Tous les éléments de l'infrastructure publique sont répartis sur plusieurs zones de disponibilité (multi-AZ). La répartition des requêtes vers les différentes zones de disponibilité (AZ) est effectuée avec ELB (Elastic Load Balancer).
