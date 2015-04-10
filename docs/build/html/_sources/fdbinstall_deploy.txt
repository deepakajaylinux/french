==============
DBInstall
==============


Synopsis
-------------

Dbinstall module aide dans le traitement des fonctions d'installation de base de données. Cette commande permet d'installer une nouvelle base de données. L'installation requiert un accès de sudo, ou il doit être exécuté en tant que root. Cela comprend l'exécution de la commande rpm ou la commande miminstall du paquet de goudron, et aussi lors de l'utilisation de la commande dbinstall qui crée une base de données initiale.

Tout en créant une base de données initiale, vous avez installé le logiciel, vous pouvez construire une base de données SQL Mimer en utilisant la commande de dbinstall.

Nous venons d'installer une nouvelle base de données sur un serveur Linux (CentOS) et quand je essaie de se connecter à la base de données (à partir du serveur), il requiert le nom de base de données dans la chaîne de connexion. Comme mentionné précédemment, la commande dbinstall nécessite un accès à sudo, ou doit être exécutée par l'utilisateur root. Si pas commencé à partir d'un shell de passe privilégiée sudo sera demandé.

Au cours de la session de dbinstall, le nom de base de données, l'emplacement de base de données, et mot de passe de l'administrateur (c.-à-SYSADM) de base de données doit être précisé. Il y aura aussi des options pour l'installation exemple environnements, etc. Lorsque la session est terminée, une base de données pleinement opérationnelle est disponible - pour un accès client / serveur sur TCP et démarrage automatique lors de la réinitialisation.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module DBinstall. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
	
		ptdeployDBInstall help
       
La représentation picturale de la commande ci-dessus est illustré ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptdeployDBInstall help
 ******************************


  This command is part of Default Modules and handles Database Installation Functions.

  DBInstall, db-install, dbinstall

          - install
          install the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploydb-install install

          - save
          save the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploydb-install save

          - drop
          drop the database for a project.
          example: ptdeploydb-install drop

      
 --------------
  Wordpress Module:

  The Wordpress module extends DBInstall by adding wordpress-install

  Wordpress module adds the actions wordpress-install and wp-install to DBInstall, requiresd to allow the Post DB
  Install hooks for Wordpress, the DB restore won't work correctly without at least the url.

  ptdeploydbinstall wordpress-install --yes --guess --hook-url=www.site.env
 ------------------------------
 End Help
 ******************************







Installation
----------------

Lorsque l'utilisateur doit installer, l'utilisateur peut émettre les commandes suivantes pour DBIstall. Le système exécute le processus d'installation.

.. code-block:: bash
	
		 ptdeploydbinstall install

.. code-block:: bash


 kevell@corp:/# ptdeploy DBInstall install
 Do you want to install a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User? 

 You must enter a value. Please try again.
 What's the MySQL Admin User?

 You must enter a value. Please try again.
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB User?
 (0) **CREATE NEW USER** 
 (1) phpci 
 (2) debian-sys-maint 
 (3) phpci 
 (4) phpmyadmin 
 1
 What's the application DB Password?
 phpci_pass
 What's the application DB Name?
 Current Db's are:
 hps
 phpci
 phpmyadmin

 phpci
 Database script executed
 **************************************
 Seems Fine...Database Actions Finished
 **************************************




Save
---------

Une fois les détails ci-dessus fournis, le système demande confirmation. Après confirmation, le système exécute le processus.

.. code-block:: bash
	
		ptdeploydbinstall save	

.. code-block:: bash


 kevell@corp:/# ptdeploy DBInstall save
 Do you want to save a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB Name?
 Current Db's are:
 asdf
 hps
 phpci 

 asdf
 Cannot connect with these details. Sure you want to continue? (Y/N) 
 y
 Exporting DB to /opt/db/database.sql 
 Database Dumping...
 **************************************
 Seems Fine...Database Actions Finished
 ************************************** 



Drop
----------------

Lorsque l'utilisateur a besoin de supprimer la base d'un projet, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
		ptdeploydbinstall drop      

.. code-block:: bash


 kevell@corp:/# ptdeploy db-install drop 

 Do you want to perform drop actions (user/db)? (Y/N) 
 y
 Do you want to drop a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root123
 What's the application DB Name?
 (0) karuna 
 (1) test1 
 (2) test2 
 2
 Database test2 dropped
 **************************************
 Seems Fine...Database Actions Finished
 **************************************



Alternative Paramètre
------------------------------

Soit des trois paramètre alternatif peut être utilisé dans commandement  dbinstall, DBInstall and db-install

eg: ptdeployDBInstall help/  ptdeploydb-install help                 

avantages
--------------

* Il se contrôler et de vérifier toutes les dépendances pour le paquet qu'il installe
* Ce sera exécuté dbconfigure premier à mettre en place les utilisateurs moins que le système possède déjà
* Dbinstall crée toutes les banques de données du système dans le répertoire d'accueil du serveur de base de données donnée

