=============
Gitbucket
=============

Synopsis
-------------

Git est un système de contrôle de révision distribué avec un accent sur la vitesse, l'intégrité des données et de soutien pour distribués, workflows non-linéaires. Git est le système de contrôle de version largement adoptée pour le développement de logiciels.

Répertoire de travail Git est un référentiel à part entière avec l'histoire complète et toutes les capacités de la version de suivi, indépendants de l'accès au réseau ou un serveur central.

GitBucket est le clone Github facilement installable écrit avec Scala. Il fournit une des caractéristiques de base ci-dessous:

* Git publique / privée référentiel (accès http seulement)
* Dépôt spectateur (certaines fonctionnalités avancées telles que l'édition de fichiers en ligne ne sont pas mises en œuvre)
* Recherche Repository (Code et questions)
* Wiki
* Questions
* Fork / demande de Pull
* Mail notification
* Calendrier des activités
* Gestion des utilisateurs (pour les administrateurs)
* Groupe (comme Organisation Github)
* Intégration LDAP
* Soutien Gravatar
* Fichier exécutable de guerre


Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de gitbucket. L'utilisateur se agit de connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
     
                ptconfigure gitbucket help

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/$ ptconfigure gitbucket help
 ******************************
  This command allows you to install a full Git Bucket installation on to a server
  The dependencies for GitBucket are also installed.

  GitBucket, gitbucket, git-bucket

        - install
        Installs the latest version of GitBucket on a system
        example: ptconfigure gitbucket install

 ------------------------------
 End Help
 ******************************

installation
----------------

Lorsque l'utilisateur doit installer le module de gitbucket dans la machine. La commande ci-dessous donnée exécuter le processus d'installation.
Lors de l'installation, le système demande pour le répertoire racine du référentiel. L'utilisateur doit définir le chemin. Il n'y a pas de répertoire par défaut.

.. code-block:: bash
       
                ptconfigure gitbucket install

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/$ ptconfigure gitbucket install
 Install Git Bucket? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !GitBucket!        *
 *******************************
 PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/GitBucket/Model/GitBucketUbuntu.php on line 67
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Command 'git' found
 [Pharaoh Logging] No command 'gitk' found
 [Pharaoh Logging] No command 'git-cola' found
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/AppConfig.php on line 115
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  git-core
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 1,458 B of archives.
 After this operation, 21.5 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main git-core all 1:1.9.1-1ubuntu0.1 [1,458 B]
 Fetched 1,458 B in 1s (783 B/s)
 Selecting previously unselected package git-core.
 (Reading database ... 182763 files and directories currently installed.)
 Preparing to unpack .../git-core_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking git-core (1:1.9.1-1ubuntu0.1) ...
 Setting up git-core (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package git-core from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/AppConfig.php on line 115
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  git-doc
 The following NEW packages will be installed:
  gitk
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 121 kB of archives.
 After this operation, 1,250 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main gitk all 1:1.9.1-1ubuntu0.1 [121 kB]
 Fetched 121 kB in 2s (43.1 kB/s)
 Selecting previously unselected package gitk.
 (Reading database ... 182764 files and directories currently installed.)
 Preparing to unpack .../gitk_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking gitk (1:1.9.1-1ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up gitk (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package gitk from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/AppConfig.php on line 115
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libjs-jquery libjs-underscore
 Suggested packages:
  python-pyinotify python-simplejson javascript-common
 Recommended packages:
  xxdiff
 The following NEW packages will be installed:
  git-cola libjs-jquery libjs-underscore
 0 upgraded, 3 newly installed, 0 to remove and 301 not upgraded.
 Need to get 363 kB of archives.
 After this operation, 1,886 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-underscore all 1.4.4-2ubuntu1 [45.6 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe git-cola all 1.9.3-1 [239 kB]
 Fetched 363 kB in 13s (27.8 kB/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 182782 files and directories currently installed.)
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
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/AppConfig.php on line 115
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-15361773074.sh
 chmod 755 /tmp/ptconfigure-temp-script-15361773074.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-15361773074.sh Permissions
 Executing /tmp/ptconfigure-temp-script-15361773074.sh
 Cloning into 'gitbucket-war'...
 remote: Counting objects: 8, done.
 remote: Total 8 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (8/8), done.
 Checking connectivity... done.
 mkdir: cannot create directory ‘/opt/gitbucket/’: Permission denied
 mv: target ‘/opt/gitbucket/’ is not a directory
 Temp File /tmp/ptconfigure-temp-script-15361773074.sh Removed
 Enter Repository Root Directory:
 /
 Program Executor Deleted if existed
 PHP Warning:  file_put_contents(/usr/bin/gitbucket): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 312
 chmod: cannot access ‘/usr/bin/gitbucket’: No such file or directory
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 GitBucket: Success
 ------------------------------
 Installer Finished
 ******************************

Options
----------

.. cssclass:: table-bordered

 +--------------------------+-----------------------------------+------------+--------------------------------------+
 | Paramètres               | paramètre alternatif              | option     | Commentaire                          |
 +==========================+===================================+============+======================================+
 |ptconfigure gitbucket     | GitBucket, gitbucket, git-bucket  | Y          | Le système démarre processus         |
 |Install                   |                                   |            | d'installation                       |
 +--------------------------+-----------------------------------+------------+--------------------------------------+
 |ptconfigure gitbucket     | GitBucket, gitbucket, git-bucket  | N          | Système arrête l'installation        |
 |Install|                  |                                   |            |                                      |
 +--------------------------+-----------------------------------+------------+--------------------------------------+

avantages
--------------

* Git soutient branchement rapide et fusion, et inclut des outils spécifiques pour la visualisation et la navigation une histoire de 
  développement non-linéaire.
* Dépôts peuvent être publiés via HTTP, FTP, rsync ou un protocole de Git plus soit une prise ordinaire, ou ssh.
* Git décrit comme étant très rapide, évolutive et a montré que ce était un ordre de grandeur plus rapide que certains systèmes de contrôle de 
  version, et aller chercher historique des versions d'un référentiel stocké localement peut être cent fois plus rapide que la récupération à 
  partir du serveur distant.
* Les mots clés sont changelogs hyperlien vers les pages des numéros correspondants, Tirez Demandes pages et des pages Wiki.
* L'ensemble du changement et diff dans les journaux de modifications sont un hyperlien vers GitBucket référentiel spectateur.
* Déclencher une accumulation lorsqu'un changement est poussé à l'aide d'un GitBucket WebHook.
