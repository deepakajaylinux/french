========
PhpUnit
========

Synopsis
----------

PHPUnit est une infrastructure de test unit pour le langage de programmation PHP en tesingkamen. C'est une instance de l'architecture des infrastructures de tests unitaires qui a pris naissance avec initialise la suite de tests de php et est devenu populaire avec pttest.

Il fonctionne de deux façons. Ils sont init et exécutent. Il est utile de travailler avec Ubuntu et centos.


Commande Aide
---------------

La commande help conduit les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans les modules de Phpunit. La commande help répertorie les paramètres alternatifs de Phpunit dans le module pttest. Il décrit également la syntaxe de l'initialisation d'ordinateur de l'utilisateur. La commande help pour phpunit est illustrée ci-dessous.


.. code-block:: bash
	
	pttest phpunit help

La syntaxe pour la commande help non respect de la casse qui ajoute un avantage pour ce module. La capture d'écran suivante visualiser l'utilisateur sur la commande aide dans la détection des systèmes.

.. code-block:: bash

 kevell@corp:/# pttest PHPUnit help
 ******************************


  This command allows you to initialize a PHPUnit test suite.

  PHPUnit, phpunit

        - init, initialize
        Initialises the PHPUnit test suite of this project
        example: pttest phpunit init
        example: pttest phpunit initialize

        - execute
        Executes the PHPUnit test suite of this project
        example: pttest phpunit execute

 ------------------------------
 End Help
 ******************************


Alternative Paramètre
---------------------------

Au lieu d'utiliser phpunit, l'utilisateur peut utiliser les paramètres suivants d'altenative.


PHPUnit,  phpunit


Initialiser
--------------

Il initialise la suite phptest de ce projet. Cela peut instruire l'usager à l'usage commun de mettre en place chargement automatique pour les classes qui doivent être testés de script. La commande d'init est comme suit,

.. code-block:: bash

	pttest phpunit init

Après avoir saisi le système peut remettre en question comme PHPUnit initialiser ? O/N. Cela peut s'expliquer par thefollowing capture d'écran.

.. code-block:: bash

 kevell@corp:/# pttest phpunit init
 Initialize PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79746566500.sh
 chmod 755 /tmp/ptconfigure-temp-script-79746566500.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79746566500.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79746566500.sh
 Temp File /tmp/ptconfigure-temp-script-79746566500.sh Removed
 Creating /tmp/ptconfigure-temp-script-57284647129.sh
 chmod 755 /tmp/ptconfigure-temp-script-57284647129.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-57284647129.sh Permissions
 Executing /tmp/ptconfigure-temp-script-57284647129.sh
 Temp File /tmp/ptconfigure-temp-script-57284647129.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitInit: Success

 ------------------------------
 Installer Finished
 ******************************


Exécuter
-------------

Cette exécution permet à l'utilisateur à exécute la suite de tests PHPUnit de pttest. Programmes pour un système peuvent exécuter dans un processus discontinu sans interaction humaine, ou un utilisateur peut saisir des commandes dans une session interactive d'un interprète. La commande suivante est utilisée pour exécuter phpunit.

.. code-block:: bash

	pttest phpunit execute

Après avoir tapé la commande il poser une question. Il peut être visualisé par l'image suivante.

.. code-block:: bash

 kevell@corp:/# pttest phpunit execute
 Execute PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-23757829034.sh
 chmod 755 /tmp/ptconfigure-temp-script-23757829034.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23757829034.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23757829034.sh
 /tmp/ptconfigure-temp-script-23757829034.sh: 3: /tmp/ptconfigure-temp-script-23757829034.sh: phpunit: not found
 Temp File /tmp/ptconfigure-temp-script-23757829034.sh Removed
 Creating /tmp/ptconfigure-temp-script-85280710426.sh
 chmod 755 /tmp/ptconfigure-temp-script-85280710426.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-85280710426.sh Permissions
 Executing /tmp/ptconfigure-temp-script-85280710426.sh
 Temp File /tmp/ptconfigure-temp-script-85280710426.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitExec: Success

 ------------------------------
 Installer Finished
 ******************************


options
--------------


.. cssclass:: table-bordered

 +------------------------------+-----------------------+--------------------------------------------------+
 | paramètres			| options		| commentaires	                           	   |
 +==============================+=======================+==================================================+
 |Initialize Phpunit? (Y/N)	| Yes			| phpunit peut être initialisé en vertu pttest .   |
 +------------------------------+-----------------------+--------------------------------------------------+
 |Execute Phpunit? (Y/N)	| Yes			| PHPUnit peut être exécuté en vertu pttest .      |
 +------------------------------+-----------------------+--------------------------------------------------+
 |Initialize Phpunit/Execute 	| No			| Il peut quitter l'écran			   |
 |Phpunit? (Y/N)|		|			|					 	   |
 +------------------------------+-----------------------+--------------------------------------------------+


Avantages
----------

* PHPUnit a été créé avec la vue que plus vite vous détectez vos erreurs de code, plus vite vous pouvez corriger.  
* Comme toutes les infrastructures de test unité PHPUnit utilise des assertions pour vérifier que le comportement de l'unité de code sous test   se comporte comme prévu. 
* PHPUnit peut produire des résultats des tests dans un certain nombre de différents formats tels que xml. 
* Phpunit peut être une sensibilité sans respect. * Phpunit confort avec Ubuntu et centOS.

