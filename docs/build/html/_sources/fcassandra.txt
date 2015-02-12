============
Cassandra
============

synopsis
-----------

Cassandra est un système distribué de gestion de base de données open source conçu pour gérer de grandes quantités de données sur plusieurs serveurs des produits de base, offrant une haute disponibilité sans point de défaillance unique. Cassandra offre un support robuste pour les clusters couvrant plusieurs datacenters, avec le maître asynchrone moins de réplication permettant des opérations à faible latence pour tous les 
clients.

Le modèle de données de Cassandra est un magasin de ligne partitionné avec une cohérence accordable. Les lignes sont organisées en tables; le premier composant de la clé primaire d'une table est la clé de la partition; au sein d'une partition, les rangées sont groupées par les autres colonnes de la clé. D'autres colonnes peuvent être indexés séparément de la clé primaire.

Commande Aide
---------------------

Cette commande permet de déterminer l'utilisation d'un module Cassandra. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        cleopatra cassandra help

La représentation picturale de la commande ci-dessus est illustré ci-dessous,

.. code-block:: bash

 kevell@corp:/# cleopatra cassandra help

 ******************************


  This command allows you to update Cassandra.

  Cassandra, cassandra

        - install
        Installs the latest version of Cassandra
        example: cleopatra cassandra install

 ------------------------------
 End Help
 ******************************

installation
--------------

Cette commande aide à l'installation de Cassandra dans le système. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash

                cleopatra cassandra install

La représentation picturale de la commande ci-dessus est illustré ci-dessous,

