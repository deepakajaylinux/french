=============
NetworkTools
=============

synopsis
----------

Les outils de réseau sont des utilitaires logiciels conçus pour analyser et configurer divers aspects du réseau informatique. Les outils de réseau les plus courants trouvés sur la plupart des systèmes d'exploitation comprend Traceroute, Netstat et Ping. Chaque outils de réseau ont ses propres fonctions.

Par exemple:

Ping est utilisé pour vérifier la connectivité

Netstat est utilisé pour afficher la connexion réseau entrant et sortant

Commande Aide
--------------

Cette commande permet de déterminer l'utilisation d'un module d'outils de réseau. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande va guider l'utilisateur final de savoir quand et comment la commande à utiliser. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash

		ptconfigure networktools help


La représentation picturale de la commande ci-dessus est listé ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools help
 ******************************


  This command allows you to install a set of common Network Tools. These include
  traceroute, netstat, lsof, telnet and ps.

  NetworkTools, networktools, network-tools

        - install
        Installs the latest version of Network Tools
        example: ptconfigure networktools install

 ------------------------------
 End Help
 ******************************


installation
---------------

Lorsque l'utilisateur a besoin d'installer ne importe quel outil de réseau dans la machine. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash


 	ptconfigure networktool install



.. cssclass:: table-bordered

 +---------------------+---------------------------------------+--------------+----------------------------------------------+
 | paramètres          | paramètre alternatif                  | option       | commentaires                                 |
 +=====================+=======================================+==============+==============================================+
 |Install Network      | au lieu de NetworkTools, nous pouvons | Y(Yes)       | Si l'utilisateur souhaite procéder le        |
 |Tools? (Y/N)         | utiliser networktools, network-tools  |              | processus d'installation qu'ils peuvent      |
 |                     | aussi.                                |              | entrée comme Y.                              |
 +---------------------+---------------------------------------+--------------+----------------------------------------------+
 |Install Network      | au lieu de NetworkTools, nous pouvons | N(No)        | Si l'utilisateur souhaite quitter le         |
 |Tools? (Y/N)         | utiliser networktools, network-tools  |              | processus d'installation qu'ils peuvent      |
 |                     | aussi.                                |              | entrée comme N.|                             |
 +---------------------+---------------------------------------+--------------+----------------------------------------------+


Si l'installation utilisateur de produit, au cours du processus d'installation, les étapes suivantes sont impliqués,

* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les nouveaux paquets qui installent.
* Détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.



Capture d' écran ci-dessous illustre graphiquement le processus décrit ci-dessus pour l'installation et la désinstallation .

