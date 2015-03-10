=============
Run Command
=============

synopsis
------------

Les modules de commande RUN permet aux utilisateurs d'exécuter une commande du système d'exploitation. Ce est principalement utilisé dans un pilote automatique. L'utilisation de ce terme commande, l'utilisateur peut spécifier la commande, le nom de l'utilisateur et aussi pour exécuter le soit en arrière-plan ou front-end. Voyons les utilisations de commande de marche.

Commande Aide
---------------------

La commande d'aide décrit les utilisations de commande de marche, sa fonctionnalité majeure, ses autres paramètres, les commandes utilisées pour exécuter une commande, et aussi sur la syntaxe pour spécifier la commande, le nom de l'utilisateur et aussi pour exécuter le soit en arrière-plan ou l'avant -fin. La syntaxe utilisée pour déclarer la commande d'aide est indiqué ci-dessous.

.. code-block:: bash

		ptdeploy RunCommand help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptdeploy RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************


Comment utiliser la commande Exécuter
-------------------------------------------


La syntaxe utilisée pour spécifier l'ordre de marche dans illustré ci-dessous.

.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered


 +------------------------+-------------------------------------------------+--------------------------------------------------------+
 | Parameter              | fonction                                        | usage                                                  |
 +========================+=================================================+========================================================+
 |command=”ls -lah /tmp”  | Il permet à l'utilisateur de spécifier la       | En utilisant ce, l'utilisateur peut spécifier leur     |
 |                        | commande et son but.                            | propre commande selon leurs besoins.                   |
 +------------------------+-------------------------------------------------+--------------------------------------------------------+
 |run-as-user=”ubuntu”    | En utilisant ce que l'utilisateur peut          | En utilisant ce, l'utilisateur peut spécifier leur     |
 |                        | spécifier le nom de l'utilisateur.              | identifiant d'utilisateur requis selon leurs besoins.  |
 +------------------------+-------------------------------------------------+--------------------------------------------------------+
 |” –background           | Il permet à l'utilisateur de spécifier où pour  | En utilisant ce, l'utilisateur peut spécifier la       |
 |                        | exécuter la commande particulière, soit en      | plateforme de leur utilisation selon leurs besoins.    |
 |                        | arrière-plan ou dans le front-end.|             |                                                        |
 +------------------------+-------------------------------------------------+--------------------------------------------------------+



La syntaxe et la table comme décrit ci-dessus peut aide à l'utilisateur comment utiliser la commande de marche.

avantages
------------

* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
* Les utilisateurs peuvent spécifier la commande, le nom de l'utilisateur et aussi pour exécuter le either in background or front-end.
* The help command guides the users in how to execute the run command an also its purpose.

