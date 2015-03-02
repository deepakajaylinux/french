==============
StandardTools
==============

synopsis
----------------

Ce module aider à installer des outils standard dans le système. Il peut installer tous les outils comme vim, zip, etc ,. L'automatisation est possible. Il spécifie la normalisation de votre environnement. Il est amical avec Ubuntu et cent OS utilisateur.

Commande Aide
---------------------

Aide commande utilisée pour trouver des informations sur une commande spécifique. Pour plus d'informations sur les outils standard. nous pouvons utiliser cette commande d'aide.

.. code-block:: bash

		ptconfigure StandardTools help

La capture d'écran suivante vous guidera.

.. code-block:: bash

 kevell@corp:/# ptconfigure StandardTools help
 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  StandardTools, standard-tools, standardtools, stdtools, std-tools

        - install
        Installs some standard tools
        example: ptconfigure stdtools install

 ------------------------------
 End Help
 ******************************



installation
------------------

   En tant que société, et en tant qu'individus, Outils norme a été dédié pour répondre aux défis de l'utilisateur, se acquitter de leurs exigences, et de satisfaire leurs objectifs d'affaires. Ce est un processus évident pour installer le module d'outils standard sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

                ptconfigure stdtools install

Après avoir saisi la commande,

Installer des outils standard? (Y / N)

Si la valeur de l'utilisateur sous la forme y

Ensuite, tous les outils standard mises à jour installées.

Si la valeur de l'utilisateur que le N

Il quitte l'écran

L'écran montre.

.. code-block:: bash


 kevell@corp:/# ptconfigure stdtools install
 Install Standard Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Std. Tools!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 curl is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package curl from the Packager Apt is already installed, so not installing.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 vim is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package vim from the Packager Apt is already installed, so not installing.

 Creating config file /etc/php5/mods-available/mysql.ini with new version
 php5_invoke: Enable module mysql for cli SAPI
 php5_invoke: Enable module mysql for fpm SAPI
 php5_invoke: Enable module mysql for apache2 SAPI

 Creating config file /etc/php5/mods-available/mysqli.ini with new version
 php5_invoke: Enable module mysqli for cli SAPI
 php5_invoke: Enable module mysqli for fpm SAPI
 php5_invoke: Enable module mysqli for apache2 SAPI
 
 Creating config file /etc/php5/mods-available/pdo_mysql.ini with new version
 php5_invoke: Enable module pdo_mysql for cli SAPI
 php5_invoke: Enable module pdo_mysql for fpm SAPI
 php5_invoke: Enable module pdo_mysql for apache2 SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   php-console-table php5-mysql
 Suggested packages:
   drupal7
 Recommended packages:
  php-console-color
 The following NEW packages will be installed:
  drush php-console-table php5-mysql
 0 upgraded, 3 newly installed, 0 to remove and 13 not upgraded.
 Need to get 430 kB of archives.
 After this operation, 1,800 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main php5-mysql amd64 5.5.9+dfsg-1ubuntu4.5 [62.9 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe php-console-table all 1.1.6-1 [14.7 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe drush all 5.10.0-2 [353 kB]
 Fetched 430 kB in 1min 4s (6,634 B/s)
 Selecting previously unselected package php5-mysql.
 (Reading database ... 212663 files and directories currently installed.)
 Preparing to unpack .../php5-mysql_5.5.9+dfsg-1ubuntu4.5_amd64.deb ...
 Unpacking php5-mysql (5.5.9+dfsg-1ubuntu4.5) ...
 Selecting previously unselected package php-console-table.
 Preparing to unpack .../php-console-table_1.1.6-1_all.deb ...
 Unpacking php-console-table (1.1.6-1) ...
 Selecting previously unselected package drush.
 Preparing to unpack .../drush_5.10.0-2_all.deb ...
 Unpacking drush (5.10.0-2) ...
 Processing triggers for libapache2-mod-php5 (5.5.9+dfsg-1ubuntu4.5) ...
 Processing triggers for php5-fpm (5.5.9+dfsg-1ubuntu4.5) ...
 php5-fpm stop/waiting
 php5-fpm start/running, process 5110
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up php5-mysql (5.5.9+dfsg-1ubuntu4.5) ...
 Setting up php-console-table (1.1.6-1) ...
 Setting up drush (5.10.0-2) ...
 Processing triggers for libapache2-mod-php5 (5.5.9+dfsg-1ubuntu4.5) ...
 Processing triggers for php5-fpm (5.5.9+dfsg-1ubuntu4.5) ...
 php5-fpm stop/waiting
 php5-fpm start/running, process 6189
 [Pharaoh Logging] Adding Package drush from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 zip is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package zip from the Packager Apt is already installed, so not installing.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 StandardTools: Success
 ------------------------------
 Installer Finished
 ******************************


Autres paramètres
----------------------------------

Voici les paramètres alternatifs. StandardTools, standard-tools, standardtools, std-tools, stdtools.

avantages
-------------

* Version mise à jour de l'installation disponible.
* En cas d'exister, il peut écraser.
* Non sensible à la casse

