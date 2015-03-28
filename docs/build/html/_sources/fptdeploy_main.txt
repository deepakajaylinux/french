============
PTDeploy
============

synopsis
------------

Le ptdeploy enveloppe les applications des utilisateurs avec déploiement automatisé, construire et libérer fonctions, Web App versionnage et l'infrastructure par code en PHP.

Il soulager les utilisateurs et fournit des modèles de déploiement automatisés et installe une version complètement continue pour votre projet.

Commande Aide
---------------------

Si vous voulez connaître le but d'un module particulier, il suffit de taper la commande comme suit:

.. code-block:: bash
	
	ptdeploy ModuleName help

cette commande permettra l'utilisation de ce module particulier et aussi les options disponibles dans les actions que vous pouvez effectuer. Explique l'utilisation du module de contrôle d'Apache sous ptdeploy aide de la commande d'aide de la capture d'écran ci-dessous.

.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheControl help
 ******************************


  This command is part of Default Modules and handles Apache Server Control Functions.

  ApacheControl, apachecontrol, apachectl

          - start
          Start the Apache server
          example: ptdeploy apachecontrol start
          example: ptdeploy apachecontrol start --yes --guess
          example: ptdeploy apachecontrol start --yes --apache-command="apache2"

          - stop
          Stop the Apache server
          example: ptdeploy apachecontrol stop
          example: ptdeploy apachecontrol stop --yes --guess
          example: ptdeploy apachecontrol stop --yes --apache-command="apache2"

          - restart
          Restart the Apache server
          example: ptdeploy apachecontrol restart
          example: ptdeploy apachecontrol restart --yes --guess
          example: ptdeploy apachecontrol restart --yes --apache-command="apache2"

          - reload
          Reloads the Apache server configuration without restarting
          example: ptdeploy apachecontrol reload
          example: ptdeploy apachecontrol reload --yes --guess
          example: ptdeploy apachecontrol reload --yes --apache-command="apache2"

 ------------------------------
 End Help
 ******************************

La commande help répertorie également les autres paramètres qui peuvent être utilisés dans la déclaration.



Pourquoi construire ce ptdeploy
------------------------------------------

Afin de construire pour le bien-déploiement, de nombreux fichiers sont nécessaires pour être copié à partir de FTP ou d'autres solutions ad hoc. Et aussi beaucoup d'outils Enterprise Automation manquait. Afin de surmonter ces pénuries ptdeploy sous l'outil de pharaon étaient construire.
PHP a ptdeploy tout comme Ruby fiils l'écart à Capistrano.

Cet outil est destiné aux applications de provisionnement et construit à vos boîtes. L'utilisateur peut mettre en place même modèle simple ou complexe le déploiement d'applications à leur système avec un ou deux fichiers PHP ou, rapidement modèles de déploiement amicales configuration de nuages.

ptdeploy est modulaire. orienté objet et extensible. Donc, si l'utilisateur nécessite des modules supplémentaires ils peuvent créer et ajouter les nouveaux modules en fonction de leurs exigences.

Ce ptdeploy agit comme une enveloppe où toutes les étapes de déploiement utilisateurs se couvre en un seul fichier. Cela permet d'utiliser une seule commande pour tirer une instance de vos applications.

Installation
---------------

Installation du ptdeploy peut se faire de deux manières possibles en fonction de la disponibilité et des besoins des utilisateurs. Ils ont deux façons d'installer ptdeploy sont:

* Installation ptdeploy via ptconfigure
* Installation du ptdeploy sans dépendre ptconfigure.

Installation ptdeploy via ptconfigure
-------------------------------------------------

Si l'utilisateur a le ptconfigure dans leur machine, puis ce est le plus simple à installer ptdeploy en utilisant la commande suivante:

.. code-block:: bash

	sudo ptconfigure ptdeploy install --yes –guess

Installation du ptdeploy sans dépendre ptconfigure
----------------------------------------------------

Si l'utilisateur souhaite installer le ptdeploy sans fonction et en utilisant le ptconfigure ils peuvent utiliser la commande suivante:


.. code-block:: bash
		
	sudo apt-get install php5 git

.. code-block:: bash

	git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install-silent

or

La commande ci-dessous est prévisible pour les utilisateurs qui souhaitent pour spécifier l'emplacement lors de l'installation.

.. code-block:: bash

	git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install

Les fonctionnalités avancées
-------------------------------

Édition des fichiers hôtes, des fichiers de l'hôte virtuel, fichiers de configuration, des mises à jour de bases de données et plus peuvent tous être automatisés à l'aide de cette.

