====================
Environment config
====================


synopsis
-------------

Ce module facilite les utilisateurs à configurer leur environnement nécessaire à leur projet. Voyons comment configurer l'environnement, comment supprimer l'environnement indésirables, la façon d'utiliser l'option de liste énumérant les environnements disponibles dans les prochains sujets.

Commande Aide
--------------------

La commande help guide les utilisateurs au sujet de la fin du module, ses paramètres de remplacement qui sont utilisés dans la déclaration. Il met en évidence les trois fonctions de configuration de l'environnement qui sont liste, configurer, supprimer. Il précise également la syntaxe pour utiliser trois fonctions principales. La syntaxe utilisée pour déclarer l'aide est indiqué ci-dessous:

.. code-block:: bash

		cleopatra envconfig help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash


 kevell@corp:/# cleopatra envconfig help
 ******************************


  This command is part of a default Module and provides you with a method by which you can
  configure environments for your project from the command line. Currently compliant with
  both Dapperstrano and Cleopatra.


  EnvironmentConfig, environmentconfig, environment-config, envconfig, env-config

        - list
        List current environments
        example: cleopatra envconfig list --yes

        - list-local
        List current local environments
        example: cleopatra envconfig list-local --yes

        - configure, config
        Configure bespoke environments for your project to use
        example: cleopatra envconfig config
        # below to create an empty environment to add instances to
        example: cleopatra envconfig config --yes
                    --keep-current-environments # do not overwrite the current environments stored in papyrusfile
                    --no-manual-servers # so it will not ask you to interactively enter connection details of instances
                    --add-single-environment # otherwise it will loop for more until you specify not to
                    --environment-name="some-name" # name of the environment to create
                    --tmp-dir=/tmp/ # we're deprecating this soon

        - configure-default, config-default
        Configure default environments for your project to use
        example: cleopatra envconfig config-default
        example: cleopatra envconfig config-default --yes --environment-name="local-80/local-8080"

        - delete, del
        Configure the environments for your project to use
        example: cleopatra envconfig delete
        example: cleopatra envconfig del --environment-name="staging"


 ------------------------------
 End Help
 ******************************

Comment configurer l'environnement
----------------------------------------------

Aux fins de la configuration des environnements, l'utilisateur peut utiliser la commande suivante:

.. code-block:: bash

		cleopatra envconfig config

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

 kevell@corp:/# cleopatra envconfig config
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

		cleopatra envconfig config --keep-current-environments

Après avoir saisi la commande ci-dessus, il sera demande les détails suivants comme indiqué dans le format tabulaire:


.. cssclass:: table-bordered

 +-------------------------------+------------+-------------------------------------------------------------------------------+
 | Parameters                    | Options    | Comments                                                                      |
 +===============================+============+===============================================================================+
 |Configure Environments         | Y          | Si l'utilisateur souhaite configurer les environnements à l'environnement     |
 |Here? (Y/N)                    |            | actuel ils peuvent d'entrée comme Y                                           |
 +-------------------------------+------------+-------------------------------------------------------------------------------+
 |Configure Environments         | N          | Si l'utilisateur ne souhaite pas configurer les environnements à              |
 |Here? (Y/N)                    |            | l'environnement actuel ils peuvent d'entrée comme N                           |
 +-------------------------------+------------+-------------------------------------------------------------------------------+
 |Use existing environment       | Y          | Si l'utilisateur souhaite utiliser les paramètres d'environnement             |
 |settings? (Y/N)                |            | existantes qu'ils peuvent entrée comme Y.                                     |
 +-------------------------------+------------+-------------------------------------------------------------------------------+
 |Use existing environment       | N          | Si l'utilisateur ne souhaite pas utiliser les paramètres d'environnement      |
 |settings? (Y/N)                |            | existantes qu'ils peuvent entrée comme N.                                     |
 +-------------------------------+------------+-------------------------------------------------------------------------------+
 |Do you want to add another     | Y          | Si l'utilisateur souhaite ajouter un autre environnement, ils peuvent         |
 |environment? (Y/N)             |            | entrée comme Y.                                                               |
 +-------------------------------+------------+-------------------------------------------------------------------------------+
 |Do you want to add another     | N          | Si l'utilisateur ne souhaite pas ajouter un autre environnement, ils          |
 |environment? (Y/N)             |            | peuvent entrée comme N.|                                                      |
 +-------------------------------+------------+-------------------------------------------------------------------------------+


La capture d'écran ci-dessous représente graphiquement le processus mentionné ci-dessus:

.. code-block:: bash


 kevell@corp:/# cleopatra envconfig config --keep-current-environments
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
------------------------------------------------------------------ 

Si l'utilisateur doit supprimer la configuration de l'environnement, ils peuvent saisir la commande suivante:

.. code-block:: bash

		cleopatra envconfig del --environment-name="kevells"

L'utilisateur peut spécifier le nom de l'environnement qu'ils souhaitent supprimer comme indiqué ci-dessus.

Après avoir saisi la commande ci-dessus, il vous sera demandé

Étape 1: Supprimer Environnements ici?

et affiche un message d'avertissement en tant que

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 

LLe utilisateur doit spécifier Y ou N

Étape 2: Environnement Kevells (Nom de l'environnement spécifié qui est censé supprimer) trouvé. Êtes-vous sûr de vouloir supprimer? (Y / N)

L'utilisateur doit spécifier Y ou N

Enfin, l'environnement spécifié est supprimé comme le montre la capture d'écran

.. code-block:: bash



 kevell@corp:/# cleopatra envconfig del --environment-name="kevells"
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

Comment lister la configuration de l'environnement
-------------------------------------------------------------------

Si l'utilisateur souhaite pouvoir voir la liste des détails sur la configuration de l'environnement, ils peuvent entrée comme indiqué:

.. code-block:: bash

		cleopatra envconfig list --yes

Après avoir saisi la commande ci-dessus, il affiche la sortie comme indiqué dans la capture d'écran:

.. code-block:: bash


 kevell@corp:/# cleopatra envconfig list --yes
 ******************************


 array(0) {
 }

 In Environment Configuration
 ******************************


Autres paramètres
--------------------------------

Au lieu de envconfig les paramètres suivants peuvent être utilisés dans la déclaration:

* EnvironmentConfig
* environmentconfig
* Environnement-config
* Env-config

avantages
------------

* Il est bien de choses à faire dans les deux cent OS et ainsi que dans ubuntu.
* Les paramètres utilisés dans la déclaration ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux autres.
* Ce module conduit les utilisateurs à configurer l'environnement, comment supprimer l'environnement indésirables, la façon d'utiliser l'option   de liste énumérant les environnements disponibles.

