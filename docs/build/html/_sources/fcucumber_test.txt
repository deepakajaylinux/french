============
Cucumber
============


synopsis
------------

Ce module aide l'utilisateur à initialiser et exécuter la suite de tests de concombre . Voyons comment initialiser et d'exécuter la suite de tests de concombre dans les sujets à venir .


Commande Aide
--------------------

La commande help guide l'utilisateur sur le but et les options disponibles en vertu d'un module. Il énumère les autres paramètres qui sont utilisés dans la déclaration . Il décrit la syntaxe pour initialiser et d'exécuter le concombre sous la pttest . La commande utilisée pour déclarer aide est indiqué ci-dessous :


.. code-block:: bash

	pttest cucumber help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide .


.. code-block:: bash

 kevell@corp:/# pttest cucumber help
 ******************************


  This command allows you to initialize a Cucumber test suite.

  Cucumber, cucumber

        - init, initialize
        Initialises the Cucumber test suite of this project
        example: pttest cucumber init
        example: pttest cucumber initialize

        - execute
        Executes the Cucumber test suite of this project
        example: pttest cucumber execute

 ------------------------------
 End Help
 ******************************


Comment initialiser le concombre
-----------------------------------

La commande utilisée pour initialiser le concombre sous pttest se affiche:


.. code-block:: bash

	pttest cucumber init

or 

.. code-block:: bash

	pttest cucumber initialize

Après avoir saisi la commande ci-dessus, le processus de initialize se produit comme le montre le tableau ci-dessous .



.. cssclass:: table-bordered

 +-----------------------------+--------------------------------------+----------+------------------------------------------------+
 | paramètres		       | paramètres alternatifs		      | options	 | commentaires		                          |
 +=============================+======================================+==========+================================================+
 |Initialize Cucumber? (Y/N)   | Au lieu de concombre, nous pouvons   | Y(Yes)	 | Si l'utilisateur souhaite procéder init        |
 | 			       | utiliser le concombre également.     | 	 | qu'ils peuvent entrée comme Y.                 |
 +-----------------------------+--------------------------------------+----------+------------------------------------------------+
 |Initialize Cucumber? (Y/N)   | Au lieu de concombre, nous pouvons   | N(No) 	 | Si l'utilisateur souhaite quitter le           | 
 |			       | cucumber also.			      | 	 | initialisation qu'ils peuvent entrée comme N.| |
 +-----------------------------+--------------------------------------+----------+------------------------------------------------+



Enfin, le concombre se pttest initialisé comme indiqué dans la capture d'écran suivante .



.. code-block:: bash


 kevell@corp:/# pttest cucumber init
 Initialize Cucumber? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Cucumber         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-81470621814.sh
 chmod 755 /tmp/ptconfigure-temp-script-81470621814.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-81470621814.sh Permissions
 Executing /tmp/ptconfigure-temp-script-81470621814.sh
 Temp File /tmp/ptconfigure-temp-script-81470621814.sh Removed
 Creating /tmp/ptconfigure-temp-script-65310697385.sh
 chmod 755 /tmp/ptconfigure-temp-script-65310697385.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-65310697385.sh Permissions
 Executing /tmp/ptconfigure-temp-script-65310697385.sh
 Temp File /tmp/ptconfigure-temp-script-65310697385.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Cucumber: Success

 ------------------------------
 Installer Finished
 ******************************


Comment exécuter le concombre
----------------------------------------

La commande utilisée pour exécuter le concombre sous pttest se affiche:


.. code-block:: bash

	pttest cucumber execute

Après avoir saisi la commande ci-dessus, le processus d'exécution se produit tel que représenté dans le tableau ci-dessous.


.. cssclass:: table-bordered


 +-----------------------------+--------------------------------------+----------+------------------------------------------------+
 | paramètres		       | paramètres alternatifs		      | options	 | commentaires		                          |
 +=============================+======================================+==========+================================================+
 |Execute Cucumber? (Y/N)      | Au lieu de concombre, nous pouvons   | Y(Yes)	 | Si l'utilisateur souhaite procéder à           |
 | 			       | utiliser le concombre également.     | 	 | l'exécution qu'ils peuvent entrée comme Y.     |
 +-----------------------------+--------------------------------------+----------+------------------------------------------------+
 |Execute Cucumber? (Y/N)      | Au lieu de concombre, nous pouvons   | N(No) 	 | Si l'utilisateur souhaite quitter le           | 
 |			       | utiliser le concombre également.     | 	 | processus d'exécution qu'ils peuvent entrée    |
 |                             |                                      |          | comme N.|                                      |
 +-----------------------------+--------------------------------------+----------+------------------------------------------------+


Si l'utilisateur de procéder à l'exécution , le processus d'exécution se produira comme illustré dans la capture d' écran ci-dessous .




avantages
------------


* Il est bien de choses à faire dans les deux cent OS et ainsi que dans ubuntu .
* Les paramètres utilisés dans la déclaration ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux autres.
* Ce concombre permet aux utilisateurs d' initialiser et d'exécuter la suite de tests de concombre .
