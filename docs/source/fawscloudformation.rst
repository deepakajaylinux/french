==================
AWSCloudFormation
==================

synopsis
-------------

AWS CloudFormation donne aux développeurs et administrateurs système un moyen facile de créer et gérer une collection de ressources connexes de AWS, mise en service et leur mise à jour de façon ordonnée et prévisible.


Vous pouvez utiliser exemples de modèles de AWS CloudFormation ou créer vos propres modèles pour décrire les ressources de l'AWS et les dépendances associées ou les paramètres d'exécution, nécessaires à l'exécution de votre application. Vous n'avez pas besoin de comprendre l'ordre pour la fourniture des services AWS ou les subtilités de faire fonctionner les ces dépendances. CloudFormation s'occupe de cela pour vous. Une fois les ressources AWS sont déployés, vous pouvez modifier et mettre à jour de manière contrôlée et prévisible, en vigueur en appliquant le contrôle de version à votre infrastructure AWS comme vous le faites avec votre logiciel.


Vous pouvez déployer et mettre à jour un modèle et sa collection associé liée des ressources (appelée une pile) en utilisant l'AWS Management Console, AWS Command Line Interface ou API. CloudFormation est disponible sans frais supplémentaires, et vous ne payez que pour les ressources AWS nécessaires à l'exécution de vos applications.


Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de AWS CloudFormation. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran du même. 

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudFormation help

 ******************************


  This command allows you to install a The AWS Cloud Formation Command
  Line Tools. This tool is provided by

  AWSCloudFormation, aws-cloud-formation, aws-cloudformation

        - install
        Installs AWSCloudFormation. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudFormation.
        example: ptconfigure aws-cloud-formation install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Si l'utilisateur a besoin d'installer le module de AWSCloudFormation dans la machine, le dessous étant donné de commande exécutera le processus d'installation.

.. code-block:: bash
        
       ptconfigure aws-cloud-formation install

.. code-block:: bash 

 kevell@corp:/# ptconfigure aws-cloud-formation install

 Install AWSCloudFormation? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         AWS CloudFn!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-17956189939.sh
 chmod 755 /tmp/ptconfigure-temp-script-17956189939.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-17956189939.sh Permissions
 Executing /tmp/ptconfigure-temp-script-17956189939.sh
 Cloning into 'aws-cloudformation'...
 remote: Counting objects: 64, done.
 remote: Total 64 (delta 0), reused 0 (delta 0), pack-reused 64
 Unpacking objects: 100% (64/64), done.
 Checking connectivity... done.
 mv: cannot move ‘/tmp/aws-cloudformation/bin’ to ‘/opt/aws-cloudformation/bin’: Directory not empty
 mv: cannot move ‘/tmp/aws-cloudformation/lib’ to ‘/opt/aws-cloudformation/lib’: Directory not empty
 Temp File /tmp/ptconfigure-temp-script-17956189939.sh Removed
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 AWSCloudFormation: Success
 ------------------------------
 Installer Finished
 ******************************


Alternative Paramètre
-----------------------


Il y a trois paramètres de substitution qui peuvent être utilisés en ligne de commande.


AWSCloudFormation, aws-cloud-formation, aws-cloudformation 


avantages
--------------

Prend en charge une gamme large de ressources de l'AWS : AWS CloudFormation prend en charge une large gamme de AWS ressources, vous permettant de construire un haut niveau de disponibilité, fiable et infrastructure évolutive de AWS pour votre application. AWS CloudFormation prend actuellement en charge des ressources dans les services AWS suivants :


Auto Scaling

Amazon CloudFront

AWS CloudWatch

Amazon DynamoDB

Amazon EC2

Amazon ElastiCache

AWS Elastic Beanstalk

AWS Elastic Load Balancing

AWS Identity and Access Management

Amazon RDS

Amazon Redshift

Amazon Route 53

Amazon S3

Amazon SimpleDB

Amazon SNS

Amazon SQS

Amazon VPC

Facile à utiliser : CloudFormation, il est facile d'organiser et de déployer une collection de ressources AWS et permet de vous décrivez les dépendances ou les paramètres spéciaux pour passer en cours d'exécution. Vous pouvez utiliser un des nombreux modèles échantillon de CloudFormation--soit in extenso, soit comme point de départ.


Pas besoin de réinventer la roue : un modèle peut être utilisé à plusieurs reprises pour créer des copies identiques de la même pile (ou utiliser comme base pour démarrer une nouvelle pile). Vous pouvez capturer et contrôler les variations d'infrastructures propres à la région comme AMIs de Amazon EC2, ainsi que les noms de snapshot Amazon Elastic Block Store (EBS) et Amazon RDS.


Transparent et ouvert : les Templates sont des fichiers texte simple au format JSON qui peuvent être placés sous vos mécanismes de contrôle de la source normale, stockées dans des emplacements privés ou publics tels que Amazon S3 et échangés par courrier électronique. Avec AWS CloudFormation, vous pouvez « ouvrir le capot, » pour voir exactement quelles ressources AWS forment une pile. Vous conservez le contrôle total et avez la possibilité de modifier le quelconque des ressources AWS créés dans le cadre d'une pile.

Déclarative et Flexible : pour créer l'infrastructure souhaitée, vous énumérer quelles ressources AWS, les valeurs de configuration et interconnexions vous avez besoin d'un modèle et puis laissez AWS CloudFormation font le reste avec quelques clics simples en une seule commande à l'aide de l'interface de ligne de commande AWS, l'AWS Management Console, ou un simple demande en appelant l'API. Vous n'aurez pas de rappeler les détails de la façon de créer et d'interconnecter les ressources respectives de AWS via leur service API ; AWS CloudFormation fait pour vous. Il est également inutile d'écrire un modèle à partir de zéro, si vous commencez avec un des nombreux modèles échantillon qui viennent avec AWS CloudFormation.


Personnalisés par l'intermédiaire de paramètres : vous pouvez utiliser les paramètres pour personnaliser des aspects de votre modèle en cours d'exécution, quand la pile est construite. Par exemple, vous pouvez passer le RDS taille de base de données, EC2 types d'instances, base de données et numéros de port pour le serveur web à AWS CloudFormation lorsque vous créez une pile. Vous pouvez également utiliser un modèle paramétré pour créer des piles multiples qui peuvent différer d'une manière contrôlée. Par exemple, vos types d'instance Amazon EC2, seuils d'alarme Amazon CloudWatch et Amazon RDS-réplica de lecture paramètres peut-être différer entre les régions AWS si vous recevez plus de trafic client aux États-Unis qu'en Europe. Vous pouvez utiliser les paramètres de modèle pour le réglage de la mélodie et les seuils dans chaque région séparément et toujours s'assurer que l'application est déployée régulièrement dans toutes les régions.


Intégration prêt : Vous pouvez intégrer AWS CloudFormation avec les outils de développement et de la gestion de votre choix.


AWS CloudFormation publie des événements de progression à travers le Service de Notification Simple Amazon (SNS). Avec SNS, vous pouvez suivre les progrès de création et suppression de pile par e-mail et intégrer avec d'autres processus par programme.

Sans frais supplémentaire : AWS CloudFormation est disponible sans frais supplémentaires. Vous serez facturé uniquement les tarifs normaux pour les ressources AWS AWS CloudFormation crée et votre application utilise.


