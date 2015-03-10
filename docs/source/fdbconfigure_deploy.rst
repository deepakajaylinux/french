============
DBConfigure
============


synopsis
-------------

Cette modules fonction de la base de surnoms. Configuration peut être dérivé de cette base de données peut être placé dans le même ensemble que une base de données provenant de DbContext de définir la configuration Entity Framework pour une application. La configuration se effectue en appelant des méthodes protégées et définition des propriétés protégées de cette base de données dans le constructeur de type dérivé de usera € ™. Le type à utiliser peut également être enregistré dans le fichier de configuration de l'application. Ce est suffisant avec Ubuntu et CentOS.


Commande Aide
(-----------------------

La commande help guide l'utilisateur pour gérer la base de données dans ptdeploy. Cette commande help guide l'utilisateur pour créer une conf. Cette remise à zéro également la base de données actuelle. Bases de données sont utilisés pour soutenir les opérations internes des organisations et de soutenir la interactions en ligne avec les clients et les fournisseurs. La commande d'aide pour dbconfigure est illustré ci-dessous.

.. code-block:: bash
	
		ptdeploy  DBConfigure help

Après les entrées de commande ci-dessus, il commence à fonctionner pour gérer la base de données. Il catéchèse les fonctions dans les captures d'écran.
  La capture d'écran ci-dessous montre à propos de DBConfigure.

.. code-block:: bash

 kevell@corp:/# ptdeploy DBConfigure help
 ******************************


  This command is part of Default Modules and handles Databasing Functions.

  DBConfigure, db-configure, dbconfigure, db-conf

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --mysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30



paramètre alternatif
-----------------------------------

Il existe de nombreuses alternatives disponibles dans DBConfigure. Chaque alternative montre une avantages ajoutées à cette modules. Ils sont,

DBConfigure, db-configure, dbconfigure, db-conf.

Configurer, conf
-----------------------

Ce processus a mis en place la base de données utilisateur et passward pour un projet. Également utiliser admin pour créer de nouvelles ressources se ils ont besoin. La capture d'écran ci-dessous montre sa fonction.

.. code-block:: bash

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --m	     ysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"


La commande suivante permet de configurer.

.. code-block:: bash

		ptdeploy  db-conf Conf

Après clé dans le dessus de ladite commande le processus suivant peut être fonctionné. Il a été montré dans les captures d'écran.

Après l'entrée en Y ??, Il demande MySql utilisateur admin, Mysql hôte, application DB utilisateur, mot de passe et l'application de db, nom Db. L'utilisateur entre l'entrée pour ces ce processus commencer ses fonctions

remettre
----------

Ce processus permet de réinitialiser la base de données actuelle à des valeurs génériques. Dans de tels cas ptdeploy peut écrire avant que la configuration de base de données de l'exécution. Le nom de la base de données peut être entrée dans la même ligne de commande lui-même.

La commande suivante sert à réinitialiser.

.. code-block:: bash

		ptdeploy  db-conf reset


La capture d'écran suivante montre la fonction de ce processus.

.. code-block:: bash

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30



Option
---------------

.. cssclass:: table-bordered


 +---------------------------+------------------------------------------------+---------+---------------------------------------------+
 | paramètre                 | Autres paramètres                              | Option  | commentaires                                |
 +===========================+================================================+=========+=============================================+
 |Do you want to configure   | au lieu de DBConfigure nous pouvons utiliser,  | Y(Yes)  | Configuré la base de données sous           |
 |a database? (Y/N)          | db-configure, dbconfigure, db-conf.            |         | ptdeploy.                                   |
 +---------------------------+------------------------------------------------+---------+---------------------------------------------+
 |Do you want to configure   | au lieu de DBConfigure nous pouvons utiliser,  | N(No)   | Quittez l'écran de configuration            |
 |a database? (Y/N)          | db-configure, dbconfigure, db-conf.|           |         |                                             |
 +---------------------------+------------------------------------------------+---------+---------------------------------------------+

 
avantages
--------------

* La configuration de base de données Advantage est une haute performance, à faible entretien, config de base de données à distance qui permet 
  à l'utilisateur de créer facilement et déployer des applications client / serveur et les applications basées sur le Web.
* Il est amical avec Ubuntu et CentOS utilisateur.
* Sensibilité non de cas est un grand mérite pour ce module
* Il supporte les interfaces standards telles que PHP
* Il est facile de manipuler les fonctions de base de données
