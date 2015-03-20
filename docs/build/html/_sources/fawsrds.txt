=================
AWS RDS 
=================

Synopsis
-------------

Amazon Relational Database Service (Amazon RDS) est un service web qui le rend facile à installer, exploiter et adapte à une base de données relationnelle dans le nuage. Il offre une capacité redimensionnable et rentable tout en gérant les tâches de gestion de temps de base de données, libérant ainsi de vous consacrer à vos applications et vos affaires.

Amazon RDS vous donne accès en ligne aux fonctionnalités d'un système de gestion de base de données relationnelle MySQL, Oracle, Microsoft SQL Server, PostgreSQL ou Amazon Aurora. Cela signifie que le code, les applications et outils que vous utilisez déjà aujourd'hui avec vos bases de données existantes peuvent être utilisés avec Amazon RDS. Amazon RDS automatiquement les correctifs du logiciel de base de données et de sauvegarde de votre base de données, stocker les sauvegardes pendant une période de rétention définie par l'utilisateur et permettant la récupération point-à-temps. Vous bénéficiez de la flexibilité de pouvoir faire évoluer les ressources de calcul ou de la capacité de stockage associé à votre Instance de base de données (Instance DB) via un seul appel d'API.

Instances de base de données à l'aide de MySQL, Oracle, SQL Server et PostgreSQL moteurs de Amazon RDS peuvent être configurées avec le but général (SSD) stockage, stockage provisionné Ops ES/s (SSD) ou de stockage magnétique. Instances de base de données en utilisant le moteur de Amazon Aurora emploient une tolérance de pannes, couche de stockage virtualisé adossés à des SSD spécialement conçu pour des charges de base de données d'auto-guérison.

De plus, Amazon RDS facilite la réplication facile à utiliser pour améliorer la disponibilité et la fiabilité pour des charges de production. À l'aide de l'option de déploiement Multi-AZ vous pouvez exécuter la mission de charges de travail stratégiques avec haute disponibilité et intégré automatisé basculement de votre base de données primaire pour une base de données secondaire répliquée de manière synchrone en cas de panne. À l'aide de réplicas de lecture, Amazon RDS pour MySQL, PostgreSQL et Amazon Aurora vous permettent également d'évoluer au-delà de la capacité d'un déploiement de base de données unique pour des charges de lecture importante base de données. Comme avec tous les Services Web Amazon, il n'y a aucun investissement initial requis, et vous ne payez que pour les ressources que vous utilisez.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'Amazon RDS. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.

.. code-block:: bash
 
 kevel@corp:/# ptconfigure Amazon RDS help

 ******************************


    This is an extension provided for Handling AWS ElastiCache.

    Amazon RDS, Amazon RDS, aws-elasticache

        - create-cache-cluster
        Lets you add cache Cluster to AWS ElastiCache
        example: ptconfigure Amazon RDS create-cache-cluster
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
        example: ptconfigure Amazon RDS delete-cache-cluster
                    --yes
                    --guess

         - delete-replication-group
        Lets you delete replication group to AWS ElastiCache
        example: ptconfigure Amazon RDS delete-replication-group
                    --yes
                    --guess

        - list
        Will display data about your AWS ElastiCache
        example: ptconfigure Amazon RDS list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Describe-instance 
---------------------------

Cette commande permet de décrire l'instance de AWS RDS. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash

	ptconfigure AWSRDS describe-instance --yes --guess 


Delete-instance 
---------------------------

Cette commande permet de supprimer l'instance. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash
	
	ptconfigure AWSRDS delete-instance --yes --guess

Create-db-snapshot 
---------------------------

Cette aide de la commande pour redémarrer crée db instantané. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash     

	ptconfigure AWSRDS create-db-snapshot --yes --guess 

Delete-db-snapshot 
-------------------------

Cette commande est utile pour enlever la copie instantanée db. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash     
	
	ptconfigure AWSRDS delete-db-snapshot –yes –guess


