=======
SVN
=======

synopsis
------------

Ce module aide les utilisateurs à installer la dernière version de SVN dans Ubuntu. Apache Subversion (SVN souvent abrégé, après le nom commande svn) est un système de gestion des versions de logiciels et de contrôle de révision distribué comme logiciel libre sous licence Apache. Les développeurs utilisent Subversion pour conserver les versions actuelles et historiques de fichiers tels que le code source, pages web, et la documentation. Son objectif est d'être un successeur essentiellement compatible avec Versions System largement utilisé (CVS). Voyons comment ce module facilite dans l'installation, la désinstallation, assurer la subversion dans Ubuntu.

Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le SVN. Il énumère les autres paramètres de SVN. Il décrit également la syntaxe pour installer, désinstaller, assurer la SVN. La commande d'aide pour le module SVN est représentée ci-dessous.

.. code-block:: bash
	
		ptconfigure svn help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide sous SVN.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn help
 ******************************


  This command allows you to install the latest available SVN in the Ubuntu
  repositories.

  SVN, svn

        - install
        Installs the latest available (In your package manager) version of SVN
        example: ptconfigure svn install

        - ensure
        Ensures SVN is installed
        example: ptconfigure svn ensure

        - uninstall
        Installs the latest version of SVN
        example: ptconfigure svn uninstall

 ------------------------------
 End Help
 ******************************



installation
---------------

La commande utilisée pour installer le SVN pour l'ubuntu est illustré ci-dessous.

.. code-block:: bash
		
		ptconfigure svn install

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme le montre sous forme de tableau.

.. cssclass:: table-bordered

 +-------------------------+-------------------------------------+-----------+---------------------------------------------------+
 | Paramètre               | Autres paramètres                   | Option    | Commentaires                                      |
 +=========================+=====================================+===========+===================================================+
 |Install SVN? (Y/N)       | au lieu de SVN, nous pouvons        | Y(Yes)    | Si l'utilisateur veut le processus                | 
 |                         | utiliser, svn ainsi                 |           | d'installation, vous pouvez aller en entrée Y.    |
 +-------------------------+-------------------------------------+-----------+---------------------------------------------------+
 |Install SVN? (Y/N)       | au lieu de SVN, nous pouvons        | N(No)     | Si les utilisateurs veulent, ils peuvent          |
 |                         | utiliser, svn ainsi                 |           | terminer l'entrée de processus d'installation N.| |
 +-------------------------+-------------------------------------+-----------+---------------------------------------------------+


Si l'utilisateur procède le processus d'installation, pendant l'exécution de l'installation, le processus suivant se produit:

* Lit listes de paquets.
* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Répertorie les paquets supplémentaires installés.
* Les listes de nouveaux paquets installés.
* Nombre de fichiers mis à niveau, nouvellement installés, retirés, pas mis à niveau.
* Enfin, l'installation de SVN se rempli. La capture d'écran ci-dessous vous montre sur le processus d'installation SVN dans Ubuntu.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn install
 Install SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libserf-1-1 libsvn1
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  libserf-1-1 libsvn1 subversion
 0 upgraded, 3 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,240 kB of archives.
 After this operation, 4,701 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libserf-1-1 amd64 1.3.3-1ubuntu0.1 [42.2 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libsvn1 amd64 1.8.8-1ubuntu3.1 [917 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main subversion amd64 1.8.8-1ubuntu3.1 [280 kB]
 Fetched 1,240 kB in 43s (28.3 kB/s)
 Selecting previously unselected package libserf-1-1:amd64.
 (Reading database ... 211229 files and directories currently installed.)
 Preparing to unpack .../libserf-1-1_1.3.3-1ubuntu0.1_amd64.deb ...
 Unpacking libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Selecting previously unselected package libsvn1:amd64.
 Preparing to unpack .../libsvn1_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Selecting previously unselected package subversion.
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Setting up libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************


Un installer
-------------

La commande utilisée pour l'ONU d'installer le SVN pour l'ubuntu est illustré ci-dessous.

.. code-block:: bash

		ptconfigure svn uninstall

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +-------------------------+---------------------------------------+------------+----------------------------------------------------+
 | Paramètre               | Autres paramètres                     | Option     | Commentaires                                       |
 +=========================+=======================================+============+====================================================+
 |Uninstall SVN? (Y/N)     | au lieu de SVN, nous pouvons          | Y(Yes)     | Si l'utilisateur peut être un désir de             |
 |                         | utiliser, svn ainsi                   |            | désinstallation effectuée comme entrée Y.          |
 +-------------------------+---------------------------------------+------------+----------------------------------------------------+
 |Uninstall SVN? (Y/N)     | au lieu de SVN, nous pouvons          | N(No)      | Si l'utilisateur veut la désinstallation           |
 |                         | utiliser, svn ainsi                   |            | peut mettre fin à l'entrée comme N|                |
 +-------------------------+---------------------------------------+------------+----------------------------------------------------+


Si l'utilisateur procède le processus d'installation des Nations Unies, lors de l'exécution de l'installation non le processus suivant se produit:

* Lit listes de paquets.
* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Les listes des paquets qui sont automatiquement installés.
* Répertorie les paquets qui sont supprimés.
* Nombre de fichiers mis à niveau, nouvellement installés, retirés, pas mis à niveau.

Enfin, l'installation de l'ONU de SVN se rempli. La capture d'écran ci-dessous vous montre sur le processus de l'ONU d'installer SVN dans Ubuntu.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn uninstall
 Uninstall SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 [Pharaoh Logging] Removing Package subversion
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  libserf-1-1 libsvn1
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
  subversion
 0 upgraded, 0 newly installed, 1 to remove and 8 not upgraded.
 After this operation, 1,425 kB disk space will be freed.
 (Reading database ... 211322 files and directories currently installed.)
 Removing subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Removed Package subversion from the Packager Apt
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************

assurer
---------

La commande utilisée pour assurer SVN est illustré ci-dessous.

.. code-block:: bash

		ptconfigure svn ensure

Le processus d'assurer remplit les fonctions suivantes:

* Il se assurera que le module est installé ou non, et ne vérifie pas la version.
* Si le module est déjà installé, il rendra compte que ce est déjà existé.
* Si le module ne est pas disponible dans la machine de l'utilisateur, puis il procède installation.

Les captures d'écran ci-dessous illustre le processus d'assurer.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: svn: not found
 [Pharaoh Logging] Module SVN reports itself as Not Installed 
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  subversion
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 0 B/280 kB of archives.
 After this operation, 1,425 kB of additional disk space will be used.
 Selecting previously unselected package subversion.
 (Reading database ... 211282 files and directories currently installed.)
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


avantages
-----------

* Les paramètres utilisés pour déclarer l'aide et installations, désinstallation, assurez-vous ne sont pas sensible à la casse, ce qui est tout   avantage par rapport à d'autres.
* L'utilisateur peut se assurer de la disponibilité avant de poursuivre l'installation.
* Il ne sera pas écraser les paquets, il est donc moins de temps.
