=============
NginxServer
=============



Synopsis
---------

Nginx, prononcé «moteur X", est un serveur Web haute performance. Le Nginx Web Server est un poids léger et un serveur polyvalent qui peut être configuré pour toutes les différentes tâches que de nombreux sites modernes demande. Ngnix serveur agit comme un facilitateur pour les utilisateurs dans la configuration des paramètres des applications. Quelques exemples pour paramètres d'applications comprend utilisateur admin mysql, hôte, passe. Nginx fait les manchettes que le nouveau serveur Web de choix pour de nombreux webmasters. La principale raison de sa popularité est sa vitesse. Nginx est plus rapide que Apache dans des environnements non-test parce que son architecture est event driven tout Apache est processus piloté. Les modules de ptconfigure agit comme un chemin à travers pour l'installation de ce serveur Nginx.

Commande Aide
-----------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module de serveur Ngnix. La commande help répertorie les autres paramètres de serveur Ngnix. Il décrit également la syntaxe pour installer le serveur Ngnix. La commande d'aide pour le serveur Ngnix est donnée ci-dessous.

.. code-block:: bash

	ptconfigure nginx-server help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de Nginx Server.

.. code-block:: bash


	kevell@corp:/# ptconfigure NginxServer help
	******************************


	This command is part of Core and provides you  with a method by which you can configure Application Settings.
	You can configure default application settings, ie: mysql admin user, host, pass

	NginxServer, nginx-server, nginxserver

        - install
        Installs Nginx HTTP Server
        example: ptconfigure nginx-server install

	------------------------------
	End Help
	******************************


installation
--------------

Installation du serveur Nginx est plus simple en utilisant la commande suivante comme indiqué:

.. code-block:: bash

	ptconfigure nginx-server install

Après avoir saisi la commande ci-dessus les opérations suivantes comme indiqué dans le format tabulaire se produit.

.. cssclass:: table-bordered

 +-------------------------+----------------------------------------------------+------------+--------------------------------------------+
 | paramaters              | Alternative Paramètre                              | options    | commentaires                               |
 +=========================+====================================================+============+============================================+
 |ptconfigure nginx-server | au lieu de Nginx Server, Les solutions suivantes   | Y(Yes)     | Si l'utilisateur souhaite procéder le      |
 |install? (Y/N)           | peuvent également être utilisés: NginxServer,      |            | processus d'installation qu'ils peuvent    |
 |                         | nginx-server, nginxserver.                         |            | entrée comme Y.                            |
 +-------------------------+----------------------------------------------------+------------+--------------------------------------------+
 |ptconfigure nginx-server | au lieu de Nginx Server, Les solutions suivantes   | N(No)      | Si l'utilisateur souhaite quitter le       | 
 |install? (Y/N)           | peuvent également être utilisés: NginxServer,      |            | processus d'installation qu'ils peuvent    |
 |                         | nginx-server, nginxserver.                         |            | entrée comme N.|                           |
 +-------------------------+----------------------------------------------------+------------+--------------------------------------------+

Si l'utilisateur procède le processus d'installation, le Nginx HTTP Server sera installé. Si le paquet de Nginx est existe déjà dans la machine de l'utilisateur, un message se affiche pour demander à l'utilisateur que Nginx est existe déjà dans cette machine. Enfin rapports sont générés avec des résultats clairs et le statut. La capture d'écran ci-dessous explique le processus mentionné ci-dessus imagée.

.. code-block:: bash
	

	Kevell@corp:/# ptconfigure nginx-server install
	
	Install Nginx Server? (Y/N) 
	y	
	*******************************
	*        Pharaoh Tools        *
	*         Nginx Server!       *
	*******************************
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
	nginx-common nginx-core
	Suggested packages:
	fcgiwrap nginx-doc
	The following NEW packages will be installed:
	nginx nginx-common nginx-core
	0 upgraded, 3 newly installed, 0 to remove and 278 not upgraded.
	Need to get 347 kB of archives.
	After this operation, 1,295 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-common all 1.4.6-1ubuntu3.1 [17.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-core amd64 1.4.6-1ubuntu3.1 [324 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx all 1.4.6-1ubuntu3.1 [5,218 B]
	Fetched 347 kB in 3s (104 kB/s)
	Selecting previously unselected package nginx-common.
	(Reading database ... 168194 files and directories currently installed.)
	Preparing to unpack .../nginx-common_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx-common (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx-core.
	Preparing to unpack .../nginx-core_1.4.6-1ubuntu3.1_amd64.deb ...
	Unpacking nginx-core (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx.
	Preparing to unpack .../nginx_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	ureadahead will be reprofiled on next reboot
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for man-db (2.6.7.1-1) ...
	Setting up nginx-common (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Setting up nginx-core (1.4.6-1ubuntu3.1) ...
	Setting up nginx (1.4.6-1ubuntu3.1) ...
	[Pharaoh Logging] Adding Package nginx from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	NginxServer: Success
	------------------------------
	Installer Finished
	******************************


avantages
----------

* En utilisant ce Nginx serveur, l'utilisateur peut configurer leurs paramètres de l'application.
* Les paramètres utilisés dans les opérations d'aide et d'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Nginx est rapide car il ne est pas nécessaire de créer un nouveau processus pour chaque nouvelle demande.
* Nginx utilise très peu de mémoire, en particulier pour les pages Web statiques.
* Nginx peut être utilisé avec une gamme de systèmes.
* Nginx est hautement évolutive, et la performance ne dépend pas de matériel.
* Nginx est facile à installer et à configurer.
* Comme Apache, Nginx a toutes les fonctionnalités que vous attendez d'un serveur Web leader:
* Fichier statique servir.
* Support SSL / TLS.
* Les hôtes virtuels.
* Inverse proxy.
* L'équilibrage de charge.
* La compression.
* Les contrôles d'accès.
* La réécriture d'URL.
* Journalisation personnalisée.
* Côté serveur comprend.
* WebDAV.
* FLV streaming.
* FastCGI.