Copy-db-snapshot 
-----------------------------------

Cette commande permet de copier la copie instantanée db. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash 
	
	ptconfigure AWSRDS copy-db-snapshot --yes --guess
        
Create-instance
------------------------

Cette commande permet de créer l'instance. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash 

	ptconfigure AWSRDS create-instance --yes –guess

Reboot-instance
------------------------

Cette commande permet de redémarrer l'instance. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash 

	ptconfigure AWSRDS reboot-instance --yes --guess

Create-instance-read replica
--------------------------------------

Cette commande permet de créer instance db lu réplique. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash 

	ptconfigure AWSRDS create-instance-readreplica --yes --guess

List
---------

Cette commande permet d'afficher des données sur votre RDS de AWS. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash 

	ptconfigure AWSRDS list --yes --guess

Alternative Parameter 
------------------------------

Il y a trois paramètres de substitution qui peuvent être utilisés en ligne de commande.

AWSRDS, awsrds, aws-rds 

avantages
--------------

Simple à déployer le Service Web de base de données : Amazon RDS, il est facile aller de la conception de projet de déploiement. Utiliser l'AWS Management Console ou les appels d'API simples pour accéder les fonctionnalités d'une base de données relationnelle prêts pour la production en quelques minutes sans se soucier de la fourniture d'infrastructures ou de l'installation et maintenance logiciels de base de données.

Réussi : Amazon RDS gère des tâches de gestion des temps de base de données, telles que les sauvegardes, gestion des correctifs et la réplication, vous permettant de poursuivre le développement d'application valeur supérieur ou les raffinements de la base de données.

Compatible : Avec Amazon RDS, vous obtenez un accès natif à un système de gestion de base de données relationnelle. Ceci facilite la compatibilité avec vos outils existants et des applications. De plus, Amazon RDS vous donne contrôle facultatif qui appuie les pouvoirs version moteur votre Instance DB via la gestion de Version pour le moteur DB.

Rapide, des performances prévisibles : Instances de base de données en utilisant MySQL de Amazon RDS, Oracle, SQL Server et Oracle moteurs peuvent être fournis avec le but général (SSD) stockage, stockage provisionné Ops ES/s (SSD) ou de stockage magnétique.

Stockage Amazon RDS générales but (SSD) offre une base cohérente de 3 entrées/sorties par GB provisionné et offre la possibilité d'éclater jusqu'à 3 000 IOPS.