En utilisant la capacité de gestion du serveur distant, les utilisateurs peuvent automatiser les déploiements à travers l'infrastructure de toute taille.

La façon dont l'ptdeploy la promotion de votre projet en utilisant dapperfy
-------------------------------------------------------------------------------------------

Le mot dapperfy est une commande de ptdeploy qui crée certains pilotes automatiques pour votre projet.

Utilisation de la dapperfy est très rapide, et ce est probablement le meilleur point de départ.

Capify Vs Dapperfy
-------------------------

Lorsque l'on compare l'capify avec dapperfy, il est évident de dire que le dapperfy est le meilleur comme il est écrit en PHP.

Le point fort est que la commande ptdeploy dapperfy fournit l'ensemble standard de pilotes automatiques pour les projets des utilisateurs. où le capify offre une fonction similaire au projet Ruby.

Comment utiliser et modules disponibles
-------------------------------------------------------

Voyons, comment utiliser l'outil de ptdeploy, d'abord, tapez simplement

.. code-block:: bash

	ptdeploy

Édition des fichiers hôtes, des fichiers de l'hôte virtuel, fichiers de configuration, des mises à jour de bases de données et plus peuvent tous être automatisés à l'aide de cette.

En utilisant la capacité de gestion du serveur distant, les utilisateurs peuvent automatiser les déploiements à travers l'infrastructure de toute taille.

La façon dont l'ptdeploy la promotion de votre projet en utilisant dapperfy
-------------------------------------------------------------------------------------------

Le mot dapperfy est une commande de ptdeploy qui crée certains pilotes automatiques pour votre projet.

Utilisation de la dapperfy est très rapide, et ce est probablement le meilleur point de départ.

Capify Vs Dapperfy
-------------------------

Lorsque l'on compare l'capify avec dapperfy, il est évident de dire que le dapperfy est le meilleur comme il est écrit en PHP.

Le point fort est que la commande ptdeploy dapperfy fournit l'ensemble standard de pilotes automatiques pour les projets des utilisateurs. où le capify offre une fonction similaire au projet Ruby.

Comment utiliser et modules disponibles
-----------------------------------------------

Voyons, comment utiliser l'outil de ptdeploy, d'abord, tapez simplement

.. code-block:: bash

 Available Commands:
 --------------------------------------- 

 ApacheControl - Apache Server Control
 ApacheVHostEditor - Apache Virtual Host Functions
 AppSettings - PTDeploy Application Settings
 Autopilot - PTConfigure Autopilot - User Defined Installations
 Builderfy - PTDeploy Builderfyer - Create some standard autopilots for your project
 CukeConf - Cucumber Configuration
 DBConfigure - Database Connection Configuration Functions
 DBInstall - Database Installation Management Functions
 Dapperfy - PTDeploy Dapperfyer - Automated Application Deployment autopilots for your project
 Drupal - Drupal - Integration and Templates for Drupal
 EnvironmentConfig - Environment Configuration - Configure Environments for a project
 GitClone - GitClone Source Control Clone Functions
 HostEditor - Host File Management Functions
 Invoke - SSH Invocation Functions
 Joomla - Joomla - Integration and Templates for Joomla
 LighttpdControl - Lighttpd Server Control
 Logging - Logging - Output errors to the logging
 NginxControl - Nginx Server Control
 NginxSBEditor - Nginx Server Block Functions
 ParallelSshChild - Command Execution Functions
 Project - PTDeploy Project Management Functions
 RunCommand - Execute a Command
 SFTP - SFTP Functionality
 SVN - SVN Source Control Project Checkout/Download Functions
 SystemDetection - System Detection - Detect the Running Operating System
 Templating - Templating
 Version - Versioning Functions
 Wordpress - Wordpress - Integration and Templates for Wordpress

 ******************************



.. toctree::
   :maxdepth: 6
   
 fapachecontrol_deploy
 fapachevhosteditor_deploy
 fappsettings_deploy
 fautopilot_deploy
 fdapperfy_deploy
 fdbconfigure_deploy
 fdbinstall_deploy
 fdrupal_deploy
 fenvironmentconfig_deploy
 fgitclone_deploy
 fgrafana_deploy
 fhosteditor_deploy
 finvoke_deploy
 fjoomla_deploy 
 flighttpdcontrol_deploy
 flogging_deploy
 fnginxcontrol_deploy
 fnginxsbeditor_deploy
 fproject_deploy
 fruncommand_deploy
 fsftp_deploy
 fsvn_deploy
 fsystemdetection_deploy
 ftemplating_deploy
 fversion_deploy
 fwordpress_deploy 
