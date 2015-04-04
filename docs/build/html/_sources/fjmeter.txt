=======
Jmeter
=======

synopsis
------------

Ce module traite de l'installation du jmeter avec la version mise à jour. JMeter peut être utilisé comme un outil de test unitaire pour les connexions de base de données JDBC, FTP, LDAP, les services Web, JMS, HTTP, les connexions TCP génériques et les processus autochtones OS. Voyons comment ce module permet à l'utilisateur dans l'installation et l'utilisation du Jmeter.

Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module Jmeter. Il énumère les autres paramètres du module de jmeter. Il décrit également la syntaxe pour l'installation du module de jmeter. La commande d'aide pour le module de jmeter est représentée ci-dessous.

.. code-block:: bash

		ptconfigure Jmeter help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu Jmeter.

.. code-block:: bash

 kevell@corp:/# ptconfigure Jmeter help

 ******************************


  This command allows you to update Jmeter.

  Jmeter, jmeter

        - install
        Installs the latest version of Jmeter
        example: ptconfigure jmeter install

 ------------------------------
 End Help
 ******************************


installation
----------------

La commande utilisée pour installer le jmeter dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash

		ptconfigure jmeter install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered


 +----------------------+-----------------------------------------+-----------+--------------------------------------------------+
 | Paramètres           | Alternative paramètres                  | Option    | Commentaires                                     |
 +======================+=========================================+===========+==================================================+
 |Install Jmeter? (Y/N) | Au lieu de jmeter, nous pouvons         | Y(Yes)    | Si l'utilisateur souhaite procéder le processus  |
 |                      | utiliser Jmeter également.              |           | d'installation qu'ils peuvent entrée comme Y.    |
 +----------------------+-----------------------------------------+-----------+--------------------------------------------------+
 |Install Jmeter? (Y/N) | Au lieu de jmeter, nous pouvons         | N(No)     | Si l'utilisateur souhaite quitter le processus   |
 |                      | utiliser Jmeter également.              |           | d'installation qu'ils peuvent entrée comme N.|   |
 +----------------------+-----------------------------------------+-----------+--------------------------------------------------+


Si l'utilisateur procède à l'installation, au cours du processus d'installation est décrite dans les listes ci-dessous:


* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les paquets qui sont automatiquement installés.
* Liste outs les nouveaux paquets qui installent.
* Détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.
* Lit les listes de paquets et affiche la liste des paquets qui sont déjà installé.


Représente imagée L'écran suivant le processus décrit ci-dessus de l'installation.


