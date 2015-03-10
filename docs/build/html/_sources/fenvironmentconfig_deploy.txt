====================
EnvironmentConfig
====================

synopsis
-------------

Ce module facilite les utilisateurs à configurer leur environnement nécessaire à leur projet. Voyons comment configurer l'environnement, comment supprimer l'environnement indésirables, la façon d'utiliser l'option de liste énumérant les environnements disponibles dans les prochains sujets.

Commande Aide
--------------------

La commande help guide les utilisateurs au sujet de la fin du module, ses paramètres de remplacement qui sont utilisés dans la déclaration. Il met en évidence les trois fonctions de configuration de l'environnement qui sont liste, configurer, supprimer. Il précise également la syntaxe pour utiliser trois fonctions principales. La syntaxe utilisée pour déclarer l'aide est indiqué ci-dessous:

.. code-block:: bash

		ptdeploy  envconfig help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash


 kevell@corp:/# ptdeployEnvironmentConfig help
 ******************************


  This command is part of a default Module and provides you with a method by which you can
  configure environments for your project from the command line. Currently compliant with
  both ptdeployand Ptconfigure.


  EnvironmentConfig, environmentconfig, environment-config, envconfig, env-config

        - list
        List current environments
        example: ptconfigure envconfig list --yes

        - configure, config
        Configure the environments for your project to use
        example: ptconfigure envconfig config
        example: ptconfigure envconfig config --keep-current-environments

        - delete, del
        Configure the environments for your project to use
        example: ptconfigure envconfig delete
        example: ptconfigure envconfig del --environment-name="staging"


 ------------------------------
 End Help
 ******************************


Comment configurer l'environnement
----------------------------------------------

Aux fins de la configuration des environnements, l'utilisateur peut utiliser la commande suivante:

.. code-block:: bash

		ptdeployenvconfig config

Après avoir saisi la commande ci-dessus les opérations suivantes a lieu comme indiqué:

Étape 1: configurer des environnements ici? (Y / N)

L'utilisateur dispose à l'entrée Y ou N.

Étape 2: Utiliser les paramètres de l'environnement existantes? (Y / N)

L'utilisateur dispose à l'entrée Y ou N.

Si l'entrée de l'utilisateur en tant que Y, il sera procéder à déjà existant.

Se ils entrée comme N, il sera demande des informations sur l'environnement

Rapport: Nom de l'environnement

Rapport: Par défaut répertoire temp (Lieu)

Après les étapes ci-dessus, l'utilisateur doit saisir les détails suivants:

Entrez cibler?

Entrez utilisateur?

Entrez le mot de passe?

Ajouter un autre serveur? (Y / N)

L'utilisateur dispose à l'entrée Y ou N.

Enfin, la configuration de l'environnement obtient le succès comme le montre la capture d'écran ci-dessous.

.. code-block:: bash

 kevell@corp:/# ptconfigure envconfig config
 Configure Environments Here? (Y/N) 
 Y
 Environment 1  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 kevells
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /home/kevells
 Enter user ?
 kevells
 Enter password ?
 123456
 Add Another Server? (Y/N)
 N
 ******************************


 Success
 In Environment Configuration
 ******************************


Lors de la configuration d'un environnement, si l'utilisateur souhaite configurer avec l'environnement actuel, ils peuvent utiliser la commande suivante:

.. code-block:: bash

		ptdeployenvconfig config --keep-current-environments


Après avoir saisi la commande ci-dessus, il sera demande les détails suivants comme indiqué dans le format tabulaire:


.. cssclass:: table-bordered

 +------------------------------------------+-----------+--------------------------------------------------------------+
 | paramètre                                | Option    | commentaires                                                 |
 +==========================================+===========+==============================================================+
 |Configure Environments Here? (Y/N)        | Y(Yes)    | Si l'utilisateur souhaite configurer les environnements à    |
 |                                          |           | l'environnement actuel ils peuvent d'entrée comme Y          |
 +------------------------------------------+-----------+--------------------------------------------------------------+
 |Configure Environments Here? (Y/N)        | N(No)     | Si l'utilisateur ne souhaite pas configurer les              |
 |                                          |           | environnements à l'environnement actuel ils peuvent d'entrée |
 |                                          |           | comme N                                                      |
 +------------------------------------------+-----------+--------------------------------------------------------------+
 |Use existing environment settings? (Y/N)  | Y(Yes)    | Si l'utilisateur souhaite utiliser les paramètres            |
 |                                          |           | d'environnement existantes qu'ils peuvent entrée comme Y.    |
 +------------------------------------------+-----------+--------------------------------------------------------------+
 |Configure Environments Here? (Y/N)        | N(No)     | Si l'utilisateur ne souhaite pas utiliser les paramètres     |
 |                                          |           | d'environnement existantes qu'ils peuvent entrée comme N.    |
 +------------------------------------------+-----------+--------------------------------------------------------------+
 |Do you want to add another                | Y(Yes)    | Si l'utilisateur souhaite ajouter un autre environnement,    |
 |environment? (Y/N)	 	            |           | ils peuvent entrée comme Y.                                  |
 +------------------------------------------+-----------+--------------------------------------------------------------+
 |Do you want to add another                | N(No)     | Si l'utilisateur ne souhaite pas ajouter un autre            |
 |environment? (Y/N)	 	            |           | environnement, ils peuvent entrée comme N.|                  |
 +------------------------------------------+-----------+--------------------------------------------------------------+


