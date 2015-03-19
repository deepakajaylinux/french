===================
Amazon ElastiCache
===================

synopsis
-------------

ElastiCache est un service web qui le rend facile à déployer, exploiter et l'évolution d'un cache en mémoire dans le nuage. Le service améliore les performances des applications web en vous permettant d'extraire des informations de caches rapides, gérés en mémoire, au lieu de compter entièrement sur les bases de données sur disque plus lents. ElastiCache prend en charge les deux moteurs de mise en cache en mémoire open 
source :


Memcached - un objet de mémoire largement adopté système de cache. ElastiCache est compatible avec Memcached, le protocole et populaires outils que vous utilisez aujourd'hui avec les environnements existants de Memcached ne peut fonctionner en toute transparence avec le service.


Redis – une boutique populaire open source clé-valeur en mémoire qui prend en charge les ensembles de structures telles que le tri de données et listes. ElastiCache prend en charge maître / esclave de réplication et Multi-AZ, qui peut être utilisé pour obtenir une redondance AZ croisée.


Amazon ElastiCache détecte automatiquement et remplace les nœuds ayant échouées, réduisant le frais généraux afférents aux infrastructures autogérées et fournit un système résilient qui atténue le risque de bases de données surchargées, quel site lent et demande les temps de chargement. Grâce à l'intégration avec Amazon CloudWatch, Amazon ElastiCache fournit une visibilité accrue dans les principaux indicateurs de performance associés à vos nœuds Memcached ou Redis.


À l'aide d'Amazon ElastiCache, vous pouvez ajouter une couche de mise en cache en mémoire à votre infrastructure en quelques minutes en utilisant l'AWS Management Console.



Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de ElastiCache Amazon. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSElastiCache help

 ******************************


    This is an extension provided for Handling AWS ElastiCache.

    AWSElastiCache, awselasticache, aws-elasticache

        - create-cache-cluster
        Lets you add cache Cluster to AWS ElastiCache
        example: ptconfigure AWSElastiCache create-cache-cluster
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess

          - reboot-cache-cluster
        Lets you reboot cache Cluster to AWS ElastiCache
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess

         - delete-cache-cluster
        Lets you delete cache Cluster to AWS ElastiCache
        example: ptconfigure AWSElastiCache delete-cache-cluster
                    --yes
                    --guess

         - delete-replication-group
        Lets you delete replication group to AWS ElastiCache
        example: ptconfigure AWSElastiCache delete-replication-group
                    --yes
                    --guess

        - list
        Will display data about your AWS ElastiCache
        example: ptconfigure AWSElastiCache list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Create-cache-cluster 
---------------------------

Cette commande permet d'ajouter le cache Cluster à AWS ElastiCache. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash

	ptconfigure AWSElastiCache create-cache-cluster –yes --guess 


Create-health-check 
---------------------------

Cette commande permet d'ajouter le bilan de santé à AWS Route53. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check –yes –guess

Reboot-cache-cluster 
---------------------------

Cette commande permet de redémarrer le cache Cluster à AWS ElastiCache.

 
.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 


Delete-cache-cluster 
-------------------------

Cette commande permet de supprimer le cache de Cluster à AWS ElastiCache. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash     
	
	ptconfigure AWSElastiCache delete-cache-cluster --yes --guess


Delete-replication-group 
-----------------------------------

Cette commande permet de supprimer le groupe de réplication à AWS ElastiCache. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash 
	
	ptconfigure AWSElastiCache delete-replication-group --yes --guess
        
List
---------------------

Cette commande permet d'afficher les données affichées sur votre ElastiCache AWS. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash 

	ptconfigure AWSElastiCache list --yes --guess

Alternative Paramètre
------------------------------       

Il y a trois paramètres de substitution qui peuvent être utilisés en ligne de commande.


AWSElastiCache, awselasticache, aws-elasticache 

avantages
--------------

Simple à déployer : Amazon ElastiCache, il est très facile de déployer un environnement compatible avec cache Memcached ou Redis. Utiliser l'AWS Management Console ou les appels d'API simples pour accéder les fonctionnalités d'un cluster de production-ready nuage cache en quelques minutes sans se soucier d'infrastructure mise en service, ou installation et maintenance de logiciels de cache.


Réussi : Amazon ElastiCache automatise les tâches de gestion de temps--tels que la gestion des correctifs, détection des pannes et récupération--vous permettant de poursuivre le développement d'applications valeur plus élevée.

