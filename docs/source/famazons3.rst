=================
Amazon S3 
=================

synopsis
-------------

Amazon Simple Storage Service (Amazon S3), fournit aux développeurs, et il s'associe avec stockage de l'objet durable, sûr et très évolutive. Amazon S3 est facile à utiliser, avec une interface de services web simple pour stocker et récupérer n'importe quel volume de données depuis n'importe où sur le web. Avec Amazon S3, vous payez seulement pour le stockage que vous utilisez réellement. Il n'y a aucune redevance minimale et pas des coûts d'installation.

Amazon S3 peut être utilisé seul ou conjointement avec d'autres services AWS comme Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Block Store (Amazon EBS) et Glacier de l'Amazone, ainsi que les référentiels de stockage tiers et passerelles. Amazon S3 permet le stockage de l'objet rentable pour une grande variété de cas d'utilisation y compris des applications de nuage, distribution de contenu, sauvegarde et archivage, reprise après sinistre et analytique de données volumineuses.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de AWS S3. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSS3 help

 ******************************


    This is an extension provided for Handling AWSS3.

    AWSS3, awss3 aws-s3

        - ensure-bucket-exists
        Lets you add bucket to AWSS3 if doesnt exists
        example: ptconfigure AWSS3 ensure-bucket-exists
                    --yes
                    --guess
        - add-object
        Lets you upload object to bucket
        example: ptconfigure AWSS3 add-object
                    --yes
                    --guess


        - remove-bucket
          Lets you remove bucket
          example: ptconfigure AWSS3 remove-bucket
                    --yes
                    --guess

        - remove-object-all
       Lets you remove all object from a bucket
          example: ptconfigure AWSS3 remove-object-all
                    --yes
                    --guess


            - remove-object
       Lets you remove a object from a bucket
          example: ptconfigure AWSS3 remove-object
                    --yes
                    --guess

        - list
        Will display data about your AWS S3
        example: ptconfigure AWSS3 list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************


Ensure-bucket-exists
---------------------------

Cette commande permet d'ajouter seau à AWSS3 si n'existe pas. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess


Add-object 
---------------------------

Cette commande permet de télécharger des objet pour seau. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash
	
	ptconfigure AWSS3 add-object --yes –guess

Remove-bucket 
---------------------------

Cette commande est utile pour enlever les seau. Le sous compte tenu de la commande s'exécutera le processus.
 
.. code-block:: bash     

	ptconfigure AWSS3 remove-bucket --yes --guess


Remove-object-all
--------------------------

Cette commande permet de supprimer tous les objets d'un seau. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash     
	
	ptconfigure AWSS3 remove-object-all --yes --guess


Remove-object	
--------------------------

Cette commande permet de supprimer un objet d'un seau. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash     
	
	ptconfigure AWSS3 remove-object --yes --guess 

List
---------

Cette commande permet d'afficher des données sur votre S3 AWS. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash 

	ptconfigure AWSS3 list --yes --guess

Alternative Paramètre
------------------------------
       
Il y a trois paramètres de substitution qui peuvent être utilisés en ligne de commande.

AWSS3, awss3 aws-s3 

avantages
--------------

Durable : Amazon S3 fournit une infrastructure durable pour stocker des données importantes et est conçu pour une durabilité de 99.999999999 % d'objets. Redondante, vos données sont stockées dans plusieurs établissements et plusieurs périphériques dans chaque établissement.

Faible coût : Amazon S3 permet de stocker de grandes quantités de données à un coût très faible. Vous payez pour ce que vous avez besoin, sans engagements minimaux ou droits payables d'avance.

Disponible : Amazon S3 est conçu pour une disponibilité de 99,99 % des objets au cours d'une année donnée.  Amazon S3 est également soutenu par le contrat de niveau de Service de Amazon S3, veiller à ce que vous pouvez compter sur elle quand vous en avez besoin. Et vous pouvez choisir une région AWS pour la latence, minimiser les coûts, ou répondre aux exigences réglementaires.

Sécurisé : Amazon S3 prend en charge le transfert de données par SSL et cryptage automatique de vos données une fois qu'il est transféré. Vous pouvez également configurer le seau politiques pour gérer les autorisations de l'objet et de contrôler l'accès à vos données en utilisant l'identité de l'AWS et gestion des accès (IAM).

Modulable : Avec Amazon S3, vous pouvez stocker autant de données que vous voulez et y accéder lorsque vous en avez besoin. Vous pouvez arrêter de deviner vos besoins de stockage futurs et échelle de haut en bas selon les besoins, augmentant considérablement la réactivité de votre entreprise.

Envoyer les Notifications d'événements : Amazon S3 peut envoyer des notifications d'événements lorsque les objets sont téléchargés vers Amazon S3. Notifications d'événement Amazon S3 peuvent être envoyées à l'aide d'Amazon SQS ou Amazon SNS, ou envoyées directement à AWS Lambda, vous permettant à des workflows de déclencheur, alertes ou tout autre traitement. Par exemple, vous pouvez utiliser Amazon S3 les notifications d'événements pour déclencher le transcodage des fichiers multimédias quand ils sont téléchargés, traitement des fichiers de données lorsqu'elles deviendront disponibles, ou synchronisation des objets Amazon S3 avec d'autres magasins de données.

Haute Performance : Amazon S3 prend en charge plusieurs parties postera pour aider à optimiser la résilience et le débit du réseau et vous permet de choisir la région AWS pour stocker vos données à proximité de l'utilisateur final et de minimiser la latence du réseau. Et Amazon S3 est intégré avec Amazon CloudFront, un service de web de diffusion de contenu qui distribue du contenu aux utilisateurs finaux avec une latence faible, les vitesses de transfert de données élevé et aucun engagement d'exigences minimales d'utilisation.
Intégrée : Amazon S3 est intégré avec d'autres services AWS pour simplifier le téléchargement de données d'Amazon S3 et le rendre plus facile de créer des solutions qui utilisent une gamme de AWS services. Amazon S3 intégrations comprennent Amazon CloudFront, Kinesis Amazon, Amazon RDS, Glacier d'Amazon, Amazon EBS, Amazon DynamoDB, Redshift Amazon, Amazon Route 53, Amazon EMR et AWS Lambda.

Facile à utiliser : Amazon S3 est facile à utiliser avec une console d'administration Web et application mobile et plein repos API et kits SDK pour une intégration aisée avec les technologies de tierce partie.

