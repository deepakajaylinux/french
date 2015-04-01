==============
NagiosServer
==============

Synopsis
-------------

Nagios est une application logicielle open source de surveillance du système informatique, la surveillance du réseau et la surveillance de l'infrastructure. Nagios offre une surveillance et d'alerte pour les serveurs, les commutateurs, les applications et les services. Il alerte les utilisateurs quand les choses vont mal et les alerte une seconde fois lorsque le problème a été résolu.

Nagios, créé à l'origine sous le nom de NetSaint, a été écrit et est actuellement maintenu par Ethan Galstad avec un groupe de développeurs qui entretiennent activement à la fois officielles et officieuses plugins. Nagios a été initialement conçu pour fonctionner sous Linux mais fonctionne également bien sur d'autres variantes Unix. Ce est un logiciel libre sous licence les termes de la GNU General Public License Version 2 telle que publiée par la Free Software Foundation.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module Nagios. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure nagios help


Est listé ci-dessous la capture d'écran picturale de la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/# ptconfigure nagiosserver help

 ******************************


  This command is part of Core and provides you with a method by which you can install Nagios.

  NagiosServer, nagios-server, nagiosserver, nagios

        - install
        Installs Nagios Network Monitoring Server
        example: ptconfigure nagios-server install

 ------------------------------
 End Help
 ******************************



installation
----------------

Cette commande aide à l'installation de Nagios dans le système. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
	        ptconfigure nagios install

La représentation picturale de la commande ci-dessus est listé ci-dessous,

.. code-block:: bash


 kevell@corp:/# ptconfigure nagios-server install

 Install Nagios Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Nagios Server!        *
 *******************************

 * Starting nagios3 monitoring daemon nagios3                                                                                  [ OK ] 
 enabling Apache2 config...
 apache2_invoke: Enable module cgi
 * Restarting web server apache2                                                                                                  AH00558:  
 apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to 
 suppress this message
                                                                                                                               [ OK ]
 apache2_invoke: Enable configuration nagios3
 * Reloading web server apache2                                                                                                        * 
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libjs-jquery nagios-images nagios3-cgi nagios3-common nagios3-core
 Suggested packages:
  javascript-common
 The following NEW packages will be installed:
  libjs-jquery nagios-images nagios3 nagios3-cgi nagios3-common nagios3-core
 0 upgraded, 6 newly installed, 0 to remove and 250 not upgraded.
 Need to get 3,748 kB of archives.
 After this operation, 12.3 MB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main nagios-images all 0.8 [2,589 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-common all 3.5.1-1ubuntu1 [53.7 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-cgi amd64 3.5.1-1ubuntu1 [794 kB]
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-core amd64 3.5.1-1ubuntu1 [231 kB]
 Get:6 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3 amd64 3.5.1-1ubuntu1 [1,528 B]
 Preconfiguring packages ...
 Fetched 3,748 kB in 1min 11s (52.1 kB/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 231932 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package nagios-images.
 Preparing to unpack .../nagios-images_0.8_all.deb ...
 Unpacking nagios-images (0.8) ...
 Selecting previously unselected package nagios3-common.
 Preparing to unpack .../nagios3-common_3.5.1-1ubuntu1_all.deb ...
 Unpacking nagios3-common (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-cgi.
 Preparing to unpack .../nagios3-cgi_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-cgi (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-core.
 Preparing to unpack .../nagios3-core_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-core (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3.
 Preparing to unpack .../nagios3_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3 (3.5.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up nagios-images (0.8) ...
 Setting up nagios3-common (3.5.1-1ubuntu1) ...
 Setting up nagios3-cgi (3.5.1-1ubuntu1) ...
 Setting up nagios3-core (3.5.1-1ubuntu1) ...
 Setting up nagios3 (3.5.1-1ubuntu1) ...
 [Pharaoh Logging] Adding Package nagios3 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NagiosServer: Success
 ------------------------------
 Installer Finished
 ******************************



Options
-----------                               

.. cssclass:: table-bordered
 
 +---------------------+----------------------------------------------------------------+--------+-------------------------------------+
 | paramètres          | paramètre alternatif                                           | option | commentaires                        |
 +=====================+================================================================+========+=====================================+
 |ptconfigure          | Il ya quatre autres paramètres qui peuvent être utilisés dans  | Y      | Le système démarre processus        |     
 |nagiosserver         | la ligne de commande. NagiosServer, nagios-server,             |        | d'installation                      |
 |Install?(Y/N)        | nagiosserver, nagios Eg: ptconfigure nagios install/           |        |                                     |
 |                     | ptconfigure nagiosserver install                               |        |                                     |
 +---------------------+----------------------------------------------------------------+--------+-------------------------------------+
 |ptconfigure          | Il ya quatre autres paramètres qui peuvent être utilisés dans  | N      | Système arrête processus            |
 |nagiosserver         | la ligne de commande.NagiosServer, nagios-server,              |        | d'installation                      |
 |install?(Y/N)        | nagiosserver, nagios Eg: ptconfigure nagios install/           |        |                                     |
 |                     | ptconfigure nagiosserver install|                              |        |                                     |
 +---------------------+----------------------------------------------------------------+--------+-------------------------------------+




Avantages
--------------

* Suivi des services de réseau (SMTP, POP3, HTTP, NNTP, ICMP, SNMP, FTP, SSH)

* Suivi des ressources d'accueil (charge processeur, l'utilisation du disque, les journaux système) sur la majorité des systèmes 
  d'exploitation de réseau, y compris Microsoft Fenêtres avec le plugin de l'NSClient ou Vérifiez MK

* Suivi de quelque chose de semblable sondes (température, alarmes, etc.) Qui ont la capacité d'envoyer des données collectées via un réseau de
  plugins spécifiquement écrites

* Suivi par exécuter des scripts à distance via Nagios distance Plugin Executor

* Surveillance à distance soutenus par les tunnels SSH ou SSL crypté

* Les données disponibles plugins graphiques

* contrôles de service PARALLELISE

* notifications de contact en cas de problèmes de service ou de l'hôte se produisent et se résoudre par e-mail, pager, SMS, ou toute autre
  méthode définie par l'utilisateur par le biais System Plugin

* La possibilité de définir des gestionnaires d'événements pour être exécuté lors d'une réparation ou d'accueil des événements pour la 
  résolution proactive des problèmes

* Journal rotation automatique de fichier

* Prise en charge de la mise en œuvre supervision redondante d'hôtes

* Une interface web option pour visualiser état actuel du réseau, les notifications, l'histoire de problème, les fichiers journaux, etc.

* Stockage de données via des fichiers texte plutôt que de base de données

* Un design simple plugin qui permet aux utilisateurs de développer facilement leurs propres contrôles de service en fonction des besoins, en
  utilisant leurs outils de choix (scripts shell, C++, Perl, Ruby, Python, PHP, C#, etc) 
