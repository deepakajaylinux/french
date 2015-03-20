=================
AMAZON ROUTE 53 
=================

synopsis
-------------

Amazon Route 53 est un nuage hautement disponible et évolutif service web Domain Name System (DNS). Il est conçu pour donner aux développeurs et aux entreprises un moyen extrêmement fiable et rentable aux utilisateurs finaux de route aux applications Internet en traduit les adresses IP numériques comme 192.0.2.1 que les ordinateurs utilisent pour se connecter les uns aux autres par des noms comme www.example.com.

Amazon Route 53 efficacement relie les demandes des utilisateurs à l'infrastructure en cours d'exécution dans AWS – tels que les instances Amazon EC2, équilibreurs de charge Elastic Load Balancing ou Amazon S3 seaux – et permet également aux utilisateurs de la route à l'infrastructure à l'extérieur de l'AWS. Vous pouvez utiliser Amazon Route 53 pour configurer DNS des bilans de santé pour acheminer le trafic vers des points de terminaison en bonne santé ou de contrôler indépendamment la santé de votre application et ses points de terminaison. Amazon Route 53 rend possible pour vous de gérer la circulation dans le monde à travers une variété de types de routage, y compris Weighted Round Robin, Geo DNS et latence basé routage — qui peuvent être combinés avec la reprise de DNS afin de permettre une variété d'architectures de faible latence, à tolérance de panne. Amazon Route 53 offre également l'enregistrement de nom de domaine – vous pouvez acheter et gérer des noms de domaine par exemple, exemple.com et Amazon Route 53 configure automatiquement les paramètres DNS pour vos domaines.


Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'Amazon Route 53. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSRoute53 help

 ******************************


    This is an extension provided for Handling AWS ROUTE53.

    AWSRoute53, awsroute53, aws-route53

        - create-hosted-zone
        Lets you add Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 create-hosted-zone
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess
          - delete-hosted-zone
        Lets you delete Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess
         - delete-health-check
        Lets you delete Health Check to AWS Route53
        example: ptconfigure AWSRoute53 delete-health-check
                    --yes
                    --guess

        - list
        Will display data about your AWS Route53
        example: ptconfigure AWSRoute53 list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

------------------------------
End Help
******************************

Create-hosted-zone 
---------------------------

Cette commande permet d'ajouter la zone hébergée à AWS Route53. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess


Create-health-check 
---------------------------

Cette commande permet d'ajouter le bilan de santé à AWS Route53. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check --yes --guess

Delete-hosted-zone 
---------------------------

Cette commande permet de supprimer la zone hébergé à AWS Route53. Le sous compte tenu de la commande s'exécutera le processus.


.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 


Delete-health-check 
-------------------------

Cette commande permet de supprimer le bilan de santé à AWS Route53. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash     
	
	ptconfigure AWSRoute53 delete-health-check --yes --guess


List
---------

Cette commande permet d'afficher des données sur votre Route53 AWS. Le sous compte tenu de la commande s'exécutera le processus.

.. code-block:: bash 

	ptconfigure AWSRoute53 list --yes --guess

Alternative Paramètre
-------------------------------


Il y a trois paramètres de substitution qui peuvent être utilisés en ligne de commande.

AWSRoute53, awsroute53, aws-route53 

avantages
--------------

Hautement disponible et fiable : Amazon Route 53 est construit en utilisant l'infrastructure hautement disponible et fiable d'AWS. La nature distribuée de nos serveurs DNS contribue à assurer une capacité conforme pour acheminer vos utilisateurs à votre application. Route 53 est conçu pour fournir le niveau de fiabilité requis par les applications importantes. Amazon Route 53 est soutenu par le contrat de niveau de Service Amazon Route 53.

Évolutive : Route 53 est conçu à l'échelle automatiquement pour gérer des volumes de requête très importante sans aucune intervention de votre part.

Conçu pour être utilisé avec d'autres Services de Web d'Amazon : Amazon Route 53 est conçu pour fonctionner avec d'autres caractéristiques de l'AWS et offrandes. Vous pouvez utiliser Amazon Route 53 pour mapper des noms de domaine à vos instances Amazon EC2, Amazon S3 seaux, distributions Amazon CloudFront et autres ressources AWS. En utilisant le service de l'identité de l'AWS et gestion des accès (IAM) avec Amazon Route 53, vous obtenez un contrôle précis à grains fins qui peuvent mettre à jour vos données DNS. Vous pouvez utiliser Amazon Route 53 pour mapper votre apex de zone (exemple.com versus www.example.com) à votre instance Elastic Load Balancing, Amazon CloudFront distribution ou compartiment du site Amazon S3 utilisant une fonctionnalité appelée enregistrement d'Alias.

Simple : Avec inscription self-service, Route 53 peut commencer à répondre à vos requêtes DNS dans les minutes. Vous pouvez configurer vos paramètres DNS avec l'AWS Management Console ou de notre API facile à utiliser. Vous pouvez également par programme intégrer l'API de 53 Route dans votre application web globale. Par exemple, vous pouvez utiliser des API de Route 53 pour créer un enregistrement DNS chaque fois que vous créez une nouvelle instance EC2.

Rapide : Utilisation d'un réseau d'anycast mondial de serveurs DNS dans le monde entier, Amazon Route 53 est conçu pour acheminer automatiquement vos utilisateurs vers l'emplacement optimal selon les conditions du réseau. Ainsi, le service offre de latence faible requête pour vos utilisateurs finaux, ainsi que mise à jour faible latence pour vos besoins de gestion des enregistrements DNS.

Rentable : Amazon Route 53 passe sur les avantages d'échelle de AWS à vous. Vous ne payez que pour la gestion des domaines à travers le service et le nombre de requêtes que le service répond pour chacun de vos domaines, à un faible coût et sans engagements minimums d'utilisation ou des droits payables d'avance.

Sécurisé : En intégrant Amazon Route 53 avec AWS identité et gestion des accès (IAM), vous pouvez accorder des pouvoirs uniques et gérer les autorisations pour chaque utilisateur au sein de votre compte AWS et spécifier qui a accès à quelles parties du service Amazon Route 53.

Flexible : Amazon Route 53 offre Weighted Round-Robin (WRR), également appelés équilibrage de charge DNS. Cela vous permet d'attribuer des poids à vos enregistrements DNS qui spécifie quelle partie de votre trafic est acheminé vers les différents points de terminaison.

