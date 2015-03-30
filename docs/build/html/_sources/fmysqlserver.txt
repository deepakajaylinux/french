===============
Mysqlserver
===============


synopsis
------------

Ce module agit comme un facilitateur d'installer mysql-serveur avec la version mise à jour via apt-get. Si le serveur MySQL existe déjà dans votre machine, il vérifie la disponibilité d'un module nouvellement mis à jour.

Le Commandement Aide
------------------------

La commande help guide les utilisateurs au sujet de la méthodologie de l'utilisation et aussi sur les actions qui peuvent être réalisées en vertu de ces modules. Il décrit également les autres noms pour mysql-serveur. La commande pour utiliser l'option d'aide est donnée ci-dessous

.. code-block:: bash

	ptconfigure mysql-server help

Cette commande permet aux utilisateurs de prendre conscience de son but et aussi sur la commande utilisée pour l'installation du serveur MySQL.
Montre une présentation picturale sur la commande d'aide de la capture d'écran ci-dessous.

.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlServer help
 ******************************


  This command allows you to install the MySQL Server. Currently only
  Mysql Workbench, the Database management GUI provided by Oracle for
  Mysql.

  MysqlServer, mysql-server, mysqlserver

        - install
        Install some Mysql Server Tools through apt-get.
        example: ptconfigure mysql-server install

  Notes, during mysql install a root password will be set. First, it'll look
  for the parameter --mysql-root-pass, if this is not set, it'll look in the
  ptconfigure config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure.

 ------------------------------
 End Help
 ******************************


installation
--------------

La commande utilisée pour l'installation du serveur mysql est donnée ci-dessous.

.. code-block:: bash

	ptconfigure mysql-server install

Lors de l'installation, le processus suivant se produit
--------------------------------------------------------------

* Ce module aide à installer quelques outils pour le serveur mysql via apt-get.
* Initialement, un mot de passe root sera fixé.
* Lors de l'installation, il va chercher un paramètre de root-passe---mysql.
* Si la racine-passe---mysql ne est pas disponible, il recherche la config de ptconfigure pour les réglages de-root-passe mysql-défaut.
* Dans le cas des deux étapes mentionnées ci-dessus se échouait, il procédera par la mise en mot de passe root à ptconfigure.

Options supplémentaires
-------------------------
Voyons à propos, les options supplémentaires impliquées dans l'installation du serveur MySQL.

.. cssclass:: table-bordered

 +------------------------+------------------------------------------------+--------------+----------------------------------------------+
 | paramètres             | Autres Paramètres                              | Option       | Commentaires                                 |
 +========================+================================================+==============+==============================================+
 |Install MySQL Server?   | A la place du serveur MySQL ces autres noms    | Y(Yes)       | Si l'utilisateur souhaite procéder le        |
 |(Y/N)                   | peuvent être utilisés: MySQLServer,            |              | processus d'installation qu'ils peuvent      |
 |                        | mysql-server, mysqlserver.                     |              | entrée comme Y.                              |
 +------------------------+------------------------------------------------+--------------+----------------------------------------------+
 |Install MySQL Server?   | A la place du serveur MySQL ces autres noms    | N(No)        | Si l'utilisateur souhaite quitter le         |
 |(Y/N)                   | peuvent être utilisés: MySQLServer,            |              | processus d'installation qu'ils peuvent      |
 |                        | mysql-server, mysqlserver.                     |              | entrée comme N|                              |
 +------------------------+------------------------------------------------+--------------+----------------------------------------------+

La capture d'écran ci-dessous vous donne une présentation graphique concernant le processus d'installation.


.. code-block:: bash



 kevell@corp:/# ptconfigure mysql-server install 
 Install MySQL Server? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         MySQL Server!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  libboost-filesystem1.54.0 libboost-program-options1.54.0 
  libboost-thread1.54.0 libgoogle-perftools4 libpcrecpp0 libsnappy1 
  libtcmalloc-minimal4 libunwind8 mongodb-clients 
 Use 'apt-get autoremove' to remove them. 
 The following NEW packages will be installed: 
  debconf-utils 
 0 upgraded, 1 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 57.4 kB of archives. 
 After this operation, 157 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main debconf-utils all 1.5.51ubuntu2 [57.4 kB] 
 Fetched 57.4 kB in 14s (4,097 B/s) 
 Selecting previously unselected package debconf-utils. 
 (Reading database ... 380784 files and directories currently installed.) 
 Preparing to unpack .../debconf-utils_1.5.51ubuntu2_all.deb ... 
 Unpacking debconf-utils (1.5.51ubuntu2) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up debconf-utils (1.5.51ubuntu2) ... 
 [Pharaoh Logging] Adding Package debconf-utils from the Packager Apt executed correctly 
 Creating /tmp/ptconfigure-temp-script-12002365099.sh 
 chmod 755 /tmp/ptconfigure-temp-script-12002365099.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-12002365099.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-12002365099.sh 
 Temp File /tmp/ptconfigure-temp-script-12002365099.sh Removed 
 [Pharaoh Logging] Package mysql-client from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 
 MysqlServer: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 



Si le serveur mysql est existe déjà dans votre machine, il jettera un message à l'utilisateur comme il est déjà installé. La capture d'écran ci-dessous représente le processus d'assurer:


.. code-block:: bash

 kevell@corp:/# ptconfigure mysql-server install
 Install MySQL Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Server!        *
 *******************************
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-23889189196.sh
 chmod 755 /tmp/ptconfigure-temp-script-23889189196.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23889189196.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23889189196.sh
 Temp File /tmp/ptconfigure-temp-script-23889189196.sh Removed
 [Pharaoh Logging] Package mysql-client from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlServer: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
----------

* Lors de l'installation du serveur mysql, il se installe avec la version mise à jour.
* Il se assure avant d'installer, et vérifier la disponibilité des modules.
* En cas de nouveaux modules inclus dans la version mise à jour, le module manquant sera installé individuellement.
* Il vérifie la disponibilité des fonctions de la bibliothèque dans le serveur mysql.
