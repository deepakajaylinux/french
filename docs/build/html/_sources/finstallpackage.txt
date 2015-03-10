===============
InstallPackage
===============


synopsis
------------------

Installer le paquet sont sorties logiques différentiels couramment utilisés dans les circuits de distribution d'horloge à grande vitesse. Cette commande permet à l'utilisateur d'installer le paquet, construire serveur, client de dev, serveur de test, serveur de dev, la production. Cette fonction principale de commande est à la liste préconfigurée de logiciels. Il est adapté avec Ubuntu et CentOS.

Commande Aide
-----------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules de InstallPackage. La commande help répertorie les autres paramètres de InstallPackage le cadre du module de ptconfigure. Il décrit également la syntaxe pour l'installation. La commande d'aide pour le module de InstallPackage est illustré ci-dessous.

.. code-block:: bash

		ptconfigure installpackage help


La capture d'écran ci-dessous montre l'effort complète de module de InstallPackage.

.. code-block:: bash

 kevell@corp:/# ptconfigure InstallPackage help

 ******************************


  This command is part of Core and provides you  with a method by which you can perform some default CLI Installs of
  different types of box.

  InstallPackage, installpackage, installpack, install-pack, install, inpack, install-package

    - dev-client
      install a dev client machine for you to work on, a bunch of IDE's, DB's and a complete set of the
      tools you need to start work immediately.
      example: ptconfigure install autopilot dev-client

    - dev-server
      Install the preconfigured list of software for a developers server.
      example: ptconfigure install autopilot dev-server

    - test-server
      Install the preconfigured list of software for a testing server.
      example: ptconfigure install autopilot test-server

    - build-server
      Install the preconfigured list of software for a build server.
      example: ptconfigure install autopilot test-server

    - production
      Install the preconfigured list of software for a production server.
      example: ptconfigure install autopilot test-server

 ------------------------------
 End Help
 ******************************
 


installation
---------------

L'installation comprend l'installation de InstallPackage nécessaire pour faire l'installation dans une version mise à jour. Ce est un processus manifeste pour installer le module InstallPackage sous ptconfigure. InstallPackage en utilisant simplement la commande ci-dessous,

.. code-block:: bash

	ptconfigure installpackage Install

Après dynamiser la commande il catéchiser entrée.

Lorsque l'entrée d'utilisateur comme il sera automatiquement oui installer InstallPackage avec vérification du système. Si pas quitter l'installation. La capture d'écran suivante démontre InstallPackage et ses fonctions.

.. code-block:: bash




paramètres alternatifs
-------------------------------

Voici les autres paramètres qui peuvent être définis dans les déclarations:

InstallPackage, installpackage, installpack, install, inpack, installpackage.

Dev-client
---------------

Cette commande est utilisée pour travailler sur un tas de développement intégré de l'environnement, Base de données et un ensemble complet d'outils que l'utilisateur nécessité de commencer à travailler immédiatement. La commande suivante utilisée pour la machine client dev.

.. code-block:: bash

		ptconfigure install autopilot dev-client

Après entrée comme ci-dessus ladite commande il commence l'installation de processus.

Le cliché suivant montre ses fonctions.

.. code-block:: bash


Dev-serveur
----------------

Cette commande utilisé pour installer liste des préconfigure de logiciels pour le serveur d'un développeur. Pilote automatique agit comme un rôle essentiel dans ce processus. Pour travailler sur ces fonctions correctement ptconfigure recommande dev-serveur en utilisant cette commande.

.. code-block:: bash

		ptconfigure install autopilot dev-server

Guide l'utilisateur sur sa fonction La capture d'écran.

.. code-block:: bash

Test-serveur
-----------------

Voici pilote Auto agit un rôle majeur dans le serveur de test. Il utilise pour installer la liste préconfigurée de logiciels pour serveur de test. Logiciel de test également disponible. La commande suivante permet d'installer le serveur de test.

.. code-block:: bash

		ptconfigure install autopilot test-server


Guide l'utilisateur sur sa fonction La capture d'écran.

.. code-block:: bash


construire serveur
-------------------

Cette commande utilisé pour installer liste des préconfigure du logiciel pour un serveur de build. Pilote automatique agit comme un rôle essentiel dans ce processus. Pour travailler sur ces fonctions correctement ptconfigure recommande construire-serveur en utilisant cette commande.

.. code-block:: bash

	ptconfigure install autopilot build-server


Guide l'utilisateur sur sa fonction La capture d'écran.


.. code-block:: bash

production
-----------------

Cette commande utilisé pour installer liste des préconfigure de logiciels pour un serveur de production. Pilote automatique agit comme un rôle essentiel dans ce processus. Pour travailler sur ces fonctions recommande correctement ptconfigure serveur de production en utilisant cette commande.

.. code-block:: bash

		ptconfigure install autopilot build-server

Guide l'utilisateur sur sa fonction La capture d'écran.

.. code-block:: bash



avantages
-------------

* Sensibilité non de cas.
* Eh bien-to-do dans Ubuntu et CentOS.
* Installation dev-serveur, dev-client, la production, la construction-serveur, test-server est un atout supplémentaire pour ce module.
* Pilote automatique agit comme un rôle vital.