Compatible : Avec Amazon ElastiCache, vous obtenez un accès natif aux environnements cache Memcached ou Redis en mémoire. Ceci facilite la compatibilité avec vos outils existants et des applications.


Élastique : Avec un simple appel d'API ou quelques clics de l'AWS Management Console, vous pouvez ajouter ou supprimer des nœuds de Cache sur votre cluster de cache de nuage pour répondre à la charge de l'application. La découverte automatique pour Memcached détecte automatiquement des nœuds de Cache par les Clients de ElastiCache quand les nœuds sont ajoutés ou supprimés du ElastiCache Cluster Amazon.



Fiable : Amazon ElastiCache a plusieurs fonctions qui améliorent la fiabilité pour les déploiements de production critiques, y compris la récupération et la détection automatique de panne. Amazon ElastiCache fonctionne sur la même infrastructure hautement fiable utilisée par d'autres Services de Web d'Amazone.

Intégrée : Amazon ElastiCache est conçu pour une utilisation transparente avec d'autres Amazon Web Services, y compris Amazon Relational Database Service (Amazon RDS), DynamoDB de Amazon, Amazon Elastic Compute Cloud (Amazon EC2), Amazon CloudWatch et Amazon Simple Notification Service (Amazon SNS).

Sécurisé : Amazon ElastiCache fournit un certain nombre de mécanismes pour garantir votre Cluster de Cache.

Amazon ElastiCache fournit des interfaces de services web qui vous permettent de configurer les paramètres de pare-feu qui contrôlent l'accès au réseau sur votre Cluster de Cache.


Amazon ElastiCache vous permet d'exécuter votre Cluster de Cache dans Amazon Virtual Private Cloud (Amazon VPC). Amazon VPC vous permet d'isoler votre Cluster de Cache en spécifiant les plages d'IP que vous souhaitez utiliser pour vos noeuds de Cache et vous connecter à vos applications existantes à l'intérieur d'Amazon VPC. Pour en savoir plus sur Amazon ElastiCache en VPC, reportez-vous au Guide d'utilisation ElastiCache Amazon.




Rentable : Amazon ElastiCache vous permet d'économiser le coût administratif de mise en place et gérer un Cluster de nœuds multiples Cache. Vous pouvez intensifier et à réduire le nombre de nœuds de Cache dans votre Cluster de Cache pour offrir des performances optimales que votre utilisation de l'application des changements de modèle, en payant uniquement pour les ressources que vous consommez réellement. La tarification à la demande vous permet de payer pour la capacité de mémoire/calcul de l'heure avec aucun engagement à long terme. Cela rend l'utilisation de ElastiCache Amazon très rentable et vous évite les coûts et la complexité de la planification, d'achat et entretien matériel.


Multi-AZ: Amazon ElastiCache fournit des fonctionnalités de réplication pour le Redis moteur et de la fonctionnalité Multi-AZ. Vous pouvez profiter de multiples Zones de disponibilité AWS gagner la disponibilité et l'évolution au-delà des contraintes de capacité d'un nœud de cache unique. En cas de perte du nœud principal, ElastiCache détecte automatiquement l'échec et le basculement vers une réplique de lecture afin de fournir une plus grande disponibilité sans la nécessité d'une intervention manuelle.



Sauvegarde et restauration : ElastiCache Amazon pour Redis vous aide à protéger vos données en créant des instantanés de vos clusters. Via quelques clics sur la console ou les appels d'API simples, vous pouvez mis en place des snapshots automatiques, ainsi que de lancer une sauvegarde chaque fois que vous choisissez. Les captures instantanées peuvent alors servir pour l'ensemencement de nouveaux ElastiCache pour les clusters Redis.




Principaux cas d'utilisation : Amazon ElastiCache permet d'améliorer considérablement les temps de latence et le débit pour beaucoup de charges de travail application de lecture importante (tels que les réseaux sociaux, jeux, partage de médias et portails Q&A) ou de charges de calcul intensif (par exemple, un moteur de recommandation). Mise en cache améliore les performances des applications en stockant les éléments critiques de données en mémoire pour un accès faible latence. Informations mises en cache peuvent inclure les résultats des requêtes de base de données e/S intensives ou les résultats des calculs de forte intensité de ressources informatiques. Les applications qui ont besoin d'un serveur de structure de données, trouverez le moteur Redis plus utiles.