Stockage Amazon RDS provisionné Ops ES/s (SSD) est une option de stockage de haute performance conçue pour offrir des performances rapide, prévisible et cohérente pour des charges de base de données transactionnelle intensif de I/O. Vous pouvez approvisionner des Ops ES/s de 1 000 à 30 000 entrées/sorties par Instance DB. (Maximum réalisé QU'IOPS variera selon le type de moteur.)

Stockage magnétique (anciennement stockage Amazon RDS Standard) est utile pour des charges de la petite base de données où les données sont moins fréquemment accédées.

Instances de base de données en utilisant le moteur de Amazon Aurora emploient une tolérance de pannes, couche de stockage virtualisé adossés à des SSD spécialement conçu pour des charges de base de données d'auto-guérison.

Base de données évolutive dans le Cloud : vous pouvez faire évoluer le calcul et des ressources de stockage disponibles à votre base de données pour répondre à votre application a besoin à l'aide de l'API d'Amazon RDS ou l'AWS Management Console. Si vous utilisez le stockage Amazon RDS provisionné IOPS avec Amazon RDS pour MySQL, Oracle ou PostgreSQL, vous pouvez provisionner et adapte le stockage jusqu'à 3 to et le IOPS à jusqu'à 30 000. Notez ce maximum réalisé QU'IOPS variera selon le type de moteur. En outre, pour les moteurs de base de données MySQL, PostgreSQL et Aurora Amazon, vous pouvez également associer un ou plusieurs réplicas de lecture avec votre déploiement d'instance de base de données, vous permettant d'évoluer au-delà de la capacité d'une instance de base de données unique pour des charges de lecture importante.

Le moteur de base de données Amazon Aurora vous permet de faire évoluer votre espace de stockage jusqu'à 64 to. Vous pouvez associer jusqu'à 15 Amazon Aurora répliques à votre déploiement d'instance de base de données. Amazon Aurora répliques partagent le même stockage sous-jacent que l'instance de source, réduisant les coûts et en évitant de copier des données sur les nœuds de la réplique.

Fiable : Amazon RDS a plusieurs fonctions qui améliorent la fiabilité des bases de données de production critiques, y compris les sauvegardes automatiques, copies instantanées DB, remplacement automatique hôte et déploiements Multi-AZ. Amazon RDS s'exécute sur la même infrastructure hautement fiable utilisée par d'autres Services de Web d'Amazone.

Pour le moteur Aurora Amazon, Amazon RDS utilise la technologie RDS Multi-AZ pour automatiser le basculement vers un des 15 répliques Aurora vous avez créé dans l'une des trois Zones de disponibilité.

Conçu pour être utilisé avec d'autres Services de Web d'Amazon : Amazon RDS est étroitement intégré aux autres Amazon Web Services. Par exemple, une application s'exécutant dans Amazon EC2 connaîtra un accès faible latence de base de données à une Instance de DB Amazon RDS dans la même région.

Sécurisé : Amazon RDS fournit un certain nombre de mécanismes pour garantir votre DB Instances.Amazon RDS permet de crypter vos bases de données MySQL ou PostgreSQL à l'aide de touches que vous gérez par AWS Key Management Service (KMS). Sur une instance de base de données en cours d'exécution avec cryptage Amazon RDS, données stockées au repos dans le stockage sous-jacent sont cryptées, comme le sont ses sauvegardes automatisées, lire des répliques et des instantanés.
Amazon RDS prend en charge le chiffrement Transparent de données dans SQL Server et Oracle. Chiffrement transparent de données dans Oracle est intégré avec AWS CloudHSM, qui permet de générer en toute sécurité, stocker et gérer vos clés de cryptage dans les appareils Hardware Security Module (HSM) locataire unique dans le nuage AWS.
Amazon RDS inclut des interfaces de services web pour configurer les paramètres de pare-feu qui contrôlent l'accès réseau à votre base de données.

Amazon RDS vous permet d'exécuter vos Instances DB dans Amazon Virtual Private Cloud (Amazon VPC). Amazon VPC vous permet d'isoler vos Instances DB en spécifiant la plage d'adresses IP que vous souhaitez utiliser et vous connecter à votre informatique existante infrastructure par le biais de standards cryptées IPsec VPN. Pour en savoir plus sur Amazon RDS en VPC, reportez-vous au Guide d'utilisation Amazon RDS.
Peu coûteux : Vous payez des taux très bas et uniquement pour les ressources que vous consommez réellement. En outre, vous bénéficiez de l'option de demande de prix avec aucun engagement initial ou à long terme, ou encore plus bas horaires tarifs via notre option de tarification réservée.

Instances DB sur demande – Instances DB à la demande vous permettent de payer pour la capacité de calcul à l'heure avec aucun engagement à long terme. Cela vous évite les coûts et la complexité de la planification, d'achat et entretien matériel et transforme ce qui sont communément gros coûts fixes en coûts de variables beaucoup plus petites.
Les Instances réservées DB – Instances DB réservées vous donner la possibilité d'effectuer un paiement de faible, unique pour chaque Instance de DB vous voulez réserver et recevoir à son tour une réduction significative sur les frais d'utilisation horaire pour cette Instance de DB. Selon votre utilisation, vous pouvez choisir entre trois types d'Instance DB réservée (léger, moyen et utilisation lourde) et de recevoir n'importe où entre 30 % et 55 % de remise sur les prix à la demande.

