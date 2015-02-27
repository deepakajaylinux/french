============
Git tools
============


synopsis
------------

Gittools est un système de contrôle de révision distribué avec un accent sur la vitesse, l'intégrité des données, et de soutien pour distribués, workflows non-linéaires.

Cette installation d'ascenseurs du module dans la version mise à jour. Lors de l'installation, il peut également installer gitfrom, noyau de git, gitcole, gitfrom sous ptconfigure. L'automatisation est possible. Il est amical avec Ubuntu et cent OS utilisateur.

Commande Aide
---------------

Cette commande d'aide à guider l'utilisateur sur ptconfigure. Ce est moins de temps, car il peut automatiquement installé. Convient à tous les types d'utilisateurs. La commande d'aide suivante aidera l'utilisateur pour l'installation des gittools. Cet argument de ligne de commande spécifie le nom de la commande à propos de laquelle l'information doit être affichée.

.. code-block:: bash

		ptconfigure gittools help

Après avoir tapé la commande, il montre l'utilisation. La capture d'écran peut exprimer la fonction de cette commande.

.. code-block:: bash

 kevell@corp:/# ptconfigure GitTools help
 ******************************


  This command allows you to install Git and a set of common Git Tools. These include
  Git - the distributed source control manager, git Core a supplement to Git, Gitk
  which is a GUI for git, and git-cola, which is also a Git GUI.

  GitTools, gittools, git-tools

        - install
        Installs the latest version of Git Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************

installation
----------------

    L'installation comprend la fourniture ou la connexion aux services nécessaires pour rendre l'équipement installé prêt à fonctionner. Ce est un processus manifeste d'installer module gittools sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash 

		ptconfigure gittools install

Après dynamiser la commande il catéchiser entrée.

L'entrée de l'utilisateur que oui il va installer automatiquement gittools avec la vérification du système. La capture d'écran suivante démontre.

.. code-block:: bash

 kevell@corp:/# ptconfigure gittools install
 Install Git Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-core from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-generic linux-image-generic
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  git-doc
 The following NEW packages will be installed:
  gitk
 0 upgraded, 1 newly installed, 0 to remove and 299 not upgraded.
 Need to get 121 kB of archives.
 After this operation, 1,250 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main gitk all 1:1.9.1-1ubuntu0.1 [121 kB]
 Fetched 121 kB in 19s (6,077 B/s)
 Selecting previously unselected package gitk.
 (Reading database ... 176395 files and directories currently installed.)
 Preparing to unpack .../gitk_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking gitk (1:1.9.1-1ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up gitk (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package gitk from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-generic linux-image-generic
 Use 'apt-get autoremove' to remove them.
 The following extra packages will be installed:
  libjs-jquery libjs-underscore
 Suggested packages:
  python-pyinotify python-simplejson javascript-common
 Recommended packages:
  xxdiff
 The following NEW packages will be installed:
  git-cola libjs-jquery libjs-underscore
 0 upgraded, 3 newly installed, 0 to remove and 299 not upgraded.
 Need to get 363 kB of archives.
 After this operation, 1,886 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-underscore all 1.4.4-2ubuntu1 [45.6 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe git-cola all 1.9.3-1 [239 kB]
 Fetched 363 kB in 1min 3s (5,679 B/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 176413 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package libjs-underscore.
 Preparing to unpack .../libjs-underscore_1.4.4-2ubuntu1_all.deb ...
 Unpacking libjs-underscore (1.4.4-2ubuntu1) ...
 Selecting previously unselected package git-cola.
 Preparing to unpack .../git-cola_1.9.3-1_all.deb ...
 Unpacking git-cola (1.9.3-1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up libjs-underscore (1.4.4-2ubuntu1) ...
 Setting up git-cola (1.9.3-1) ...
 [Pharaoh Logging] Adding Package git-cola from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitTools: Success
 ------------------------------
 Installer Finished
 ******************************

Le traitement rapide d'installation par les étapes suivantes,

Étape 1 Installez gittools? (Y / N)

Étape 2 Si l'utilisateur donne Y, le système peut vérifier la version et l'installer

Étape 3 Si l'utilisateur donne N, quitter l'installation.

Options
---------

.. cssclass:: table-bordered

 +--------------------------+---------------------------------------------+-------------+-------------------------------------------+
 | paramètres               | paramètre alternatif                        | option      | commentaires                              |
 +==========================+=============================================+=============+===========================================+
 |Install gittools?(Y/N)    | Au lieu d'utiliser gittools nous pouvons    | Y(Yes)      | Il va installer git et un ensemble de     |
 |                          | utiliser GitTools, gittools, git-tools      |             | gittools ordinaires en vertu ptconfigure. |
 +--------------------------+---------------------------------------------+-------------+-------------------------------------------+
 |Install gittools?(Y/N)    | Au lieu d'utiliser gittools nous pouvons    | N(No)       | La sortie du système d'installation       |
 |                          | utiliser GitTools, gittools, git-tools|     |             |                                           |
 +--------------------------+---------------------------------------------+-------------+-------------------------------------------+


avantages
-----------

* Gittools sont associés à des flux de travail complexes.
* Gittools fait granulaire engage plus facile que ne importe quel autre système de contrôle de version (VCS), car l'utilisateur peut déterminer 
  quels changements exactement sera dans le prochain commit.
* Gittools pour améliorer le flux de travail de codage de l'utilisateur.
* Git-cola est un outil avancé Git, similaire à git-gui commis.
* Git-cola dispose d'une visionneuse graphique, mise en scène interactive facile, soutien inotify.
