==============
Jenkins
==============

synopsis
-------------

Jenkins est populaire pour construire serveur. Jenkins est un outil d'intégration continue open source écrit en Java. Jenkins fournit des services d'intégration continue pour le développement logiciel. Il se agit d'un système en fonctionnement sur serveur dans un conteneur de servlet comme Apache Tomcat.

La fonctionnalité et la flexibilité de base de Jenkins lui permettent de se intégrer dans une variété d'environnements et peut aider à rationaliser le processus de développement pour tous les acteurs impliqués

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module Jenkins. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande.

.. code-block:: bash
             
		ptconfigure jenkins help

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash



 
 kevell@corp:/# ptconfigure jenkins help
 ******************************


 This command allows you to install Jenkins, the popular Build Server.

 Jenkins, jenkins

 - install
 Installs Jenkins through apt-get
 example: ptconfigure jenkins install

 ------------------------------
 End Help
 ******************************



installation
----------------

Si l'utilisateur doit installer le module Jenkins dans la machine, la commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
              
	        ptconfigure jenkins install


Est listé ci-dessous la capture d'écran de la commande ci-dessus,

.. code-block:: bash


 kevell@corp:/# ptconfigure jenkins install

 Install Jenkins? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Jenkins !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-82538719911.sh
 chmod 755 /tmp/ptconfigure-temp-script-82538719911.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-82538719911.sh Permissions
 Executing /tmp/ptconfigure-temp-script-82538719911.sh
 OK
 Ign http://dl.google.com stable InRelease
 Hit http://dl.google.com stable Release.gpg
 Hit http://dl.google.com stable Release
 Hit http://dl.google.com stable/main amd64 Packages
 Hit http://dl.google.com stable/main i386 Packages
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Ign http://in.archive.ubuntu.com trusty InRelease
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://security.ubuntu.com trusty-security InRelease
 Hit http://downloads.hipchat.com stable InRelease
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Hit http://extras.ubuntu.com trusty Release.gpg
 Ign http://packages.elasticsearch.org stable InRelease
 Get:1 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Ign http://dl.google.com stable/main Translation-en_IN
 Hit http://downloads.hipchat.com stable/main amd64 Packages
 Ign http://dl.google.com stable/main Translation-en
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Ign http://repos.zend.com server InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Get:2 http://security.ubuntu.com trusty-security Release [63.5 kB]
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://extras.ubuntu.com trusty Release
 Hit http://downloads.hipchat.com stable/main i386 Packages
 Ign http://archive.canonical.com trusty InRelease
 Hit http://repos.zend.com server Release.gpg
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://repos.zend.com server Release
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://pkg.jenkins-ci.org binary/ Release
 Get:3 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://archive.canonical.com trusty Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://repos.zend.com server/non-free amd64 Packages
 Hit http://packages.elasticsearch.org stable Release
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Hit http://repos.zend.com server/non-free i386 Packages
 Hit http://archive.canonical.com trusty Release
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Hit http://in.archive.ubuntu.com trusty Release
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty Release
 Hit http://archive.canonical.com trusty/partner amd64 Packages
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Get:4 http://in.archive.ubuntu.com trusty-updates Release [63.5 kB]
 Hit http://ppa.launchpad.net trusty Release
 Hit http://archive.canonical.com trusty/partner i386 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Get:5 http://security.ubuntu.com trusty-security/main Sources [76.1 kB]
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Ign http://archive.canonical.com trusty/partner Translation-en
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Ign http://downloads.hipchat.com stable/main Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Ign http://downloads.hipchat.com stable/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Get:6 http://security.ubuntu.com trusty-security/restricted Sources [2,061 B]
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Get:7 http://security.ubuntu.com trusty-security/universe Sources [18.0 kB]
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Ign http://repos.zend.com server/non-free Translation-en_IN
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Ign http://repos.zend.com server/non-free Translation-en
 Get:8 http://security.ubuntu.com trusty-security/multiverse Sources [1,905 B]
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Get:9 http://security.ubuntu.com trusty-security/main amd64 Packages [251 kB]
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Get:10 http://in.archive.ubuntu.com trusty-updates/main Sources [189 kB]
 Ign https://repo.varnish-cache.org precise InRelease
 Get:11 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Get:12 http://security.ubuntu.com trusty-security/universe amd64 Packages [89.7 kB]
 Get:13 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [3,459 B]
 Get:14 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2,564 B]
 Get:15 http://security.ubuntu.com trusty-security/main i386 Packages [242 kB]
 Get:16 http://in.archive.ubuntu.com trusty-updates/universe Sources [107 kB]
 Get:17 https://repo.varnish-cache.org precise Release.gpg
 Hit https://repo.varnish-cache.org precise Release
 Hit https://repo.varnish-cache.org precise/varnish-4.0 amd64 Packages
 Hit https://repo.varnish-cache.org precise/varnish-4.0 i386 Packages
 Get:18 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [4,765 B]
 Get:19 https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN
 Get:20 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [489 kB]
 Get:21 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:22 http://security.ubuntu.com trusty-security/universe i386 Packages [89.7 kB]
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en
 Get:23 http://security.ubuntu.com trusty-security/multiverse i386 Packages [3,628 B]
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Get:24 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B]
 Get:25 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [260 kB]
 Get:26 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.7 kB]
 Get:27 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [478 kB]
 Get:28 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B]
 Get:29 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [262 kB]
 Get:30 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.9 kB]
 Hit http://in.archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/main Sources
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Sources
 Hit http://in.archive.ubuntu.com trusty-backports/universe Sources
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Sources
 Hit http://in.archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/universe Translation-en
 Ign http://in.archive.ubuntu.com trusty/main Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/universe Translation-en_IN
 Fetched 2,760 kB in 1min 18s (35.4 kB/s)
 Reading package lists...
 Temp File /tmp/ptconfigure-temp-script-82538719911.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   daemon
 The following NEW packages will be installed:
   daemon jenkins
 0 upgraded, 2 newly installed, 0 to remove and 96 not upgraded.
 Need to get 60.1 MB of archives.
 After this operation, 69.4 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe daemon amd64 0.6.4-1 [98.2 kB]
 Get:2 http://pkg.jenkins-ci.org/debian/ binary/ jenkins 1.607 [60.0 MB]
 Fetched 60.1 MB in 18min 15s (54.9 kB/s)
 Selecting previously unselected package daemon.
 (Reading database ... 198135 files and directories currently installed.)
 Preparing to unpack .../daemon_0.6.4-1_amd64.deb ...
 Unpacking daemon (0.6.4-1) ...
 Selecting previously unselected package jenkins.
 Preparing to unpack .../archives/jenkins_1.607_all.deb ...
 Unpacking jenkins (1.607) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Setting up daemon (0.6.4-1) ...
 Setting up jenkins (1.607) ...
  * Starting Jenkins Continuous Integration Server jenkins
   ...done.
 Processing triggers for ureadahead (0.100.0-16) ...
 [Pharaoh Logging] Adding Package jenkins from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 Jenkins: Success
 ------------------------------
 Installer Finished
 ******************************


options
-----------

.. cssclass:: table-bordered

 +----------------------------+--------------------------------------+------------+-------------------------------------------------+
 | Paramètres                 | alternative paramètres               | Option     | Commentaires                                    |
 +============================+======================================+============+=================================================+
 |ptconfigure Jenkins Install | Au lieu d'utiliser Jenkins,          | Y(Yes)     | Une fois que l'utilisateur fournit l'option,    |
 |                            | l'utilisateur peut ajouter jenkins   |            | système démarre processus d'installation        |
 +----------------------------+--------------------------------------+------------+-------------------------------------------------+
 |ptconfigure Jenkins Install | Au lieu d'utiliser Jenkins,          | N(No)      | Une fois que l'utilisateur fournit l'option,    |
 |                            | l'utilisateur peut ajouter jenkins   |            | le système se arrête processus d'installation|  |
 +----------------------------+--------------------------------------+------------+-------------------------------------------------+


avantages
--------------

* Détection de bug immédiate
* Aucune étape d'intégration dans le cycle de vie
* Un système déployable à un moment donné
* Enregistrement de l'évolution du projet
