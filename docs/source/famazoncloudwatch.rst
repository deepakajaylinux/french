===================
Amazon CloudWatch
==================

synopsis
-------------

Amazon CloudWatch est un service de surveillance des ressources cloud AWS et les applications que vous exécutez sur AWS. Vous pouvez utiliser Amazon CloudWatch de collecter et de suivre les mesures, de recueillir et de surveiller les fichiers journaux et régler des alarmes. Amazon CloudWatch peut surveiller les ressources AWS tels que les instances Amazon EC2, Amazon DynamoDB tables et instances Amazon RDS DB, ainsi que des paramètres personnalisés générés par vos applications et services et les fichiers journaux que génèrent vos applications. Vous pouvez utiliser Amazon CloudWatch pour approfondir la visibilité de la systémique dans l'utilisation des ressources et les performances des applications Santé opérationnelle. Vous pouvez utiliser ces idées pour réagir et garder votre application fonctionne correctement.


Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'Amazon CloudWatch. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.


.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudWatch help

 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  AWSCloudWatch, aws-cloud-watch, aws-cloudwatch

        - install
        Installs AWSCloudWatch. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudWatch
        example: ptconfigure aws-cloudwatch install

 ------------------------------
 End Help
 ******************************

installation
----------------

Si l'utilisateur a besoin d'installer le module Amazon CloudWatch dans la machine, le dessous étant donné de commande exécutera le processus d'installation.


.. code-block:: bash
        
        ptconfigure aws-cloudwatch install

.. code-block:: bash 

	

avantages
--------------

Moniteur Amazon EC2 : Découvre les métriques pour CPU utilization, transfert de données et activité de l'utilisation du disque à partir d'instances Amazon EC2 (surveillance de base) sans frais supplémentaires. Moyennant des frais supplémentaires, CloudWatch fournit un suivi détaillé pour les instances EC2 avec une résolution supérieure et l'agrégation métrique. Aucun logiciel supplémentaire ne doit être installé.


Moniteur autres ressources AWS : Surveiller les métriques sur Amazon DynamoDB tableaux, volumes Amazon EBS, instances Amazon RDS DB, les flux de travail Amazon Elastic MapReduce, Elastic Load Balancers, files d'attente de Amazon SQS, Amazon SNS sujets et plus sans frais supplémentaires. Aucun logiciel supplémentaire ne doit être installé.


Moniteur Custom Metrics : Soumettre Custom Metrics générés par vos propres applications via une simple demande d'API et ont surveillé par Amazon CloudWatch. Vous pouvez envoyer et stocker les paramètres qui sont importants pour le rendement opérationnel de votre application pour vous aider à dépanner et à repérer les tendances.


Moniteur et magasin de journaux : vous pouvez utiliser les journaux CloudWatch pour surveiller et dépanner vos systèmes et applications à l'aide de votre système existant, application et les fichiers de journal des événements personnalisé. Vous pouvez envoyer votre système existant, application et les fichiers journaux personnalisés aux journaux CloudWatch et surveiller ces journaux en temps quasi réel. Cela peut vous aider à mieux comprendre et exploiter vos systèmes et applications, et vous pouvez stocker vos journaux à l'aide de stockage très résistant et peu coûteux pour un accès ultérieur.


Programmer des alarmes : Régler des alarmes sur n'importe lequel de vos paramètres pour vous envoyer des notifications ou de prendre d'autres actions automatisées. Par exemple, lorsqu'une mesure spécifique de Amazon EC2 traverse votre seuil d'alarme, vous pouvez utiliser Auto Scaling pour dynamiquement ajouter ou supprimer des instances EC2 ou vous envoyer une notification.


Afficher des graphiques et statistiques : Découvre les graphiques et statistiques pour l'un de vos paramètres du panneau de commandes Amazon CloudWatch et obtenez un aperçu rapide de toutes vos alarmes et surveillé les ressources AWS en un seul endroit.