.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools install
 Install Network Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Network Tools!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  traceroute
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 45.0 kB of archives.
 After this operation, 176 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe traceroute amd64 1:2.0.20-0ubuntu0.1 [45.0 kB]
 Fetched 45.0 kB in 4s (10.0 kB/s)
 Selecting previously unselected package traceroute.
 (Reading database ... 182980 files and directories currently installed.)
 Preparing to unpack .../traceroute_1%3a2.0.20-0ubuntu0.1_amd64.deb ...
 Unpacking traceroute (1:2.0.20-0ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up traceroute (1:2.0.20-0ubuntu0.1) ...
 update-alternatives: using /usr/bin/traceroute.db to provide /usr/bin/traceroute (traceroute) in auto mode
 update-alternatives: using /usr/bin/lft.db to provide /usr/bin/lft (lft) in auto mode
 update-alternatives: using /usr/bin/traceproto.db to provide /usr/bin/traceproto (traceproto) in auto mode
 update-alternatives: using /usr/sbin/tcptraceroute.db to provide /usr/sbin/tcptraceroute (tcptraceroute) in auto mode
 [Pharaoh Logging] Adding Package traceroute from the Packager Apt executed correctly
 [Pharaoh Logging] Package netstat from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package lsof from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package telnet from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package ps from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetworkTools: Success
 ------------------------------
 Installer Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure networktools uninstall

 Uninstall Network Tools? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !Network Tools!!        *
 *******************************
 [Pharaoh Logging] Removing Package traceroute
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Package 'traceroute' is not installed, so not removed
 0 upgraded, 0 newly installed, 0 to remove and 70 not upgraded.
 [Pharaoh Logging] Package traceroute from the Packager Apt is not installed, so not removed.
 [Pharaoh Logging] Removing Package netstat
 E: Unable to locate package netstat
 Reading package lists...
 Building dependency tree...
 Reading state information...
 [Pharaoh Logging] Removing Package lsof
 php5_invoke prerm: Disable module opcache for apache2 SAPI
 php5_invoke prerm: Disable module readline for apache2 SAPI
 php5_invoke prerm: Disable module pdo for apache2 SAPI
 php5_invoke prerm: Disable module mcrypt for apache2 SAPI
 php5_invoke prerm: Disable module json for apache2 SAPI
 apache2_invoke prerm: Disable module php5
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 php5_invoke prerm: Disable module readline for cgi SAPI
 php5_invoke prerm: Disable module readline for cli SAPI
 php5_invoke prerm: Disable module opcache for cli SAPI
 php5_invoke prerm: Disable module pdo for cli SAPI
 php5_invoke prerm: Disable module mcrypt for cli SAPI
 php5_invoke prerm: Disable module json for cli SAPI
 php5_invoke prerm: Disable module opcache for cgi SAPI
 php5_invoke prerm: Disable module pdo for cgi SAPI
 php5_invoke prerm: Disable module mcrypt for cgi SAPI
 php5_invoke prerm: Disable module json for cgi SAPI
 apache2_invoke php5-cgi prerm: No action required
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  apache2 libmcrypt4
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
   libapache2-mod-php5 lsof php5 php5-cgi php5-cli php5-common php5-json
  php5-mcrypt php5-readline
 0 upgraded, 0 newly installed, 9 to remove and 70 not upgraded.
 After this operation, 39.2 MB disk space will be freed.
 (Reading database ... 194484 files and directories currently installed.)
 Removing php5 (5.5.9+dfsg-1ubuntu4.7) ...
 Removing libapache2-mod-php5 (5.5.9+dfsg-1ubuntu4.7) ...
 Module php5 disabled.
  * Restarting web server apache2
   ...done.
 Removing php5-readline (5.5.9+dfsg-1ubuntu4.7) ...
 Removing php5-mcrypt (5.4.6-0ubuntu5) ...
 Removing php5-cli (5.5.9+dfsg-1ubuntu4.7) ...
 Removing php5-cgi (5.5.9+dfsg-1ubuntu4.7) ...
 Removing php5-json (1.3.2-2build1) ...
 Removing php5-common (5.5.9+dfsg-1ubuntu4.7) ...
 Removing lsof (4.86+dfsg-1ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Removed Package lsof from the Packager Apt
 [Pharaoh Logging] Removing Package telnet
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Package 'telnet' is not installed, so not removed
 The following packages were automatically installed and are no longer required:
   apache2 libmcrypt4
 Use 'apt-get autoremove' to remove them.
 0 upgraded, 0 newly installed, 0 to remove and 70 not upgraded.
 [Pharaoh Logging] Package telnet from the Packager Apt is not installed, so not removed.
 [Pharaoh Logging] Removing Package ps
 E: Unable to locate package ps
 Reading package lists...
 Building dependency tree...
 Reading state information...
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 
 
 Single App Uninstaller:
 ------------------------------
 NetworkTools: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
-----------

Ce module aide à l'installation de l'ensemble d'outils de réseau communes. Cela profite aux utilisateurs d'installer différents outils qui peuvent être utiles pour la mise en réseau avec d'autres ordinateurs à la fois au sein du réseau et à travers l'Internet. Cela aide les utilisateurs qui travaillent avec des machines distantes.
