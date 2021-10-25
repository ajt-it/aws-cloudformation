![Apache 2.0](https://img.shields.io/badge/apache-2.0-orange) ![Licence GPL-3.0](https://img.shields.io/badge/Licence-GPL_3.0-red)


# AWS-Infrastructure as Code (IaC)

Administration d'une infrastructure cloud (AWS) grâce à l'automatisation de la création de l’ensemble des ressources via un stack CloudFormation.

Souvent plébiscité dans le cadre du cloud computing, l'infrastructure as code offre aux développeurs 
la possibilité d'automatiser leurs déploiements de manière à éviter les tâches manuelles ou encore de 
devoir écrire d'eux-mêmes les appels aux interfaces de programmation. 
Cette technologie constitue une réponse aux besoins des entreprises en termes de mise à l'échelle des 
applications axée sur l'automatisation et la simplification de l'infrastructure de projets informatiques. 


## Représentation de l'infrastructure

![infra aws](https://user-images.githubusercontent.com/46109209/138763086-9d9c4728-3328-4256-9fcd-4514f5f09009.png)


## Langages


 - :white_check_mark: YAML

 - :white_check_mark: SHELL


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

Mettre en place une liaison VPN entre un serveur VPN local et le sous-réseau privé AWS via une instance EC2.

La mise en place de l’auto-scaling sur les instances EC2 permettra d'augmenter le nombre de machines dès que la charge CPU des serveurs atteint 80% en moyenne sur 5 minutes et une alerte par email est envoyée à chaque fois que l'événement survient.


## Technologies

Liste des technologies AWS utilisées :

- aws CloudFormation
- aws EC2
- aws RDS
- aws S3
- aws Simple Notification Service
- aws VPC
- aws CloudWatch
- Docker
- Wordpress
- Amazon Linux 2 OS


## Ressources

- https://docs.aws.amazon.com/
- https://docs.docker.com/
- https://deliciousbrains.com/wp-offload-media/
- https://wp-cli.org/fr/
- https://www.google.com/

