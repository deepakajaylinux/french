=========
Behat
=========

synopsis
------------

Ce module permet à l'utilisateur d'initialiser Behat suite de tests . Le Behat aide à tester un script php . Il peut mettre en évidence les modèles activés et désactivés . Voyons comment init et exécuter le Behat de pttest .


Commande Aide

---------------------
La commande help guide l'utilisateur sur le but et les options disponibles en vertu d'un module. Il énumère les autres paramètres qui sont utilisés dans la déclaration . Il décrit la syntaxe pour initialiser et d'exécuter un Behat sous la pttest . La commande utilisée pour déclarer aide est indiqué ci-dessous :


.. code-block:: bash

	pttest behat help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide .


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


Comment initialiser Behat

-----------------------------

La commande utilisée pour initialiser la Behat sous pttest se affiche:


.. code-block:: bash

	pttest behat init

or 

.. code-block:: bash

	pttest behat initialize


Après avoir saisi la commande ci-dessus, le processus de initialize se produit comme le montre le tableau ci-dessous .



.. cssclass:: table-bordered

 +------------------------+----------------------------------------+---------+-----------------------------------------+
 | paramètres	          | paramètres alternatifs	           | options |	commentaires			       |
 +========================+========================================+=========+=========================================+
 |Initialize Behat? (Y/N) | Au lieu de Behat , nous pouvons        | Y(Yes)  | Si l'utilisateur souhaite procéder init |
 |			  | utiliser également Behat		   |	     | qu'ils peuvent entrée comme Y.          |
 +------------------------+----------------------------------------+---------+-----------------------------------------+
 |Initialize Behat? (Y/N) | Au lieu de Behat , nous pouvons        | N(No)   | Si l'utilisateur souhaite quitter le    |
 |			  | utiliser également Behat		   |	     | processus d'initialisation qu'ils       |
 |                        |                                        |         | peuvent entrée comme N.|                |      
 +------------------------+----------------------------------------+---------+-----------------------------------------+



Enfin, le pttest Behat se initialisé comme indiqué dans la capture d'écran suivante .


.. code-block:: bash

 kevell@corp:/# pttest behat init
 Initialize Behat? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Behat         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-72748278108.sh
 chmod 755 /tmp/ptconfigure-temp-script-72748278108.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-72748278108.sh Permissions
 Executing /tmp/ptconfigure-temp-script-72748278108.sh
 /tmp/ptconfigure-temp-script-72748278108.sh: 3: /tmp/ptconfigure-temp-script-72748278108.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-72748278108.sh Removed
 Creating /tmp/ptconfigure-temp-script-35600300430.sh
 chmod 755 /tmp/ptconfigure-temp-script-35600300430.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-35600300430.sh Permissions
 Executing /tmp/ptconfigure-temp-script-35600300430.sh
 Temp File /tmp/ptconfigure-temp-script-35600300430.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************


Comment exécuter l' Behat
---------------------------

La commande utilisée pour exécuter le Behat sous pttest se affiche:


.. code-block:: bash

	pttest behat execute


Après avoir saisi la commande ci-dessus, le processus d'exécution se produit tel que représenté dans le tableau ci-dessous.



.. cssclass:: table-bordered 
 

 +------------------------+----------------------------------------+---------+---------------------------------------------+
 | paramètres             | paramètres alternatifs                 | options | commentaires                                |
 +========================+========================================+=========+=============================================+
 |Execute Behat? (Y/N)    | Au lieu de Behat , nous pouvons        | Y(Yes)  | Si l'utilisateur souhaite procéder          |
 |			  | utiliser également Behat		   |	     | d'exécution qu'ils peuvent entrée comme Y.  |
 +------------------------+----------------------------------------+---------+---------------------------------------------+
 |Execute Behat? (Y/N)    | Au lieu de Behat , nous pouvons        | N(No)   | Si l'utilisateur souhaite quitter le        |
 |			  | utiliser également Behat		   |	     | processus d'exécution qu'ils                |
 |                        |                                        |         | peuvent entrée comme N.|                    |      
 +------------------------+----------------------------------------+---------+---------------------------------------------+



Si l'utilisateur de procéder à l'exécution , le processus d'exécution se produira comme représenté dans la capture d'écran suivante .


.. code-block:: bash

 kevell@corp:/# pttest behat execute
 Execute Behat? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *            Behat!           *
 *******************************
 Creating /tmp/ptconfigure-temp-script-93439425208.sh
 chmod 755 /tmp/ptconfigure-temp-script-93439425208.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-93439425208.sh Permissions
 Executing /tmp/ptconfigure-temp-script-93439425208.sh
 /tmp/ptconfigure-temp-script-93439425208.sh: 2: /tmp/ptconfigure-temp-script-93439425208.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-93439425208.sh Removed
 Creating /tmp/ptconfigure-temp-script-97268122064.sh
 chmod 755 /tmp/ptconfigure-temp-script-97268122064.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-97268122064.sh Permissions
 Executing /tmp/ptconfigure-temp-script-97268122064.sh
 Temp File /tmp/ptconfigure-temp-script-97268122064.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************


avantages
-----------

* Il guide les utilisateurs à identifier les erreurs de script php .
* Utilisation des fonctions de Behat les utilisateurs peuvent définir et spécifier le comportement de développement piloté .
* Le processus d' initialisation et l'exécution peut être fait en vertu du présent Behat de pttestt .
* Il est bien de choses à faire dans les deux cent OS et ainsi que dans ubuntu .
* Les paramètres utilisés dans la déclaration ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux autres.

