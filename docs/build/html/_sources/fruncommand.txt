=============
Run Command
=============

synopsis
-----------

Les modules de commande RUN permet aux utilisateurs d'exécuter des commandes du système d'exploitation. Ce est principalement être utilisé dans sur le pilote automatique. Grâce à cette commande, l'utilisateur peut spécifier exécuter la ligne de commande, le nom de l'utilisateur et donc d'exécuter le soit en arrière-plan ou front-end. Voyons les utilisations de commande de marche.

HelpCommand
----------------

La commande d'aide décrit les utilisations de commande de marche, ses principales fonctions à ce sujet, ses autres paramètres, les commandes utilisées pour exécuter une commande, et donc sur la syntaxe pour la spécification de la commande, le nom de l'utilisateur et donc d'exécuter l'une ou l'autre en arrière-plan ou l'avant -fin. La syntaxe utilisée pour déclarer la commande d'aide est indiqué ci-dessous.

.. code-block:: bash

		ptconfigure RunCommand help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptconfigure RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************


La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered

 
 +-----------------------+---------------------------------------------------+------------------------------------------------------+
 | paramètre             | fonction                                          | utilisation                                          |
 +=======================+===================================================+======================================================+
 |command=”ls -lah /tmp” | Il permet à l'utilisateur de spécifier la         | En utilisant ce, l'utilisateur peut spécifier        |
 |                       | commande et de son but.                           | leur propre instruction en fonction de leurs         |
 |                       |                                                   | exigences.                                           |
 +-----------------------+---------------------------------------------------+------------------------------------------------------+
 |run-as-user=”ubuntu”   | En utilisant ce, l'utilisateur peut spécifier le  | En utilisant ce, l'utilisateur peut spécifier        |
 |                       | nom de l'utilisateur.                             | l'enregistrement de l'utilisateur requis selon       |
 |                       |                                                   | leurs besoins.                                       |
 +-----------------------+---------------------------------------------------+------------------------------------------------------+
 |En utilisant ce,       | Il permet à l'utilisateur de spécifier l'endroit  | En utilisant ce, l'utilisateur peut spécifier la     |
 |l'utilisateur peut     | où la commande spécifique soit dans le fond ou    | plate-forme de leur utilisation en fonction de       |
 |spécifier la plate-    | dans le front-end terme.                          | leurs exigences.                                     |
 |forme de leur          |                                                   |                                                      |
 |utilisation en         |                                                   |                                                      |
 |fonction de leurs      |                                                   |                                                      |
 |besoins, "-background| |                                                   |                                                      |
 +-----------------------+---------------------------------------------------+------------------------------------------------------+


paramètres alternatifs
----------------------

nous pouvons utiliser les paramètres suivants,

RunCommand, runcommand, run-command


avantages
------------

* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire dans les deux Cent OS et ainsi que dans Ubuntu.
* Les utilisateurs peuvent spécifier la commande, le nom de l'utilisateur et donc d'exécuter l'une ou l'autre en arrière-plan ou front-end.
* La commande help guide les utilisateurs à la façon d'exécuter la commande de marche sur de sorte que son effet.
