============
NetBeans
============


Synopsis
-------------

NetBeans est un environnement de développement intégré (IDE) pour développer principalement avec Java, mais aussi avec d'autres langues, en particulier PHP, C / C ++ et HTML. Ce est aussi un cadre de la plate-forme d'application pour les applications Java de bureau et autres.

L'EDI NetBeans est écrit en Java et peut fonctionner sur Windows, OS X, Linux, Solaris et d'autres plates-formes supportant une JVM compatible. NetBeans IDE est un IDE multiplate-forme avec un support intégré pour langage de programmation Java.

La plate-forme NetBeans permet aux applications d'être développés à partir d'un ensemble de composants logiciels modulaires appelées modules. Les applications basées sur la plate-forme NetBeans (y compris l'EDI NetBeans lui-même) peuvent être prolongés par des développeurs tiers.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module Netbeans. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure Netbeans help

.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans help
 ******************************


  This command allows you to install and uninstall NetBeans - IDE.

  NetBeans, Netbeans, netbeans

        - install
        Installs a version of NetBeans.
        example: ptconfigure netbeans install
	
	- uninstall
        Uninstalls a version of NetBeans.
        example: ptconfigure netbeans uninstall
 ------------------------------
 End Help
 ******************************


installation
----------------

Cette commande aide à l'installation dans le système Netbeans. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
	        ptconfigure netbeans install


.. code-block:: bash


 kevell@corp:/# ptconfigure netbeans install
 Install NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed

 Enter (1) to Install NetBeans in Silent:
 Enter (2) to install NetBeans in UserFriendly:
 1
 Creating /tmp/ptconfigure-temp-script-53829501149.sh
 chmod 755 /tmp/ptconfigure-temp-script-53829501149.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-53829501149.sh Permissions
 Executing /tmp/ptconfigure-temp-script-53829501149.sh
 --2015-04-01 11:42:15--  http://download.netbeans.org/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving download.netbeans.org (download.netbeans.org)... 137.254.120.26
 Connecting to download.netbeans.org (download.netbeans.org)|137.254.120.26|:80... connected.
 HTTP request sent, awaiting response... 302 Moved Temporarily
 Location: http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh [following]
 --2015-04-01 11:42:16--  http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving dlc-cdn.sun.com (dlc-cdn.sun.com)... 23.205.118.80, 23.205.118.73
 Connecting to dlc-cdn.sun.com (dlc-cdn.sun.com)|23.205.118.80|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 212403200 (203M) [application/x-sh]
 Saving to: â€˜netbeans-8.0-linux.shâ€™ 

 100%[===========================================================================================>] 21,24,03,200 78.0KB/s   in 78m 40s

 2015-04-01 13:00:58 (43.9 KB/s) - â€˜netbeans-8.0-linux.shâ€™ saved [212403200/212403200]

 Temp File /tmp/ptconfigure-temp-script-53829501149.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ****************************** 


désinstallation
-----------------

Cette commande aide à la désinstallation Netbeans dans le système . La commande ci-dessous donnée exécuter le processus d'installation .

.. code-block:: bash

	ptconfigure netbeans uninstall

.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans uninstall

 Uninstall NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-80402838784.sh
 chmod 755 /tmp/ptconfigure-temp-script-80402838784.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-80402838784.sh Permissions
 Executing /tmp/ptconfigure-temp-script-80402838784.sh
 Configuring the installer...
 Searching for JVM on the system...
 Extracting installation data...
 Running the installer wizard...
 Temp File /tmp/ptconfigure-temp-script-80402838784.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ******************************



Options
-----------                               

.. cssclass:: table-bordered


 +-----------------------+-----------------------------------------------------+--------------+-------------------------------------+
 | paramètres            | paramètre alternatif                                | option       | commentaires                        |
 +=======================+=====================================================+==============+=====================================+
 |ptconfigure Netbeans   | Il ya trois paramètres alternatifs qui peuvent être | Y            | Le système démarre processus        |
 |Install?(Y/N)          | utilisés en ligne de commande. Netbeans, NetBeans,  |              | d'installation                      |
 |                       | netbeans Par exemple,: ptconfigure NetBeans install |              |                                     |
 |                       | , ptconfigure netbeans install                      |              |                                     |
 +-----------------------+-----------------------------------------------------+--------------+-------------------------------------+
 |ptconfigure Netbeans   | Il ya trois paramètres alternatifs qui peuvent être | N            | Système arrête processus            |
 |Install?(Y/N)          | utilisés en ligne de commande. Netbeans, NetBeans,  |              | d'installation                      |
 |                       | netbeans Par exemple,: ptconfigure NetBeans install |              |                                     |
 |                       | , ptconfigure netbeans install|                     |              |                                     |
 +-----------------------+-----------------------------------------------------+--------------+-------------------------------------+




avantages
--------------

* La gestion de l'interface utilisateur (par exemple, les menus et les barres d'outils)
* Gestion des paramètres de l'utilisateur
* La gestion du stockage (sauvegarde et le chargement tout type de données)
* Gestion des fenêtres
* Assistant cadre (prend en charge les boîtes de dialogue, étape par étape)
* NetBeans Visual Library
* Outils de développement intégré
