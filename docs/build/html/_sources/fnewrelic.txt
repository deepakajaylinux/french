=========
Newrelic
=========

Synopsis
----------------

Newrelic utilisé pour surveiller le serveur. La collaboration entre les différents rôles offre de nombreux avantages. La combinaison d'une base de code commune, intégration continue, techniques test-driven et déploie automatisés, entre autres choses, exposer les problèmes, dans le code l'application, de l'infrastructure ou de la configuration, plus tôt parce que le logiciel ne est pas «jeté sur le mur" pour des opérations à l'extrémité de codage. Déploiements automatisés et des environnements de production standardisés, les principaux aspects de DevOps, font déploiements prévisible et libérer les gens de tâches routinières et répétitives pour aller faire des choses plus créatives. Le newrelic est à l'aise avec Ubuntu et cent OS.

commande Aide
----------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules newrelic. Les listes de commandes de l'aide sur les autres paramètres de newrelic sous module de ptconfigure. Il décrit également la syntaxe pour détecter la machine de l'utilisateur. La commande d'aide pour newrelic est illustré ci-dessous.

.. code-block:: bash

		ptconfigure newrelic help

La syntaxe de la non cas de commande d'aide sensible qui ajoute un avantage pour ce module. Visualiser l'utilisateur sur la commande d'aide en vertu newrelic La capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptconfigure NewRelic help
 ******************************

  This command allows you to update Newrelic.
   NewRelic, newrelic, Newrelic

  - install
  Installs the latest version of ptconfigure
  example: ptconfigure newrelic install

 ------------------------------
 End Help
 ******************************


installation
-------------------

Ces procédures d'installation sont pour les administrateurs système. Cette section fournit des informations sur la compatibilité et les exigences, instructions de base sur la façon d'installer et configurer ptconfigure à l'information plus détaillée.

Avant l'installation, l'utilisateur doit suivre:

1. Assurez-vous que votre système répond aux exigences de compatibilité et PHP de New Relic.

2. Si vous ne possédez pas déjà un compte New Relic, en créer un.

3. De nouveaux paramètres de votre compte Relic, copiez votre clé d'.

4. Suivez les procédures d'installation de l'agent à la fois pour l'extension PHP et le démon de proxy local.

5. Remplissez les paramètres de configuration de l'agent et éventuellement le démon proxy.

6. Modifiez le nom de l'application par défaut à un nom significatif.

7. votre programme d'accueil de PHP (comme php-fpm) le cas échéant Redémarrer Apache ou.

8. Si aucune donnée ne apparaît après quelques minutes, voir Dépannage de votre installation.