.. code-block:: bash

 kevell@corp:/#  cleopatra cassandra install

 Install Cassandra? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Cassandra!        *
 *******************************
 Creating /tmp/cleopatra-temp-script-10553509319.sh
 chmod 755 /tmp/cleopatra-temp-script-10553509319.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-10553509319.sh Permissions
 Executing /tmp/cleopatra-temp-script-10553509319.sh
 gpg: directory `/home/deepak/.gnupg' created
 gpg: new configuration file `/home/deepak/.gnupg/gpg.conf' created
 gpg: WARNING: options in `/home/deepak/.gnupg/gpg.conf' are not yet active during this run
 gpg: keyring `/home/deepak/.gnupg/secring.gpg' created
 gpg: keyring `/home/deepak/.gnupg/pubring.gpg' created
 gpg: requesting key 8D77295D from hkp server pgp.mit.edu
 gpg: /home/deepak/.gnupg/trustdb.gpg: trustdb created
 gpg: key 8D77295D: public key "Eric Evans <eevans@sym-link.com>" imported
 gpg: no ultimately trusted keys found
 gpg: Total number processed: 1
 gpg:               imported: 1  (RSA: 1)
 gpg: requesting key 2B5C1B00 from hkp server pgp.mit.edu
 gpg: key 2B5C1B00: public key "Sylvain Lebresne (pcmanus) <sylvain@datastax.com>" imported
 gpg: Total number processed: 1
 gpg:               imported: 1  (RSA: 1)
 gpg: requesting key 0353B12C from hkp server pgp.mit.edu
 gpg: key 0353B12C: public key "T Jake Luciani <jake@apache.org>" imported
 gpg: Total number processed: 1
 gpg:               imported: 1  (RSA: 1)
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 deb-src http://www.apache.org/dist/cassandra/debian 21x main
 OK
 OK
 OK
 Get:1 http://www.apache.org 21x InRelease [3167 B]
 Get:2 http://www.apache.org 21x/main amd64 Packages [696 B]
 Ign http://extras.ubuntu.com trusty InRelease
 Get:3 http://www.apache.org 21x/main i386 Packages [696 B]
 Hit http://extras.ubuntu.com trusty Release.gpg
 Hit http://extras.ubuntu.com trusty Release
 Hit http://extras.ubuntu.com trusty/main Sources
 Ign http://www.apache.org 21x/main Translation-en
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://us.archive.ubuntu.com precise InRelease
 Hit http://dl.hhvm.com trusty InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://us.archive.ubuntu.com precise Release.gpg
 Hit http://dl.hhvm.com trusty/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise Release
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Hit http://us.archive.ubuntu.com precise/main amd64 Packages
 Get:4 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Hit http://us.archive.ubuntu.com precise/universe amd64 Packages
 Get:5 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Hit http://us.archive.ubuntu.com precise/main i386 Packages
 Get:6 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Get:7 http://us.archive.ubuntu.com precise/universe i386 Packages [4796 kB]
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Ign http://dl.hhvm.com trusty/main Translation-en
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Ign http://archive.canonical.com trusty InRelease
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Hit http://archive.canonical.com trusty Release.gpg
 Ign http://security.ubuntu.com trusty-security InRelease
 Hit http://archive.canonical.com trusty Release
 Get:8 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Hit http://archive.canonical.com trusty/partner Sources
 Get:9 http://security.ubuntu.com trusty-security Release [62.0 kB]
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Hit http://archive.canonical.com trusty/partner amd64 Packages
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Get:10 http://security.ubuntu.com trusty-security/main Sources [64.8 kB]
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Ign http://in.archive.ubuntu.com trusty InRelease
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Ign http://repos.zend.com server InRelease
 Hit http://repos.zend.com server Release.gpg
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Hit http://repos.zend.com server Release
 Hit http://repos.zend.com server/non-free amd64 Packages
 Hit http://repos.zend.com server/non-free i386 Packages
 Ign http://apt.newrelic.com newrelic InRelease
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Get:11 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://archive.canonical.com trusty/partner i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Hit http://archive.canonical.com trusty/partner Translation-en
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://in.archive.ubuntu.com trusty Release
 Get:12 http://in.archive.ubuntu.com trusty-updates Release [62.0 kB]
 Ign http://wireframesketcher.com  InRelease
 Ign http://repos.zend.com server/non-free Translation-en
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Get:13 http://security.ubuntu.com trusty-security/restricted Sources [2061 B]
 Get:14 http://security.ubuntu.com trusty-security/universe Sources [17.4 kB]
 Hit http://apt.newrelic.com newrelic Release.gpg
 Ign https://repo.varnish-cache.org precise InRelease
 Get:15 http://security.ubuntu.com trusty-security/multiverse Sources [723 B]
 Hit http://ppa.launchpad.net trusty Release.gpg
 Ign http://packages.dotdeb.org squeeze InRelease
 Get:16 http://security.ubuntu.com trusty-security/main amd64 Packages [200 kB]
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Hit http://wireframesketcher.com  Release.gpg
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Hit http://packages.dotdeb.org squeeze Release
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://apt.newrelic.com newrelic Release
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://ppa.launchpad.net trusty Release
 Get:17 https://repo.varnish-cache.org precise Release.gpg
 Hit http://wireframesketcher.com  Release
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Get:18 https://repo.varnish-cache.org precise Release
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Get:19 https://repo.varnish-cache.org precise/varnish-4.0 amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Get:20 https://repo.varnish-cache.org precise/varnish-4.0 i386 Packages
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Get:21 https://repo.varnish-cache.org precise/varnish-4.0 Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Get:22 http://in.archive.ubuntu.com trusty-updates/main Sources [160 kB]
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Get:23 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8875 B]
 Get:24 http://security.ubuntu.com trusty-security/universe amd64 Packages [85.3 kB]
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en
 Get:25 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [1161 B]
 Hit http://wireframesketcher.com  Packages
 Get:26 http://security.ubuntu.com trusty-security/main i386 Packages [190 kB]
 Get:27 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2061 B]
 Get:28 http://in.archive.ubuntu.com trusty-updates/universe Sources [99.4 kB]
 Get:29 http://security.ubuntu.com trusty-security/restricted i386 Packages [8846 B]
 Get:30 http://security.ubuntu.com trusty-security/universe i386 Packages [85.3 kB]
 Get:31 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [4502 B]
 Get:32 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [407 kB]
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Ign http://apt.newrelic.com newrelic/non-free Translation-en
 Get:33 http://security.ubuntu.com trusty-security/multiverse i386 Packages [1412 B]
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Ign http://wireframesketcher.com  Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Get:34 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [8875 B]
 Get:35 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [243 kB]
 Get:36 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.2 kB]
 Get:37 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [399 kB]
 Get:38 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [8846 B]
 Get:39 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [243 kB]
 Get:40 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.4 kB]
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
 Get:41 http://us.archive.ubuntu.com precise/main Translation-en [726 kB]
 Get:42 http://us.archive.ubuntu.com precise/universe Translation-en [3341 kB]
 Fetched 10.2 MB in 4min 2s (42.1 kB/s)
 Temp File /tmp/cleopatra-temp-script-10553509319.sh Removed
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://us.archive.ubuntu.com/ubuntu/ precise/main amd64 Packages (/var/lib/apt/lists/us.archive.ubuntu.com_ubuntu_dists_precise_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://us.archive.ubuntu.com/ubuntu/ precise/universe amd64 Packages (/var/lib/apt/lists/us.archive.ubuntu.com_ubuntu_dists_precise_universe_binary-amd64_Packages)
 W: Duplicate sources.list entry http://us.archive.ubuntu.com/ubuntu/ precise/main i386 Packages (/var/lib/apt/lists/us.archive.ubuntu.com_ubuntu_dists_precise_main_binary-i386_Packages)
 W: Duplicate sources.list entry http://us.archive.ubuntu.com/ubuntu/ precise/universe i386 Packages (/var/lib/apt/lists/us.archive.ubuntu.com_ubuntu_dists_precise_universe_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package cassandra from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 
 
 Single App Installer:
 --------------------------------------------
 Cassandra: Success
 ------------------------------
 Installer Finished
 ******************************

options
----------


.. cssclass:: table-bordered



 +---------------------------+-------------------------------------------+------------------+----------------------------------------------+
 | Paramètres		     | Alternative Paramètre			 | options	    | commentaires			           |
 +===========================+===========================================+==================+==============================================+
 |cleopatra cassandra        | Il ya deux autres paramètres qui peuvent  | Y 		    | Le système démarre processus d'installation  |
 |Install 		     | être utilisés dans la ligne de commande.  |		    |						   |
 | 			     | Cassandra , cassandra Par 		 |		    |						   |
 |			     | exemple: cleopatra cassandra install,     |		    |						   |
 | 			     |          cleopatra cassandra install      | 		    |						   |
 +---------------------------+-------------------------------------------+------------------+----------------------------------------------+
 |cleopatra cassandra        | Il ya deux autres paramètres qui peuvent  | N                | Système arrête processus d'installation      |
 |Install                    | être utilisés dans la ligne de commande.  |                  |                                              |
 |                           | Cassandra , cassandra Par                 |                  |                                              |
 |                           | exemple: cleopatra cassandra install,     |                  |                                              |
 |                           |          cleopatra cassandra install|     |                  |                                              |
 +---------------------------+-------------------------------------------+------------------+----------------------------------------------+


avantages
--------------

* Décentralisée - Chaque noeud du cluster a le même rôle. Il n'y a pas de point de défaillance unique. Les données sont distribuées sur le 
  cluster (de sorte que chaque noeud contient des données différentes), mais il n'y a pas de maître que chaque nœud peut desservir toute 
  demande.
* Prend en charge la réplication de centre de réplication et de données multi - stratégies de réplication sont configurables. Cassandra est 
  conçu comme un système distribué, pour le déploiement d'un grand nombre de noeuds à travers de multiples centres de données. Les principales 
  caractéristiques de l'architecture distribuée de Cassandra sont spécifiquement adaptés pour le centre de données multiples déploiement, pour 
  la redondance, pour le basculement et la récupération en cas de catastrophe.
* Évolutivité - Lire et écrire débit à la fois augmenter linéairement en nouvelles machines sont ajoutés, sans temps d'arrêt ou l'interruption d  'applications.
* Tolérant aux pannes - Les données sont automatiquement répliquées sur plusieurs nœuds pour la tolérance aux pannes. Réplication sur plusieurs   centres de données est prise en charge. Nœuds défaillants peuvent être remplacés sans interruption.
* La cohérence accordable - écrit et lit offrir un niveau de cohérence accordable, tout le chemin depuis », écrit ne manquent jamais" à "bloc 
  pour toutes les répliques soit lisible", avec le niveau de quorum au milieu.
