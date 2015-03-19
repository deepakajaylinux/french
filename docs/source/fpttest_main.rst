PTTest
==============

synopsis
------------

Le pttest vise à la configuration et l'exécution d'automatisation gestion des tests à l'aide de php.

Il utilise un ensemble commun de règles dans un éventail d'outils et de technologies pour la gestion de la configuration de test suite et l'exécution.

Il fournit une API commune permettant d'exécuter des tests dans un large éventail de langues et outils de test. L'utilisateur peut exécuter des suites de tests complexes avec peu ou aucune configuration supplémentaire requise. Il nourrit les tests utilisateurs en manuel ou en utilisant un système d'exploitation et à la main assure la stabilité de l'environnement.

Il est modulaire, orienté objet et extensible. Donc si les utilisateurs se sent des modules supplémentaires au besoin ils peuvent encadrer et ajouter leur propre module selon leurs exigences.  

Il appartient à une suite d'outils de Pharaon qui enveloppe la gestion de la Configuration, gestion d'Automation de Test, le déploiement automatisé, Équipez et gestion des versions et plus, le tout mis en œuvre dans le code et tout en PHP.

Commande Aide
-------------------

Si vous voulez connaître le but d'un module particulier, il suffit de taper la commande suivante :

.. code-block:: bash

	pttest ModuleName help

Cette commande permettra l'utilisation de ce module particulier et également les options disponibles dans les actions que vous pouvez effectuer. La capture d'écran sous explique l'utilisation de la behat module sous pttest à l'aide de la commande help.


La commande help répertorie également les autres paramètres qui peuvent être utilisés dans la déclaration.


.. code-block:: bash

 kevell@corp:/# pttest Behat help
 ******************************


  This command allows you to initialize a Behat test suite.

  Behat, behat

        - init, initialize
        Initialises the Behat test suite of this project
        example: pttest behat init
        example: pttest behat initialize

        - execute
        Executes the Behat test suite of this project
        example: pttest behat execute

 ------------------------------
 End Help
 ******************************

Installation
----------------

Installation de la pttest peut se faire de deux manières possibles, selon la disponibilité et les exigences des utilisateurs. Ils ont deux façons d'installer pttest sont :


* Installing pttest via ptconfigure	
* Installing the pttest without depending on ptconfigure.

Pttest d'installation via ptconfigure
---------------------------------------------

Si l'utilisateur a le ptconfigure dans leur machine, puis c'est le moyen le plus simple d'installer pttest en utilisant la commande suivante :


.. code-block:: bash

	sudo ptconfigure pttest install --yes --guess

Installer le pttest sans fonction ptconfigure 
--------------------------------------------------------------

Si l'utilisateur souhaite installer le pttest sans fonction et à l'aide de la ptconfigure ils peuvent utiliser la commande suivante :


.. code-block:: bash

	sudo apt-get install php5 git

.. code-block:: bash

	git clone https://github.com/phpengine/pttest && sudo php pttest/install-silent

or

La commande ci-dessous est prévisible pour les utilisateurs qui souhaitent pour spécifier l'emplacement pendant l'installation.


.. code-block:: bash

	git clone https://github.com/phpengine/pttest && sudo php pttest/install

Comment utiliser et Modules disponibles 
---------------------------------------------

Voyons, comment utiliser l'outil pttest, tout d'abord, il suffit de taper comme


.. code-block:: bash

	pttest

Cette commande liste tous les noms des modules qui sont disponibles sous pttest. La capture d'écran suivante qui représente visuellement.


.. code-block:: bash

 kevell@corp:/# pttest 
 ******************************


 PTTest by Golden Contact Computing
 -------------------

 About:
 -----------------
 pttest is for Test Automation. It can be used to generate starter test suites for your applications,
 and automated test execution scripts within minutes.

 By providing an common API by which to execute tests in a wide range
 of languages and test tools, you can run complex test suites across a range of platforms with little to no
 extra configuration.

 -------------------------------------------------------------

 Available Commands:
 ---------------------------------------

 Autopilot - ptconfigure Autopilot - User Defined Installations
 Behat - Behat - Initialize or Execute a Behat Test Suite
 Cucumber - Cucumber - Initialize or Execute a Cucumber Test Suite
 EnvironmentConfig - Environment Configuration - Configure Environments for a project
 PHPUnit - PHPUnit - Initialize or Execute a PHPUnit Test Suite
 SystemDetection - System Detection - Detect the Running Operating System
 Templating - Templating
 Testify - Testifyer - Creates default tests for your project

 ******************************

Jouer avec les Modules PTTest 
------------------------------------

.. toctree::
   :maxdepth: 6
 
 fbehat_test
 fcucumber_test
 fenvironmentconfig_test 
 fphpunit_test
 fsystemdetection_test
 ftemplating_test