.. code-block:: bash



 kevell@corp:/# ptconfigure newrelic install
 Install NewRelic? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         NewRelic!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-55665166254.sh
 chmod 755 /tmp/ptconfigure-temp-script-55665166254.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-55665166254.sh Permissions
 Executing /tmp/ptconfigure-temp-script-55665166254.sh
 --2015-03-30 16:36:51--  https://download.newrelic.com/548C16BF.gpg
 Resolving download.newrelic.com (download.newrelic.com)... 50.31.164.159
 Connecting to download.newrelic.com (download.newrelic.com)|50.31.164.159|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 1682 (1.6K) [application/octet-stream]
 Saving to: â€˜STDOUTâ€™
 
 100%[=======================================================================================================>] 1,682       --.-K/s   in 0s      

 2015-03-30 16:36:55 (5.96 MB/s) - written to stdout [1682/1682]
 OK
 Ign http://dl.google.com stable InRelease
 Hit http://downloads.hipchat.com stable InRelease
 Ign http://archive.ubuntu.com trusty InRelease
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://extras.ubuntu.com precise InRelease
 Ign http://us.archive.ubuntu.com precise InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://archive.ubuntu.com trusty-updates InRelease
 Hit http://security.ubuntu.com trusty-security Release.gpg
 Ign http://us.archive.ubuntu.com precise-security InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Get:1 http://extras.ubuntu.com precise Release.gpg [72 B]
 Ign http://packages.dotdeb.org squeeze InRelease
 Hit http://downloads.hipchat.com stable/main amd64 Packages
 Ign http://archive.ubuntu.com trusty-proposed InRelease
 Ign http://us.archive.ubuntu.com precise-updates InRelease
 Hit http://security.ubuntu.com trusty-security Release
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://extras.ubuntu.com precise Release
 Get:2 http://dl.hhvm.com trusty InRelease [2,104 B]
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Ign http://us.archive.ubuntu.com precise-backports InRelease
 Ign http://archive.ubuntu.com trusty-backports InRelease
 Hit http://downloads.hipchat.com stable/main i386 Packages
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://security.ubuntu.com trusty-security/universe amd64 Packages
 Hit http://packages.dotdeb.org squeeze Release
 Hit http://us.archive.ubuntu.com precise Release.gpg
 Hit http://archive.ubuntu.com trusty Release.gpg
 Hit http://extras.ubuntu.com precise/main Sources
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://security.ubuntu.com trusty-security/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise-security Release.gpg
 Hit http://extras.ubuntu.com precise/main amd64 Packages
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://security.ubuntu.com trusty-security/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-updates Release.gpg
 Hit http://extras.ubuntu.com precise/main i386 Packages
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Hit http://packages.elasticsearch.org stable Release
 Hit http://security.ubuntu.com trusty-security/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports Release.gpg
 Get:3 http://archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://security.ubuntu.com trusty-security/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise Release
 Hit http://packages.elasticsearch.org stable Release
 Hit http://archive.ubuntu.com trusty-proposed Release.gpg
 Hit http://security.ubuntu.com trusty-security/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise-security Release
 Hit http://packages.elasticsearch.org stable Release
 Hit http://archive.ubuntu.com trusty-backports Release.gpg
 Ign http://archive.canonical.com precise InRelease
 Hit http://security.ubuntu.com trusty-security/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates Release
 Hit http://archive.ubuntu.com trusty Release
 Hit http://security.ubuntu.com trusty-security/main i386 Packages
 Hit http://archive.canonical.com precise Release.gpg
 Hit http://us.archive.ubuntu.com precise-backports Release
 Hit http://mirror.stshosting.co.uk precise InRelease
 Get:4 http://archive.ubuntu.com trusty-updates Release [63.5 kB]
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://us.archive.ubuntu.com precise/main Sources
 Hit http://archive.canonical.com precise Release
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise/restricted Sources
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://us.archive.ubuntu.com precise/universe Sources
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise/multiverse Sources
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Hit http://us.archive.ubuntu.com precise/main amd64 Packages
 Hit http://archive.canonical.com precise/partner Sources
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://us.archive.ubuntu.com precise/restricted amd64 Packages
 Ign http://downloads-distro.mongodb.org dist InRelease
 Ign http://extras.ubuntu.com precise/main Translation-en_IN
 Hit http://archive.canonical.com precise/partner amd64 Packages
 Hit http://us.archive.ubuntu.com precise/universe amd64 Packages
 Ign http://extras.ubuntu.com precise/main Translation-en
 Hit http://archive.canonical.com precise/partner i386 Packages
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://archive.canonical.com precise/partner Translation-en
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Get:5 http://oss.oracle.com unstable InRelease
 Ign http://oss.oracle.com unstable InRelease
 Hit http://us.archive.ubuntu.com precise/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise/main i386 Packages
 Hit http://us.archive.ubuntu.com precise/restricted i386 Packages
 Hit http://repo.mysql.com trusty InRelease
 Hit http://us.archive.ubuntu.com precise/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise/multiverse i386 Packages
 Hit http://oss.oracle.com unstable Release
 Ign http://oss.oracle.com unstable Release
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Ign http://apt.newrelic.com newrelic InRelease
 Hit http://us.archive.ubuntu.com precise/main Translation-en
 Ign http://downloads.hipchat.com stable/main Translation-en_IN
 Get:6 http://oss.oracle.com unstable/main amd64 Packages
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://dl.google.com stable Release.gpg
 Hit http://us.archive.ubuntu.com precise/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise/restricted Translation-en
 Ign http://oss.oracle.com unstable/main i386 Packages/DiffIndex
 Hit http://us.archive.ubuntu.com precise/universe Translation-en
 Hit http://us.archive.ubuntu.com precise-security/main Sources
 Ign http://oss.oracle.com unstable/non-free i386 Packages/DiffIndex
 Hit http://us.archive.ubuntu.com precise-security/restricted Sources
 Hit http://us.archive.ubuntu.com precise-security/universe Sources
 Hit http://us.archive.ubuntu.com precise-security/multiverse Sources
 Hit http://us.archive.ubuntu.com precise-security/main amd64 Packages
 Get:7 http://www.apache.org 21x InRelease [3,167 B]
 Hit http://us.archive.ubuntu.com precise-security/restricted amd64 Packages
 Ign http://downloads.hipchat.com stable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-security/universe amd64 Packages
 Hit http://us.archive.ubuntu.com precise-security/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-security/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/multiverse i386 Packages
 Hit http://oss.oracle.com unstable/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/main Translation-en
 Hit http://oss.oracle.com unstable/non-free i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/multiverse Translation-en
 Get:8 http://oss.oracle.com unstable/main Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-security/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-security/universe Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/main Sources
 Hit http://us.archive.ubuntu.com precise-updates/restricted Sources
 Hit http://us.archive.ubuntu.com precise-updates/universe Sources
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-updates/multiverse Sources
 Hit http://us.archive.ubuntu.com precise-updates/main amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/restricted amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-updates/universe amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/multiverse amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Get:9 http://dl.hhvm.com trusty/main amd64 Packages [1,686 B]
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/main i386 Packages
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/multiverse Translation-en
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Hit http://us.archive.ubuntu.com precise-updates/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/universe Translation-en
 Hit http://mirror.stshosting.co.uk precise/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/main Sources
 Hit http://mirror.stshosting.co.uk precise/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/restricted Sources
 Err http://oss.oracle.com unstable/main amd64 Packages
   HttpError404
 Hit http://us.archive.ubuntu.com precise-backports/universe Sources
 Err http://oss.oracle.com unstable/non-free amd64 Packages
   HttpError404
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Sources
 Ign http://oss.oracle.com unstable/main Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-backports/main amd64 Packages
 Hit http://downloads-distro.mongodb.org dist Release.gpg
 Ign http://oss.oracle.com unstable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe amd64 Packages
 Ign http://oss.oracle.com unstable/non-free Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-backports/multiverse amd64 Packages
 Ign http://oss.oracle.com unstable/non-free Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/main i386 Packages
 Hit http://repo.mysql.com trusty/mysql-5.6 Sources
 Hit http://us.archive.ubuntu.com precise-backports/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed Release
 Hit http://us.archive.ubuntu.com precise-backports/main Translation-en
 Hit http://archive.ubuntu.com trusty-backports Release
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty/main Sources
 Hit http://us.archive.ubuntu.com precise-backports/restricted Translation-en
 Hit http://archive.ubuntu.com trusty/universe Sources
 Hit http://repo.mysql.com trusty/mysql-5.6 amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe Translation-en
 Hit http://archive.ubuntu.com trusty/restricted Sources
 Hit http://repo.mysql.com trusty/mysql-5.6 i386 Packages
 Hit http://archive.ubuntu.com trusty/multiverse Sources
 Hit http://archive.ubuntu.com trusty/main amd64 Packages
 Hit http://archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty/main i386 Packages
 Hit http://archive.ubuntu.com trusty/universe i386 Packages
 Hit http://archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty/main Translation-en
 Ign http://us.archive.ubuntu.com precise/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty/multiverse Translation-en
 Ign http://us.archive.ubuntu.com precise/multiverse Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/restricted Translation-en_IN
 Hit http://archive.ubuntu.com trusty/restricted Translation-en
 Ign http://us.archive.ubuntu.com precise/universe Translation-en_IN
 Hit http://archive.ubuntu.com trusty/universe Translation-en
 Hit http://apt.newrelic.com newrelic Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Get:10 http://archive.ubuntu.com trusty-updates/universe amd64 Packages [261 kB]
 Hit http://dl.google.com stable Release
 Get:11 http://www.apache.org 21x/main amd64 Packages [698 B]
 Get:12 http://www.apache.org 21x/main i386 Packages [698 B]
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://downloads-distro.mongodb.org dist Release
 Hit http://apt.newrelic.com newrelic Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://dl.google.com stable/main amd64 Packages
 Hit http://dl.google.com stable/main i386 Packages
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://downloads-distro.mongodb.org dist/10gen amd64 Packages
 Hit http://downloads-distro.mongodb.org dist/10gen i386 Packages
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Get:13 http://archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B]
 Get:14 http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.7 kB]
 Get:15 http://archive.ubuntu.com trusty-updates/main amd64 Packages [488 kB]
 Ign http://dl.hhvm.com trusty/main Translation-en_IN
 Ign http://dl.hhvm.com trusty/main Translation-en
 Ign http://mirror.stshosting.co.uk precise/main Translation-en_IN
 Ign http://mirror.stshosting.co.uk precise/main Translation-en
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en_IN
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en
 Ign http://www.apache.org 21x/main Translation-en_IN
 Ign http://www.apache.org 21x/main Translation-en
 Ign http://dl.google.com stable/main Translation-en_IN
 Ign http://dl.google.com stable/main Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en_IN
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en
 Ign http://apt.newrelic.com newrelic/non-free Translation-en_IN
 Ign http://apt.newrelic.com newrelic/non-free Translation-en
 Get:16 http://archive.ubuntu.com trusty-updates/universe i386 Packages [261 kB]
 Get:17 http://archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B]
 Get:18 http://archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.9 kB]
 Get:19 http://archive.ubuntu.com trusty-updates/main i386 Packages [477 kB]
 Hit http://archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty-proposed/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty-proposed/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty-proposed/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-proposed/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed/main i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed/main Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/universe Translation-en
 Hit http://archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/main i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-backports/universe Translation-en
 Ign http://archive.ubuntu.com trusty/main Translation-en_IN
 Ign http://archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://archive.ubuntu.com trusty/universe Translation-en_IN
 Fetched 1,602 kB in 3min 28s (7,665 B/s)
 Temp File /tmp/ptconfigure-temp-script-55665166254.sh Removed
 [Pharaoh Logging] Package newrelic-sysmond from the Packager Apt is already installed, so not installing
 Enter Your Licence Key:
 e1686c78ccc839ce4941916812c625760cc0070b
 Creating /tmp/ptconfigure-temp-script-7830870709.sh
 chmod 755 /tmp/ptconfigure-temp-script-7830870709.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-7830870709.sh Permissions
 Executing /tmp/ptconfigure-temp-script-7830870709.sh
 New Relic Server Monitor: newrelic-sysmond already running
 Temp File /tmp/ptconfigure-temp-script-7830870709.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 
 
 Single App Installer:
 --------------------------------------------
 NewRelic: Success
 ------------------------------
 Installer Finished
 ******************************







