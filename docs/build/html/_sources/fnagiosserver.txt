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

 kevell@corp:/# ptconfigure nagios help
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
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:

 The following packages have unmet dependencies:
 nagios3 : Depends: nagios3-core (= 3.2.3-3ubuntu1) but it is not going to be installed
 [Pharaoh Logging] Adding Package nagios3 from the Packager Apt did not execute correctly
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
 |nagiosserver         | la ligne de commande.NagiosServer, nagios-server, nagiosserver |        | d'installation                      |
 |Install?(Y/N)        | , nagios Eg: ptconfigure nagios install/                       |        |                                     |
 |                     | ptconfigure nagiosserver install                               |        |                                     |
 +---------------------+----------------------------------------------------------------+--------+-------------------------------------+
 |ptconfigure          | Il ya quatre autres paramètres qui peuvent être utilisés dans  | N      | Système arrête processus            |
 |nagiosserver         | la ligne de commande.NagiosServer, nagios-server, nagiosserver |        | d'installation                      |
 |install?(Y/N)        | , nagios Eg: ptconfigure nagios install/                       |        |                                     |
 |                     | ptconfigure nagiosserver install|                              |        |                                     |
 +---------------------+----------------------------------------------------------------+--------+-------------------------------------+




Avantages
--------------

* Suivi des services de réseau (SMTP, POP3, HTTP, NNTP, ICMP, SNMP, FTP, SSH)
* Suivi des ressources d'accueil (charge processeur, l'utilisation du disque, les journaux système) sur la majorité des systèmes 
  d'exploitation de réseau, y compris Microsoft
  Fenêtres avec le plugin de l'NSClient ou Vérifiez MK.
* Suivi de quelque chose de semblable sondes (température, alarmes, etc.) Qui ont la capacité d'envoyer des données collectées via un réseau de
  plugins spécifiquement écrites
* Suivi par exécuter des scripts à distance via Nagios distance Plugin Executor
* Surveillance à distance soutenus par les tunnels SSH ou SSL crypté.
* Les données disponibles plugins graphiques
* contrôles de service PARALLELISE
* La capacité de définir des hiérarchies d'accueil de réseau à l'aide (hôtes 'parent') permettant la détection et la distinction entre des 
  hôtes qui sont à la baisse ou inaccessible
* notifications de contact en cas de problèmes de service ou de l'hôte se produisent et se résoudre par e-mail, pager, SMS, ou toute autre 
  méthode définie par l'utilisateur par le biais  System Plugin.
* La possibilité de définir des gestionnaires d'événements pour être exécuté lors d'une réparation ou d'accueil des événements pour la 
  résolution proactive des problèmes
* Journal rotation automatique de fichier
* Prise en charge de la mise en œuvre supervision redondante d'hôtes
* Une interface web option pour visualiser état actuel du réseau, les notifications, l'histoire de problème, les fichiers journaux, etc.
* Stockage de données via des fichiers texte plutôt que de base de données
* Un design simple plugin qui permet aux utilisateurs de développer facilement leurs propres contrôles de service en fonction des besoins, en
  utilisant leurs outils de choix (scripts shell, C++, Perl, Ruby, Python, PHP, C#) etc
