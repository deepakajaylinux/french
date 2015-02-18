=================
DeveloperTools
=================

synopsis
----------------

Le module devtools rend l'installation beaucoup plus facile de créer un package suivant la structure définie dans les Devtools. Il rend également plus facile de tester votre paquet, par éditeur. Ce module dans un emballage ayant une excellente idée: non seulement est-il le paquet utilisateur plus fiable sur le long terme, il simplifie également le processus de développement de manière surprenante. Ceci est approprié dans Ubuntu et CentOS.

Commande Aide
------------------------

Devtools rend le développement de package une brise: cela fonctionne avec les conventions existantes pour la structure du code, en ajoutant des outils efficaces pour soutenir le cycle de développement de package. Avec devtools, élaboration d'un ensemble devient si facile que ce sera la configuration par défaut de l'utilisateur lorsque l'utilisateur est en train d'écrire une quantité importante de code.

.. code-block:: bash

                cleopatra devtools help

La capture d'écran ci-dessous explique.

.. code-block:: bash

 kevell@corp:/# cleopatra devtools help
 ******************************


  This command allows you to install a set of Developer Tools. These include
  Geany IDE, Bluefish IDE, Kompozer IDE and Emma DB Manager.

  DeveloperTools, devtools, dev-tools

        - install
        Installs the latest version of Developer Tools
        example: cleopatra devtools install

 ------------------------------
 End Help
 ******************************

installation
------------------

L'installation comprend la fourniture ou la connexion aux services nécessaires pour rendre l'équipement installé prêt à fonctionner. Ce est un processus manifeste d'installer module devtools sous Cleopatra en utilisant simplement la commande ci-dessous,

.. code-block:: bash

	 cleopatra devtools install

Après dynamiser la commande il catéchiser entrée.

Lorsque l'entrée d'utilisateur comme il sera automatiquement oui installer devtools avec vérification du système. Si pas quitter l'installation. ce qui suit capture d'écran démontre.

.. code-block:: bash


 kevell@corp:/$ cleopatra devtools install
 Install Developer Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         Devel Tools!        *
 *******************************

 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  geany-common
 Suggested packages:
  libvte9
 The following NEW packages will be installed:
  geany geany-common
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 3,808 kB of archives.
 After this operation, 9,872 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe geany-common all 1.23.1+dfsg-1 [2,709 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe geany amd64 1.23.1+dfsg-1 [1,100 kB]
 Fetched 3,808 kB in 4min 54s (12.9 kB/s)
 Selecting previously unselected package geany-common.
 (Reading database ... 182047 files and directories currently installed.)
 Preparing to unpack .../geany-common_1.23.1+dfsg-1_all.deb ...
 Unpacking geany-common (1.23.1+dfsg-1) ...
 Selecting previously unselected package geany.
 Preparing to unpack .../geany_1.23.1+dfsg-1_amd64.deb ...
 Unpacking geany (1.23.1+dfsg-1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up geany-common (1.23.1+dfsg-1) ...
 Setting up geany (1.23.1+dfsg-1) ...
 Preparing to unpack .../bluefish-data_2.2.5-1_all.deb ...
 Unpacking bluefish-data (2.2.5-1) ...
 Selecting previously unselected package bluefish-plugins.
 Preparing to unpack .../bluefish-plugins_2.2.5-1_amd64.deb ...
 Unpacking bluefish-plugins (2.2.5-1) ...
 Selecting previously unselected package bluefish.
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for shared-mime-info (1.2-0ubuntu3) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Setting up bluefish-data (2.2.5-1) ...
 Setting up bluefish-plugins (2.2.5-1) ...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/AppConfig.php on line 115
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 DeveloperTools: Success
 ------------------------------
 Installer Finished
 ******************************

Options
-------------

.. cssclass:: table-bordered

 +-------------------+----------------------------------+--------+---------------------------------------------+
 | Paramètres        | Alternate parameter              | Option | Commentaires                                |
 +-------------------+----------------------------------+--------+---------------------------------------------+
 |Install devtools?  | Au lieu d'utiliser  devtools     | Y      | Il va installer éditeur et base de données  | 
 |(Y/N) 	     | nous pouvons utiliser Developer  |        | de données devtools sous cleopatra          |
 |                   | Tools, devtools,dev-tools 	| 	 | devtools sous cleopatra                     |
 +-------------------+----------------------------------+--------+---------------------------------------------+
 |Install devtools?  | Au lieu d'utiliser  devtools     | N      | La sortie du système d'installation         |
 |(Y/N) 	     | nous pouvons utiliser Developer  |        |                                             |
 |                   | Tools, devtools,dev-tools| 	| 	 |                                             |
 +-------------------+----------------------------------+--------+---------------------------------------------+
                       

Avantages
----------------

* Faciliter le processus de développement de l'emballage
* Aider à libérer votre colis dans la nature
* Assurez-il facile à installer et éditeur de base de données.
* Mise au point rapide
* Sur-le-Fly modifications de style - Pour les changements de style rapide, l'utilisateur ne même pas besoin d'utiliser un éditeur de texte. 
  L'utilisateur peut inspecter l'élément particulier sur la page pour déterminer quels styles sont appliquées.