Options
---------------

.. cssclass:: table-bordered


 +-------------------------+-------------------------------------------------+--------------+------------------------------------------+
 | paramètres              | paramètre alternatif                            | option       | commentaires                             |
 +=========================+=================================================+==============+==========================================+
 |Install newrelic?(Y/N)   | Au lieu d'utiliser newrelic l'utilisateur peut  | Y(Yes)       | Il commence à installer newrelic         |
 |                         | utiliser NewRellic, Newrelic                    |              | sous ptconfigure                         |
 +-------------------------+-------------------------------------------------+--------------+------------------------------------------+
 |Install newrelic?(Y/N)   | Au lieu d'utiliser newrelic l'utilisateur peut  | N(No)        | Il termine l'installation                |
 |                         | utiliser NewRellic, Newrelic|                   |              |                                          |
 +-------------------------+-------------------------------------------------+--------------+------------------------------------------+


avantages
-------------

Les avantages techniques
----------------------------

* Livraison de logiciels continue
* Problèmes moins complexes pour fixer
* Résolution plus rapide des problèmes
* Comforts avec Ubuntu et CentOS
* Sensibilité non de cas


Avantages pour l'entreprise
-----------------------------

* Livraison rapide de fonctionnalités
* Environnements d'exploitation plus stables
* Plus de temps pour ajouter de la valeur (plutôt que de fixer / maintenir)
