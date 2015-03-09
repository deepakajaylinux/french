==================
PTDeploy
==================

Synopsis
-------------

Le ptdeploy enveloppe les applications des utilisateurs avec déploiement automatisé, construire et libérer fonctions, Web App versionnage et l'infrastructure par code en PHP.

Afin de construire pour le bien-déploiement, de nombreux fichiers sont nécessaires pour être copié à partir de FTP ou d'autres solutions ad hoc. Et aussi beaucoup d'outils Enterprise Automation manquait. Afin de surmonter ces pénuries ptdeploy sous l'outil de pharaon étaient construire. PHP a ptdeploy tout comme Ruby fiils l'écart dans ptdeploy.

Cet outil est destiné aux applications de provisionnement et construit à vos boîtes. L'utilisateur peut mettre en place même modèle simple ou complexe le déploiement d'applications à leur système avec un ou deux fichiers PHP ou, rapidement modèles de déploiement amicales configuration de nuages.

ptdeploy est modulaire, orienté objet et extensible. Donc, si l'utilisateur nécessite des modules supplémentaires ils peuvent créer et ajouter les nouveaux modules en fonction de leurs exigences.

Ce ptdeploy agit comme une enveloppe où toutes les étapes du déploiement de l'utilisateur se couvrir en un seul fichier. Cela permet d'utiliser une seule commande pour tirer une instance de vos applications.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de ptdeploy. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
         ptconfigure ptdeploy help

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy help
 ******************************


  This command allows you to update ptdeploy.

  ptdeploy, dapper, ptdeploy

        - install
        Installs the latest version of ptdeploy
        example: ptconfigure ptdeploy install

        - ensure
        Installs the latest version of ptdeploy, only if a version is not installed
        example: ptconfigure ptdeploy ensure

 ------------------------------
 End Help
 ******************************

installation
----------------

Cette commande permet d'installer la dernière version de ptdeploy. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
        ptconfigure ptdeploy install

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy install
 Install ptdeploy ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ptdeploy         *
 *******************************
 What is the program data directory? Found "/opt/ptdeploy" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/ptdeploy.git'  /tmp/ptdeploy/ptdeployCloning into '/tmp/ptdeploy/ptdeploy'...
 remote: Counting objects: 6989, done.
 remote: Total 6989 (delta 0), reused 0 (delta 0), pack-reused 6989
 Receiving objects: 100% (6989/6989), 2.61 MiB | 176.00 KiB/s, done.
 Resolving deltas: 100% (4335/4335), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************


assurer
----------------

Cette commande permet d'installer la dernière version de ptdeploy, seulement si une version ne est pas installé. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
        ptconfigure ptdeploy ensure

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************




Options
-----------                               

.. cssclass:: table-bordered


 +-------------------------+-----------------------------------------------------------+-------------+------------------------------------+
 | paramètres	           | Autres paramètres                                         | requis      | commentaire	                  |
 +=========================+===========================================================+=============+====================================+
 |ptconfigure ptdeploy     | Il ya deux autres paramètres qui peuvent être utilisés    | Y           | Le système démarre processus       |
 |install? (Y/N)           | en ligne de commande. ptdeploy, dapper, ptdeploy example: |             | d'installation                     |
 |                         | ptconfigure ptdeploy install / ptconfigure dapper install |             |                                    |
 +-------------------------+-----------------------------------------------------------+-------------+------------------------------------+
 |ptconfigure ptdeploy     | Il ya deux autres paramètres qui peuvent être utilisés    | N           | Système arrête processus           |
 |install? (Y/N)           | en ligne de commande. ptdeploy, dapper, ptdeploy example: |             | d'installation                     |
 |                         | ptconfigure ptdeploy install / ptconfigure dapper install||             |                                    |
 +-------------------------+-----------------------------------------------------------+-------------+------------------------------------+



avantages
--------------

* Modification des fichiers hôtes, dossiers virtuels d'accueil, fichiers de configuration, les mises à jour de bases de données et plus 
  peuvent tous être automatisé en utilisant ce.
* En utilisant la capacité de gestion de serveur à distance, les utilisateurs peuvent automatiser les déploiements à travers l'infrastructure 
  de toute taille.
