==========
Xcache
==========

synopsis
---------

XCache est un cacher d'opération code gratuit, open source, il est conçu pour améliorer les performances d'exécution de scripts PHP sur les serveurs. Il optimise les performances en éliminant le moment de la compilation du code PHP de la version compilée du code de mise en cache dans la mémoire et de cette façon la version compilée charge le script PHP directement à partir de la mémoire.


Commande Aide
---------------

Cette commande permet de déterminer l'utilisation de xcache. Il énumère les paramètres alternatifs de xcache. Il décrit également la syntaxe pour le fonctionnement du module xcache. La commande help pour xcache est montrée ci-dessous.

.. code-block:: bash

	ptconfigure xcache help

La représentation picturale de la commande ci-dessus est listée ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache help
 ******************************


  This command allows you to update Xcache.

  Xcache, xcache

        - install
        Installs the latest version of xcache
        example: ptconfigure xcache install

 ------------------------------
 End Help
 ******************************


installation
---------------


La commande utilisée pour l'installation du module xcache sur le terminal est répertoriée ci-dessous,

.. code-block:: bash

        ptconfigure xcache install

La commande ci-dessus a pour but d'installer la dernière version de xcache et ses dépendances

La représentation picturale de la commande ci-dessus est listée ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache install
 Install Xcache? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Xcache!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-56147605410.sh
 chmod 755 /tmp/ptconfigure-temp-script-56147605410.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-56147605410.sh Permissions
 Executing /tmp/ptconfigure-temp-script-56147605410.sh
 --2015-03-20 17:05:11--  http://kr.archive.ubuntu.com/ubuntu/pool/universe/x/xcache/php5-xcache_3.1.0-2_amd64.deb
 Resolving kr.archive.ubuntu.com (kr.archive.ubuntu.com)... 103.22.220.133
 Connecting to kr.archive.ubuntu.com (kr.archive.ubuntu.com)|103.22.220.133|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 108582 (106K) [application/x-debian-package]
 Saving to: ‘php5-xcache_3.1.0-2_amd64.deb.1’

 100%[=======================================================================================================>] 1,08,582    36.1KB/s   in 2.9s   

 2015-03-20 17:05:15 (36.1 KB/s) - ‘php5-xcache_3.1.0-2_amd64.deb.1’ saved [108582/108582]

 php5_invoke xcache: already enabled for apache2 SAPI
 php5_invoke xcache: already enabled for cli SAPI
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 (Reading database ... 195553 files and directories currently installed.)
 Preparing to unpack php5-xcache_3.1.0-2_amd64.deb ...
 Unpacking php5-xcache (3.1.0-2) over (3.1.0-2) ...
 Setting up php5-xcache (3.1.0-2) ...
 * Restarting web server apache2
   ...done.
 Temp File /tmp/ptconfigure-temp-script-56147605410.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xcache: Success
 ------------------------------
 Installer Finished
 ******************************



Alternative Paramètre
-----------------------

Il y a deux autres paramètres qui peuvent être utilisés en ligne de commande.

Xcache, xcache


avantages
-----------

* Stable fonctionnement 
* adaptation rapide aux nouvelles versions PHP 
* installation Simple