.. code-block:: bash

 kevell@corp:/# ptconfigure Jmeter install
 Install Jmeter? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Jmeter        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-51122634115.sh
 chmod 755 /tmp/ptconfigure-temp-script-51122634115.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-51122634115.sh Permissions
 Executing /tmp/ptconfigure-temp-script-51122634115.sh
 Ign http://dl.google.com stable InRelease
 Ign http://packages.dotdeb.org squeeze InRelease
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://archive.canonical.com precise InRelease
 Ign http://archive.ubuntu.com trusty InRelease
 Hit http://downloads.hipchat.com stable InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Get:1 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Ign http://us.archive.ubuntu.com precise InRelease
 Ign http://extras.ubuntu.com precise InRelease
 Ign http://archive.ubuntu.com trusty-updates InRelease
 Hit http://dl.hhvm.com trusty InRelease
 Hit http://archive.canonical.com precise Release.gpg
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://packages.dotdeb.org squeeze Release
 Get:2 http://security.ubuntu.com trusty-security Release [63.5 kB]
 Ign http://us.archive.ubuntu.com precise-security InRelease
 Hit http://downloads.hipchat.com stable/main amd64 Packages
 Hit http://extras.ubuntu.com precise Release.gpg
 Ign http://archive.ubuntu.com trusty-proposed InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://archive.canonical.com precise Release
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Ign http://us.archive.ubuntu.com precise-updates InRelease
 Hit http://downloads.hipchat.com stable/main i386 Packages
 Hit http://extras.ubuntu.com precise Release
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Hit http://packages.elasticsearch.org stable Release.gpg
 Ign http://archive.ubuntu.com trusty-backports InRelease
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Ign http://us.archive.ubuntu.com precise-backports InRelease
 Hit http://archive.canonical.com precise/partner Sources
 Hit http://extras.ubuntu.com precise/main Sources
 Hit http://packages.elasticsearch.org stable Release.gpg
 Get:3 http://security.ubuntu.com trusty-security/universe amd64 Packages [91.6 kB]
 Hit http://archive.ubuntu.com trusty Release.gpg
 Hit http://us.archive.ubuntu.com precise Release.gpg
 Hit http://archive.canonical.com precise/partner amd64 Packages
 Hit http://extras.ubuntu.com precise/main amd64 Packages
 Hit http://mirror.stshosting.co.uk precise InRelease
 Hit http://packages.elasticsearch.org stable Release.gpg
 Get:4 http://us.archive.ubuntu.com precise-security Release.gpg [198 B]
 Get:5 http://archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://archive.canonical.com precise/partner i386 Packages
 Hit http://packages.elasticsearch.org stable Release
 Hit http://extras.ubuntu.com precise/main i386 Packages
 Get:6 http://us.archive.ubuntu.com precise-updates Release.gpg [198 B]
 Get:7 http://archive.ubuntu.com trusty-proposed Release.gpg [933 B]
 Get:8 http://oss.oracle.com unstable InRelease
 Ign http://oss.oracle.com unstable InRelease
 Hit http://packages.elasticsearch.org stable Release
 Get:9 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Hit http://us.archive.ubuntu.com precise-backports Release.gpg
 Ign http://downloads-distro.mongodb.org dist InRelease
 Hit http://archive.ubuntu.com trusty-backports Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Get:10 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [3,459 B]
 Hit http://us.archive.ubuntu.com precise Release
 Hit http://archive.ubuntu.com trusty Release
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Get:11 http://security.ubuntu.com trusty-security/main amd64 Packages [251 kB]
 Get:12 http://us.archive.ubuntu.com precise-security Release [54.3 kB]
 Get:13 http://archive.ubuntu.com trusty-updates Release [63.5 kB]
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://oss.oracle.com unstable Release
 Ign http://oss.oracle.com unstable Release
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Ign http://archive.canonical.com precise/partner Translation-en
 Ign http://downloads.hipchat.com stable/main Translation-en_IN
 Get:14 http://us.archive.ubuntu.com precise-updates Release [196 kB]
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Get:15 http://oss.oracle.com unstable/main amd64 Packages
 Ign http://downloads.hipchat.com stable/main Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Get:16 http://security.ubuntu.com trusty-security/universe i386 Packages [91.5 kB]
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://oss.oracle.com unstable/main i386 Packages/DiffIndex
 Ign http://oss.oracle.com unstable/non-free i386 Packages/DiffIndex
 Ign http://extras.ubuntu.com precise/main Translation-en_IN
 Get:17 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:18 http://archive.ubuntu.com trusty-proposed Release [211 kB]
 Ign http://extras.ubuntu.com precise/main Translation-en
 Hit http://us.archive.ubuntu.com precise-backports Release
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Get:19 http://security.ubuntu.com trusty-security/multiverse i386 Packages [3,628 B]
 Hit http://us.archive.ubuntu.com precise/main Sources
 Get:20 http://security.ubuntu.com trusty-security/main i386 Packages [242 kB]
 Hit http://us.archive.ubuntu.com precise/restricted Sources
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://us.archive.ubuntu.com precise/universe Sources
 Hit http://repo.mysql.com trusty InRelease
 Hit http://us.archive.ubuntu.com precise/multiverse Sources
 Hit http://us.archive.ubuntu.com precise/main amd64 Packages
 Hit http://oss.oracle.com unstable/main i386 Packages
 Ign http://apt.newrelic.com newrelic InRelease
 Hit http://us.archive.ubuntu.com precise/restricted amd64 Packages
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://oss.oracle.com unstable/non-free i386 Packages
 Hit http://us.archive.ubuntu.com precise/universe amd64 Packages
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Get:21 http://oss.oracle.com unstable/main Translation-en_IN
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise/multiverse amd64 Packages
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://dl.google.com stable Release.gpg
 Hit http://us.archive.ubuntu.com precise/main i386 Packages
 Hit http://us.archive.ubuntu.com precise/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise/universe i386 Packages
 Hit http://dl.hhvm.com trusty/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise/multiverse i386 Packages
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Hit http://archive.ubuntu.com trusty-backports Release
 Hit http://archive.ubuntu.com trusty/main Sources
 Hit http://us.archive.ubuntu.com precise/main Translation-en
 Hit http://archive.ubuntu.com trusty/universe Sources
 Hit http://archive.ubuntu.com trusty/restricted Sources
 Hit http://us.archive.ubuntu.com precise/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty/multiverse Sources
 Get:22 http://www.apache.org 21x InRelease [3,167 B]
 Hit http://archive.ubuntu.com trusty/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise/restricted Translation-en
 Hit http://archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Hit http://archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise/universe Translation-en
 Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages
 Get:23 http://us.archive.ubuntu.com precise-security/main Sources [125 kB]
 Hit http://archive.ubuntu.com trusty/main i386 Packages
 Hit http://mirror.stshosting.co.uk precise/main amd64 Packages
 Hit http://mirror.stshosting.co.uk precise/main i386 Packages
 Hit http://archive.ubuntu.com trusty/universe i386 Packages
 Hit http://archive.ubuntu.com trusty/restricted i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty/multiverse i386 Packages
 Get:24 http://us.archive.ubuntu.com precise-security/restricted Sources [3,759 B]
 Err http://oss.oracle.com unstable/main amd64 Packages
   HttpError404
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Get:25 http://us.archive.ubuntu.com precise-security/universe Sources [34.2 kB]
 Hit http://archive.ubuntu.com trusty/main Translation-en
 Err http://oss.oracle.com unstable/non-free amd64 Packages
   HttpError404
 Hit http://downloads-distro.mongodb.org dist Release.gpg
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Get:26 http://us.archive.ubuntu.com precise-security/multiverse Sources [1,815 B]
 Ign http://oss.oracle.com unstable/main Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://archive.ubuntu.com trusty/multiverse Translation-en
 Get:27 http://us.archive.ubuntu.com precise-security/main amd64 Packages [492 kB]
 Ign http://oss.oracle.com unstable/main Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://oss.oracle.com unstable/non-free Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://archive.ubuntu.com trusty/restricted Translation-en
 Ign http://oss.oracle.com unstable/non-free Translation-en
 Hit http://archive.ubuntu.com trusty/universe Translation-en
 Get:28 http://archive.ubuntu.com trusty-updates/universe amd64 Packages [263 kB]
 Get:29 http://us.archive.ubuntu.com precise-security/restricted amd64 Packages [8,943 B]
 Hit http://repo.mysql.com trusty/mysql-5.6 Sources
 Hit http://repo.mysql.com trusty/mysql-5.6 amd64 Packages
 Get:30 http://us.archive.ubuntu.com precise-security/universe amd64 Packages [108 kB]
 Hit http://repo.mysql.com trusty/mysql-5.6 i386 Packages
 Get:31 http://archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B]
 Get:32 http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.7 kB]
 Get:33 http://us.archive.ubuntu.com precise-security/multiverse amd64 Packages [2,463 B]
 Get:34 http://us.archive.ubuntu.com precise-security/main i386 Packages [531 kB]
 Get:35 http://archive.ubuntu.com trusty-updates/main amd64 Packages [490 kB]
 Hit http://apt.newrelic.com newrelic Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://dl.google.com stable Release
 Hit http://pkg.jenkins-ci.org binary/ Release
 Get:36 http://www.apache.org 21x/main amd64 Packages [704 B]
 Get:37 http://www.apache.org 21x/main i386 Packages [704 B]
 Get:38 http://us.archive.ubuntu.com precise-security/restricted i386 Packages [8,939 B]
 Get:39 http://us.archive.ubuntu.com precise-security/universe i386 Packages [116 kB]
 Hit http://downloads-distro.mongodb.org dist Release
 Get:40 http://us.archive.ubuntu.com precise-security/multiverse i386 Packages [2,652 B]
 Hit http://us.archive.ubuntu.com precise-security/main Translation-en
 Hit http://us.archive.ubuntu.com precise-security/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-security/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-security/universe Translation-en
 Get:41 http://us.archive.ubuntu.com precise-updates/main Sources [487 kB]
 Hit http://apt.newrelic.com newrelic Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://dl.google.com stable/main amd64 Packages
 Hit http://dl.google.com stable/main i386 Packages
 Get:42 http://archive.ubuntu.com trusty-updates/universe i386 Packages [264 kB]
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Get:43 http://us.archive.ubuntu.com precise-updates/restricted Sources [7,981 B]
 Get:44 http://us.archive.ubuntu.com precise-updates/universe Sources [112 kB]
 Hit http://downloads-distro.mongodb.org dist/10gen amd64 Packages
 Hit http://downloads-distro.mongodb.org dist/10gen i386 Packages
 Get:45 http://archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B]
 Get:46 http://us.archive.ubuntu.com precise-updates/multiverse Sources [9,417 B]
 Get:47 http://us.archive.ubuntu.com precise-updates/main amd64 Packages [884 kB]
 Get:48 http://archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.9 kB]
 Get:49 http://archive.ubuntu.com trusty-updates/main i386 Packages [480 kB]
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-updates/universe Translation-en
 Get:50 http://archive.ubuntu.com trusty-proposed/universe amd64 Packages [31.1 kB]
 Get:51 http://archive.ubuntu.com trusty-proposed/restricted amd64 Packages [28 B]
 Get:52 http://archive.ubuntu.com trusty-proposed/multiverse amd64 Packages [28 B]
 Get:53 http://archive.ubuntu.com trusty-proposed/main amd64 Packages [161 kB]
 Get:54 http://us.archive.ubuntu.com precise-updates/restricted amd64 Packages [13.6 kB]
 Get:55 http://us.archive.ubuntu.com precise-updates/universe amd64 Packages [255 kB]
 Get:56 http://archive.ubuntu.com trusty-proposed/universe i386 Packages [31.1 kB]
 Get:57 http://archive.ubuntu.com trusty-proposed/restricted i386 Packages [28 B]
 Get:58 http://archive.ubuntu.com trusty-proposed/multiverse i386 Packages [28 B]
 Get:59 http://archive.ubuntu.com trusty-proposed/main i386 Packages [158 kB]
 Get:60 http://us.archive.ubuntu.com precise-updates/multiverse amd64 Packages [16.4 kB]
 Get:61 http://us.archive.ubuntu.com precise-updates/main i386 Packages [923 kB]
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
 Ign http://dl.hhvm.com trusty/main Translation-en_IN
 Ign http://dl.hhvm.com trusty/main Translation-en
 Ign http://archive.ubuntu.com trusty/main Translation-en_IN
 Ign http://archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://archive.ubuntu.com trusty/universe Translation-en_IN
 Ign http://mirror.stshosting.co.uk precise/main Translation-en_IN
 Ign http://mirror.stshosting.co.uk precise/main Translation-en
 Get:62 http://us.archive.ubuntu.com precise-updates/restricted i386 Packages [13.6 kB]
 Get:63 http://us.archive.ubuntu.com precise-updates/universe i386 Packages [264 kB]
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en_IN
 Get:64 http://us.archive.ubuntu.com precise-updates/multiverse i386 Packages [16.6 kB]
 Hit http://us.archive.ubuntu.com precise-updates/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/multiverse Translation-en
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/universe Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/main Sources
 Hit http://us.archive.ubuntu.com precise-backports/restricted Sources
 Hit http://us.archive.ubuntu.com precise-backports/universe Sources
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Sources
 Hit http://us.archive.ubuntu.com precise-backports/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/main Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/universe Translation-en
 Ign http://www.apache.org 21x/main Translation-en_IN
 Ign http://www.apache.org 21x/main Translation-en
 Ign http://dl.google.com stable/main Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/main Translation-en_IN
 Ign http://dl.google.com stable/main Translation-en
 Ign http://us.archive.ubuntu.com precise/multiverse Translation-en_IN
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/restricted Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/universe Translation-en_IN
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en_IN
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en
 Ign http://apt.newrelic.com newrelic/non-free Translation-en_IN
 Ign http://apt.newrelic.com newrelic/non-free Translation-en
 Fetched 7,656 kB in 2min 14s (56.9 kB/s)
 Reading package lists...
 Building dependency tree...
 Reading state information...
 jmeter is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 Temp File /tmp/ptconfigure-temp-script-51122634115.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 Jmeter: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
------------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce module de volonté installe le Jmeter dans la version mise à jour.
* Si le module existe déjà dans la machine de l'utilisateur, il affiche un message comme il est déjà existant.
* JMeter soutient paramétrage variable affirmations (de validation de réponse), par les cookies de fil, les variables de configuration et une 
  variété derapports.
* Développeurs hors site peuvent facilement étendre JMeter avec plugins personnalisés.

