================
MysqlTools
================

synopsis
-----------

Ce module vise à installer quelques outils qui aide le serveur MySQL. Il facilite également l'installation du GUI et MySQL Workbench ainsi que mytop outil de ligne de commande.

Commande Aide
--------------

La commande help instruit les utilisateurs dans la manipulation de ce module. En plus de cela, il sera également fixé les paramètres de remplacement. La commande utilisée pour l'option d'aide est donnée ci-dessous:

.. code-block:: bash

	ptconfigure MysqlTools help

La commande d'aide précise également la commande utilisée pour installer ce module mysqltools. Regardez la capture d'écran ci-dessous.

.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools help

 ******************************


  This command allows you to install some tools to help with MySQL Server. Installs the MySQL
  Workbench GUI and also the mytop Command Line Tool.

  MysqlTools, mysql-tools, mysqltools

        - install
        Installs Mysql Tools through apt-get.
        example: ptconfigure mysql-tools install

 ------------------------------
 End Help
 ******************************


installation
-------------

Ce module installe les outils de mysql qui prend en charge le serveur mysql à l'aide d'apt-get. La commande utilisée pour l'installation mysqltools à votre machine est indiqué ci-dessous:
.. code-block:: bash

	ptconfigure MysqlTools install


.. cssclass:: table-bordered


 +----------------------+--------------------------------------------+---------------+------------------------------------------+
 | paramètres           | alternative Paramètres                     | Option        | Commentaires                             |
 +======================+============================================+===============+==========================================+
 |Install MySQL Tools?  | A la place de MySQL Outils ces autres noms | Y(Yes)        | Si l'utilisateur souhaite procéder le    |
 |(Y/N)                 | peuvent être utilisés: MysqlTools,         |               | processus d'installation qu'ils peuvent  |
 |                      | mysql-outils, mysqltools.                  |               | entrée comme Y.                          |
 +----------------------+--------------------------------------------+---------------+------------------------------------------+
 |Install MySQL Tools?  | A la place de MySQL Outils ces autres noms | N(No)         | Si l'utilisateur souhaite procéder le    |
 |(Y/N)                 | peuvent être utilisés: MysqlTools,         |               | processus d'installation qu'ils peuvent  |
 |                      | mysql-outils, mysqltools.                  |               | entrée comme N.|                         |
 +----------------------+--------------------------------------------+---------------+------------------------------------------+



Si l'utilisateur de procéder l'installation des outils de mysql les opérations suivantes sont effectuées lors de l'installation



* Il lit les listes de paquets.
* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Installe les paquets supplémentaires qui sont nécessaires.
* Installe les paquets suggérés.
* Installe les nouveaux paquets.
* Affiche le nombre de fichiers qui sont mis à niveau, nouvellement installés, enlevés, et non mis à niveau.

La capture d'écran comme indiqué ci-dessous vous donne une présentation graphique concernant les mesures comme expliqué ci-dessus.

.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools install

 Install MySQL Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Tools!        *
 *******************************
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:
 
 The following packages have unmet dependencies:
 mysql-workbench : Depends: libmysqlcppconn7 (>= 1.1.3) but it is not installabl                                                                                        e
                   Recommends: ttf-bitstream-vera but it is not going to be inst                                                                                        alled
                   Recommends: mysql-utilities but it is not going to be install                                                                                        ed
 [Pharaoh Logging] Adding Package mysql-workbench from the Packager Apt did not e                                                                                        xecute correctly
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing maintainer
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing architecture
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libconfig-inifiles-perl
 The following NEW packages will be installed:
  libconfig-inifiles-perl mytop
 0 upgraded, 2 newly installed, 0 to remove and 13 not upgraded.
 Need to get 73.8 kB of archives.
 After this operation, 288 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main libconfig-inifiles-perl                                                                                         all 2.68-1 [39.6 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe mytop all 1.9.1-1 [34                                                                                        .1 kB]
 Fetched 73.8 kB in 7s (10.5 kB/s)
 Selecting previously unselected package libconfig-inifiles-perl.
 (Reading database ... 254866 files and directories currently installed.)
 Preparing to unpack .../libconfig-inifiles-perl_2.68-1_all.deb ...
 Unpacking libconfig-inifiles-perl (2.68-1) ...
 Selecting previously unselected package mytop.
 Preparing to unpack .../archives/mytop_1.9.1-1_all.deb ...
 Unpacking mytop (1.9.1-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libconfig-inifiles-perl (2.68-1) ...
 Setting up mytop (1.9.1-1) ...
 [Pharaoh Logging] Adding Package mytop from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlTools: Success
 ------------------------------
 Installer Finished
 ******************************
 

Il sera également spécifie le nom d'outils qui sont installés, par exemple

.. code-block:: bash


 .. rubric:: mysql-server-core-5.5:amd64, mysql-server-5.5: amd64, libaio1:amd64, mysql-server:amd64.

avantages
----------

* L'utilisateur peut installer leurs outils nécessaires qui prend en charge serveur mysql.
* Il facilite également l'installation du GUI et MySQL Workbench ainsi que mytop outil de ligne de commande.
* Après l'achèvement de l'installation, il sera affiche les outils listes qui sont nouvellement installés