La capture d'écran ci-dessous représente graphiquement le processus mentionné ci-dessus:

.. code-block:: bash


 kevells@corp:/# ptdeployenvconfig config --keep-current-environments
 Configure Environments Here? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 Y
 Do you want to add another environment? (Y/N) 
 N
 ******************************


 Success
 In Environment Configuration
 ******************************




Comment faire pour supprimer la configuration de l'environnement
------------------------------------------------------------------------

Si l'utilisateur doit supprimer la configuration de l'environnement, ils peuvent saisir la commande suivante:

.. code-block:: bash

	ptdeployenvconfig del --environment-name="kevells"

L'utilisateur peut spécifier le nom de l'environnement qu'ils souhaitent supprimer comme indiqué ci-dessus.

Après avoir saisi la commande ci-dessus, il vous sera demandé

Étape 1: Supprimer Environnements ici?

et affiche un message d'avertissement en tant que

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 


L'utilisateur doit spécifier Y ou N


Étape 2: Environnement Kevells (Nom de l'environnement spécifié qui est censé supprimer) trouvé. Êtes-vous sûr de vouloir supprimer? (Y / N)

L'utilisateur doit spécifier Y ou N

Enfin, l'environnement spécifié est supprimé comme le montre la capture d'écran.

.. code-block:: bash

 kevell@corp:/# ptconfigure envconfig del --environment-name="kevells"
 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 Y
 Environment kevells found. Are you sure you want to delete it? (Y/N) 
 Y
 [Pharaoh Logging] Removing environment kevells.
 ******************************


 Success
 In Environment Configuration
 ******************************



Une autre façon de suppression d'un environnement en sans préciser le nom de l'environnement est tel que représenté en utilisant la commande:

.. code-block:: bash

	ptdeployenvconfig delete

Après avoir saisi la commande ci-dessus, il vous sera demandé

Étape 1: Supprimer Environnements ici?

et affiche un message d'avertissement en tant que

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 


L'utilisateur doit spécifier Y ou N

Enfin, l'environnement est supprimé comme le montre la capture d'écran:

.. code-block:: bash


 kevell@corp:/# ptdeployenvconfig delete
 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 Y
 PHP Notice:  Undefined index: environment-name in /opt/ptdeploy/ptdeploy/src/Modules/EnvironmentConfig/Model/EnvironmentConfigAllLinux .php on line 161
 PHP Notice:  Undefined index: environment-name in /opt/ptdeploy/ptdeploy/src/Modules/EnvironmentConfig/Model/EnvironmentConfigAllLinux .php on line 161
 ******************************


 Success
 In Environment Configuration
 ******************************



Comment lister la configuration de l'environnement
--------------------------------------------------

Si l'utilisateur souhaite pouvoir voir la liste des détails sur la configuration de l'environnement, ils peuvent entrée comme indiqué:

.. code-block:: bash

	ptdeployenvconfig list

Après avoir saisi la commande ci-dessus, il sera demande

Inscrivez Environnement ici? (Y / N)

si l'utilisateur spécifie que Y, il va générer l'affichage de sortie, comme illustré dans la capture d'écran:

.. code-block:: bash

 kevell@corp:/# ptdeploy envconfig list
 List Environments Here? (Y/N) 
 Y
 ******************************


 array(2) {
  [0]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(13) "default-local"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(9) "127.0.0.1"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
  [1]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(18) "default-local-8080"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(14) "127.0.0.1:8080"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
 }

 In Environment Configuration
 ******************************


Autres paramètres
--------------------------------
 
Au lieu de envconfig les paramètres suivants peuvent être utilisés dans la déclaration:

* EnvironmentConfig
* environmentconfig
* environment-config
* env-config

avantages
------------

* Il est bien de choses à faire dans les deux cent OS et ainsi que dans ubuntu.
* Les paramètres utilisés dans la déclaration ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux autres.
* Ce module conduit les utilisateurs à configurer l'environnement, comment supprimer l'environnement indésirables, la façon d'utiliser l'option   de liste énumérant les environnements disponibles.

