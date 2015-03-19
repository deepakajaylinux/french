================
Amazon DynamoDB
================

synopsis
-------------

Amazon DynamoDB est un service de base de données NoSQL rapide et flexible pour toutes les applications nécessitant une latence de milliseconde cohérente, à un seul chiffre à toutes les échelles. C'est une base de données entièrement géré et supporte les document et les modèles de données clé-valeur. Son modèle de données souple et des performances fiables rendent un grand ajustement pour mobile, web, jeux, ad-tech, Ito et beaucoup d'autres applications.


Commande Aide
----------------------	

Cette commande permet de déterminer l'utilisation de AWS DynamoDB. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.


.. code-block:: bash


 kevell@corp:/# ptconfigure AWSDynamoDb help

 ******************************


    This is an extension provided for Handling AWSDynamoDb.

    AWSDynamoDb, awsdynamodb,aws-dynamodb

        - describe-table
        Describe a table
        example: ptconfigure AWSDynamoDb describe-table
                    --yes
                    --guess
        - delete-table
        Lets you delete a table
        example: ptconfigure AWSDynamoDb delete-table
                    --yes
                    --guess


        - create-table
          Lets you create a table
          example: ptconfigure AWSDynamoDb create-table
                    --yes
                    --guess




        - list
        Will display data about your AWS AWSDynamoDb
        example: ptconfigure AWSDynamoDb list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************

Describe-table 
-------------------

Cette commande permet de décrire un tableau. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash

	 ptconfigure AWSDynamoDb describe-table --yes --guess

Delete-table 
-------------------

Cette commande permet de supprimer une table. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash

	ptconfigure AWSDynamoDb delete-table --yes --guess

Create-table
---------------------

Cette commande permet de créer une table. La partie la plus critique est que c'est irréversible.


.. code-block:: bash     

	ptconfigure AWSDynamoDb create-table --yes --guess 


List 
---------------------

Cette commande permet d'afficher des données sur votre AWSDynamoDb AWS. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash 
	
	ptconfigure AWSDynamoDb list --yes --guess

Alternative Paramètre
------------------------------       

Il y a deux autres paramètres qui peuvent être utilisés en ligne de commande.


AWSDynamoDb, awsdynamodb,aws-dynamodb 

avantages
--------------

Scan restreint d'Index secondaire – un moyen plus simple pour numériser des tables DynamoDB : Amazon DynamoDB permet de récupérer tous les éléments d'une table à l'aide de l'opération d'analyse. Avec Scan d'Index secondaire, vous pouvez maintenant utiliser l'opération d'analyse sur les index secondaires et récupérer toutes les données de certains attributs et les éléments qui sont projetées sur un index secondaire. Secondaire Index Scan fonctionne sur les index secondaires les et mondiaux. Index secondaires peuvent être numérisés à partir de la console de DynamoDB ou en appelant l'API d'analyse avec un paramètre supplémentaire pour spécifier l'index.


Indexation en ligne-une méthode flexible pour gérer les index secondaires Global : Amazon DynamoDB permet de créer des index secondaires Global (GSI) à table créer le temps. GSIs vous permettent d'écrire des requêtes riches avec des filtres. Avec l'indexation en ligne, vous pouvez ajouter ou supprimer le GSIs à une table de DynamoDB à tout moment à l'aide de la console de DynamoDB, ou via un simple appel d'API. Tandis que la GSI est ajouté ou supprimé, le DynamoDB table peut toujours gérer le trafic en ligne et fournir un service continu au niveau du débit mis en service.


Inscrivez-vous pour la prévisualisation des cours d'eau DynamoDB : DynamoDB cours d'eau fournit un temps commandé des question niveau change dans n'importe quelle table de DynamoDB. Les changements sont dédupliquées et stockées pendant 24 heures. Cette fonctionnalité permet aux développeurs d'étendre la puissance de DynamoDB avec croix-région réplication, analytique continue avec Redshift intégration, notifications de changement et bien d'autres.


