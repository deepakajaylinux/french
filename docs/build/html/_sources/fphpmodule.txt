===========
PHPModules
===========

synopsis
-------------

Ce Modules vise à installer et enveloppant certains des modules PHP communs et utiles, soutenir. Quelques exemples sont: php5-gd l'libs d'image, php5-libs imagick l'image, php5-curl la manipulation libs, php5-mysql les libs pour la gestion des connexions mysql fichier distant. Voyons comment utiliser ce module, le processus d'installation dans les prochains sujets.

Commande Aide
----------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module PHP. Il énumère les alternatives aux paramètres du module PHP. Il décrit également la syntaxe pour installer le module PHP. La commande d'aide pour le module PHP est représentée ci-dessous.

.. code-block:: bash
	
		ptconfigure PHPModules help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide pour le module PHP.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPModules help

 ******************************


  This command allows you to install some common and helpful PHP Modules.

  PHPModules, php-mods, phpmods, php-modules, phpmodules

        - install
        Installs some common PHP Modules. These include php5-gd the image libs,
        php5-imagick the image libs, php5-curl the remote file handling libs,
        php5-mysql the libs for handling mysql connections.
        example: ptconfigure phpmods install

 ------------------------------
 End Help
 ******************************


installation
--------------

La commande utilisée pour installer les modules php dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash

		ptconfigure phpmods install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +---------------------------+----------------------------------------------+-----------+--------------------------------------------+
 | paramètres                | paramètre alternatif                         | option    | commentaires                               |
 +===========================+==============================================+===========+============================================+
 |Install PHP Modules?(Y/N)  | au lieu de phpmods nous pouvons utiliser     | Yes       | Si l'utilisateur souhaite procéder à       |
 |                           | PHPModules, php-mods, php-modules,           |           | l'installation processus, ils peuvent      |
 |                           | phpmodules aussi                             |           | entrée comme Y                             |
 +---------------------------+----------------------------------------------+-----------+--------------------------------------------+
 |Data directory             | au lieu de phpmods nous pouvons utiliser     | No        | Si l'utilisateur souhaite quitter le       |
 |                           | PHPModules, php-mods, php-modules,           |           | d'installation qu'ils peuvent entrée comme |
 |                           | phpmodules aussi.                            |           | N.|                                        |
 +---------------------------+----------------------------------------------+-----------+--------------------------------------------+

	

Si l'utilisateur procède à l'installation, au cours du processus d'installation est décrite dans les listes ci-dessous:


* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les paquets qui sont automatiquement installés.
* Liste outs les nouveaux paquets qui installent.
* Détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.


La capture d'écran ci-dessous représente graphiquement le processus décrit ci-dessus de l'installation.
.. code-block:: bash



 kevell@corp:/# ptconfigure phpmods install

 Install PHP Modules? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mods!        *
 *******************************
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 /packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists 
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 php5_invoke: Enable module apcu for cgi SAPI
 php5_invoke: Enable module apcu for cli SAPI
 rmdir: failed to remove â€˜/usr/share/doc/php-apcâ€™: Directory not empty
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  php5-apcu
 Suggested packages:
  php5-gd
 The following NEW packages will be installed:
  php-apc php5-apcu
 0 upgraded, 2 newly installed, 0 to remove and 252 not upgraded.
 Need to get 75.9 kB of archives.
 After this operation, 344 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe php5-apcu amd64 4.0.2-2build1 [73.2 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/universe php-apc all 4.0.2-2build1 [2,762 B]
 Fetched 75.9 kB in 42s (1,783 B/s)
 Selecting previously unselected package php5-apcu.
 (Reading database ... 233423 files and directories currently installed.)
 Preparing to unpack .../php5-apcu_4.0.2-2build1_amd64.deb ...
 Unpacking php5-apcu (4.0.2-2build1) ...
 Selecting previously unselected package php-apc.
 Preparing to unpack .../php-apc_4.0.2-2build1_all.deb ...
 Unpacking php-apc (4.0.2-2build1) ...
 Setting up php5-apcu (4.0.2-2build1) ...
 Setting up php-apc (4.0.2-2build1) ...
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt executed correctly
 php5_invoke: Enable module gd for cgi SAPI
 php5_invoke: Enable module gd for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
   php5-gd
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 0 B/28.0 kB of archives.
 After this operation, 163 kB of additional disk space will be used.
 Selecting previously unselected package php5-gd.
 (Reading database ... 233448 files and directories currently installed.)
 Preparing to unpack .../php5-gd_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking php5-gd (5.5.9+dfsg-1ubuntu4.7) ...
 Setting up php5-gd (5.5.9+dfsg-1ubuntu4.7) ...
 [Pharaoh Logging] Adding Package php5-gd from the Packager Apt executed correctly
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
  php5-imagick : Depends: libmagickcore3 (>= 8:6.6.0.4) but it is not installable
                Depends: libmagickwand3 (>= 8:6.6.0.4) but it is not installable
                Depends: libtiff4 but it is not installable
                Depends: php5-common (= 5.3.29-1~dotdeb.0) but 5.5.9+dfsg-1ubuntu4.7 is to be installed
 [Pharaoh Logging] Adding Package php5-imagick from the Packager Apt did not execute correctly
 php5_invoke: Enable module curl for cgi SAPI
 php5_invoke: Enable module curl for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  php5-curl
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 0 B/27.4 kB of archives.
 After this operation, 142 kB of additional disk space will be used.
 Selecting previously unselected package php5-curl.
 (Reading database ... 233455 files and directories currently installed.)
 Preparing to unpack .../php5-curl_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking php5-curl (5.5.9+dfsg-1ubuntu4.7) ...
 Setting up php5-curl (5.5.9+dfsg-1ubuntu4.7) ...
 [Pharaoh Logging] Adding Package php5-curl from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 php5-mysql is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 252 not upgraded.
 [Pharaoh Logging] Package php5-mysql from the Packager Apt is already installed, so not installing.
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
 php5-memcache : Depends: php5-common (= 5.3.29-1~dotdeb.0) but 5.5.9+dfsg-1ubuntu4.7 is to be installed
 [Pharaoh Logging] Adding Package php5-memcache from the Packager Apt did not execute correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   php5-memcached
 0 upgraded, 0 newly installed, 0 to remove and 251 not upgraded.
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt did not execute correctly
 php5_invoke: Enable module mongo for cgi SAPI
 php5_invoke: Enable module mongo for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  php5-mongo
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 94.5 kB of archives.
 After this operation, 334 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe php5-mongo amd64 1.4.5-1build1 [94.5 kB]
 Fetched 94.5 kB in 45s (2,096 B/s)
 Selecting previously unselected package php5-mongo.
 (Reading database ... 233462 files and directories currently installed.)
 Preparing to unpack .../php5-mongo_1.4.5-1build1_amd64.deb ...
 Unpacking php5-mongo (1.4.5-1build1) ...
 Setting up php5-mongo (1.4.5-1build1) ...
 [Pharaoh Logging] Adding Package php5-mongo from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPModules: Success
 ------------------------------
 Installer Finished
 ******************************


avantages
------------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Tout l'installation fréquemment utilisé des modules php se enveloppait dans un processus unique.

