===========
Dapperfy
===========

synopsis
------------

Dapperfy est une partie amende de module de base par défaut qui aide et soutient les utilisateurs dans la création d'un ensemble standard de fichiers de pilotage automatique pour leurs projets. Les utilisateurs peuvent configurer les paramètres d'application par défaut. Par exemple: utilisateur admin mysql, hôte, passer.

Voyons comment utiliser les fonctions de liste standard et dapper dapper cadre de ce module parmi les sujets à venir.

Commande Aide
--------------------

La commande help enveloppe toutes les informations nécessaires concernant dapperfy tels que ses principales utilisations, la liste des paramètres de remplacement qui peut être utilisé dans la déclaration, ce sont fonction principale de dapperfy (Ex: standard, liste), et aussi la syntaxe utilisée pour déclarer ces fonctions intéressantes. La commande suivante est utilisée pour déclarer aide option sous dapperfy,

.. code-block:: bash


		ptdeploy Dapperfy help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptdeploy Dapperfy help
 ******************************


  This command is part of a default Module Core and provides you with a method by which you can
  create a standard set of Autopilot files for your project from the command line.
  You can configure default application settings, ie: mysql admin user, host, pass


  Dapperfy, dapperfy

        - list
        List all of the autopilot files in your build/config/ptdeploy/autopilots
        example: ptdeploy dapperfy list

        - standard
        Create a standard set of autopilots to manage
        example: ptdeploy dapperfy standard

        The start of the command will be ptdeploy autopilot execute *filename*

        
 --------------
  Drupal Module:

  The Drupal module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Drupal site. This module adds the 'drupal' action to dapperfy.

  - drupal
  create drupal tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy drupal --yes --guess

 --------------
  Joomla Module:

  The Joomla module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Joomla site. This module adds the 'joomla' action to dapperfy.

  - joomla, joomla30
  create joomla tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy joomla --yes --guess

  - joomla-ptvirtualize, joomla30-ptvirtualize
  create joomla tailored automated deployment ptdeploy autopilots for your ptvirtualize Virtual Machines
  example: ptdeploy dapperfy joomla-ptvirtualize --yes --guess
 --------------
  Wordpress Module:

  The Wordpress module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Wordpress site. This module adds the 'wordpress' action to dapperfy.

  - wordpress
  create wordpress tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy wordpress --yes --guess
 ------------------------------
 End Help
 ******************************


Comment utiliser Dapper standard
---------------------------------------

La commande utilisée pour dapperfy standard est indiqué ci-dessous,

.. code-block:: bash

		ptdeploy dapperfy standard

Après être entré dans l'ordre donné ci-dessus, le processus suivant comme décrit dans le tableau ci-dessous volonté se produit dans une base étape par étape.

.. cssclass:: table-bordered

 +------------------------+-----------------------------------+--------------+------------------------------------------------------------+
 | paramètre              | Autres paramètres                 | Option       | commentaires                                               |
 +========================+===================================+==============+============================================================+
 |Dapperfy This? (Y/N)    | au lieu de dapperfy nous pouvons  | Y(Yes)       | Si l'utilisateur souhaite procéder processus de            |
 |                        | utiliser, Dapperfy                |              | dapperfying qu'ils peuvent entrée comme Y.                 |
 +------------------------+-----------------------------------+--------------+------------------------------------------------------------+
 |Dapperfy This? (Y/N)    | au lieu de dapperfy nous pouvons  | N(No)        | Si l'utilisateur souhaite quitter le processus de          |
 |                        | utiliser, Dapperfy                |              | dapperfying qu'ils peuvent entrée comme N.                 |
 +------------------------+-----------------------------------+--------------+------------------------------------------------------------+
 |Use existing            |                                   | Y(Yes)       | Si l'utilisateur souhaite procéder avec les paramètres     | 
 |environment settings?   |                                   |              | d'environnement existantes qu'ils peuvent entrée           |
 |(Y/N)	                  |                                   |              | comme Y.                                                   |
 +------------------------+-----------------------------------+--------------+------------------------------------------------------------+
 |Use existing            |                                   | N(No)        | Si l'utilisateur souhaite continuer avec les nouveaux      |
 |environment settings?   |                                   |              | paramètres de l'environnement qu'ils peuvent entrée        |
 |(Y/N)	                  |                                   |              | comme N.                                                   |
 +------------------------+-----------------------------------+--------------+------------------------------------------------------------+
 |Do you want to add      |                                   | Y(Yes)       | Si l'utilisateur souhaite ajouter un autre environnement   |
 |another environment?    |                                   |              | pour dapperfying qu'ils peuvent entrée comme Y.            |
 |(Y/N)                   |                                   |              |                                                            |
 +------------------------+-----------------------------------+--------------+------------------------------------------------------------+
 |Do you want to add      |                                   | N(No)        | Si l'utilisateur n'a pas besoin d'ajouter un autre         |
 |another environment?	  |                                   |              | environnement pour dapperfying qu'ils peuvent entrée       |
 |(Y/N)                   |                                   |              | comme N.|                                                  |
 +------------------------+-----------------------------------+--------------+------------------------------------------------------------+


Les deux types de captures d'écran différents peuvent être utiles pour les utilisateurs dans la définition d'une représentation picturale du processus de dapperfying. La seconde capture d'écran illustre méthode de spécification volonté en utilisant les paramètres d'environnement existants.


.. code-block:: bash


 kevell@corp:/# ptdeploy dapperfy standard
 Dapperfy This? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 ******************************


 Success
 In Dapperfy
 ******************************


Comment utiliser la liste Dapperfy
------------------------------------

L'objectif principal de la fonction de liste est de lister tous les fichiers du pilote automatique des projets des utilisateurs qui sont disponibles dans un emplacement particulier. La syntaxe pour utiliser la liste sous dapperfy est illustré ci-dessous,

.. code-block:: bash

                ptdeploy dapperfy list

La capture d'écran ci-dessous illustre le fonctionnement de l'option de liste sous dapperfy.




avantages
-----------

* Il est bien de choses à faire dans les deux Ubuntu et ainsi que dans cent OS.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse.
* L'utilisateur peut voir la liste des fichiers de pilotage automatique qui sont disponibles pour leurs projets.
* Bien que dapperfying, l'utilisateur peut spécifier les paramètres d'environnement qu'ils requièrent.
* De nombreux environnements peuvent être ajoutés à dapperfy.
