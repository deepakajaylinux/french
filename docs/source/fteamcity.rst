=================
Teamcity 
=================

synopsis
---------

Teamcity est une gestion de construction basé sur Java et le serveur d'intégration continue. Ce module vise à installer la dernière version du serveur Teamcity et ses dépendances.

Commande Aide
-----------------

La commande help guide l'utilisateur à fournir ce qui est nécessaire pour accomplir la tâche. La commande de faire usage de l'aide sous la borne est donnée comme suit,

.. code-block:: bash

	ptconfigure Teamcity help

Le cliché ci-dessous vous donne une représentation picturale de commande d'aide et il a énuméré deux paramètres que Teamcity et TeamCity. (Les paramètres sont insensibles à la casse)

.. code-block:: bash

	kevell@copy:/# ptconfigure teamcity help
	******************************


	This command allows you to install Teamcity, the popular Build Server.

	Teamcity, teamcity

        - install
        Installs Teamcity from the Jetbrains distributed native package
        example: ptconfigure teamcity install

	------------------------------
	End Help
	******************************


installation
-------------

La commande utilisée pour installer le module Teamcity est donnée ci-dessous,

.. code-block:: bash

	ptconfigure Teamcity install


La capture d'écran ci-dessous explique comment installer module de TeamCity.

.. code-block:: bash


	kevell@corp:/# ptconfigure Teamcity install
	Install Teamcity? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Teamcity !        *
	*******************************
	PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/Teamcity/Model/TeamcityUbuntu.php on line 42
	[Pharaoh Logging] Ensure module install is not checking versions
	[Pharaoh Logging] Module Java reports itself as Installed
	[Pharaoh Logging] Not installing as already installed
	Creating /tmp/ptconfigure-temp-script-82478215982.sh
	chmod 755 /tmp/ptconfigure-temp-script-82478215982.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-82478215982.sh Permissions
	Executing /tmp/ptconfigure-temp-script-82478215982.sh
	--2015-01-08 14:42:15--  http://download.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download.jetbrains.com (download.jetbrains.com)... 54.217.236.18
	Connecting to download.jetbrains.com (download.jetbrains.com)|54.217.236.18|:80... connected.
	HTTP request sent, awaiting response... 302 Moved Temporarily
	Location: http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz [following]
	--2015-01-08 14:42:16--  http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download-cf.jetbrains.com (download-cf.jetbrains.com)... 54.230.190.208, 54.230.190.220, 54.230.190.210, ...
	Connecting to download-cf.jetbrains.com (download-cf.jetbrains.com)|54.230.190.208|:80... connected.
	HTTP request sent, awaiting response... 200 OK
	Length: 551078596 (526M) [application/x-tar]
	Saving to: ‘TeamCity-8.1.3.tar.gz’
		
	 99% [                                                                                                   >  ] 60,46,771   63.3KB/s 	



Options
---------

.. cssclass:: table-bordered

 +--------------------------+-----------+---------------------------------------------------------------+
 | paramètres               | options   | commentaires                                                  |
 +==========================+===========+===============================================================+
 |ptconfigure Teamcity      | Y(Yes)    | Cette commande va installer le module Teamcity                | 
 |install                   |           |                                                               |
 +--------------------------+-----------+---------------------------------------------------------------+
 |Install Teamcity (Y/N)    | Y         | Si l'utilisateur saisit Y, ce module vérifie exigences de     |
 |                          |           | support pour Teamcity si sorties Il a été actualisé à la      |
 |                          |           | nouvelle version ou bien il installe le nouveau package avec  |
 |                          |           | les exigences de soutien.                                     |
 +--------------------------+-----------+---------------------------------------------------------------+
 |Install Teamcity (Y/N)    | N         | Si l'utilisateur entre N, l'installation a été interrompue.|  |
 +--------------------------+-----------+---------------------------------------------------------------+



Avantages pour les utilisateurs
--------------------------------------

* Installe toutes les exigences de soutien de lancer le serveur de TeamCity de manière efficace
* L'utilisation de la facilité d'accès et l'installation
* Le codage est insensible à la casse.

