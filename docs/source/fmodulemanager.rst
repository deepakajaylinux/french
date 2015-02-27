==============
ModuleManager
==============



synopsis
-----------

Le principal objectif du gestionnaire de module est de permettre à l'utilisateur de gérer leurs modules. Ses principales fonctions comprennent l'installation, activer, désactiver, assurer, désinstallation. voyons sur ces grandes fonctions de gestionnaire de module d'une manière élaborée à partir des sujets à venir.

Commande Aide
----------------------

La commande d'aide de ce gestionnaire de module est un manuel d'utilisation brève qui guide l'utilisateur concernant le but, du gestionnaire de module, décrit l'utilisateur sur les grandes fonctions telles que l'installation, activer, désactiver, assurer, désinstaller avec la syntaxe de les déclarer. Il énumère également les aboutissants alternatives paramètres de gestionnaire de module. La commande pour déclarer l'option d'aide en vertu de gestionnaire de module est présenté ci-dessous:

.. code-block:: bash

		ptconfigure ModuleManager help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de gestionnaire de module.

.. code-block:: bash


 kevell@corp:/# ptconfigure ModuleManager help

 ******************************


  The Module Manager allows you to manage modules. Install, Ensure, Uninstall, Enable, Disable.

  ModuleManager, module-manager, modulemanager

        - install
        Installs the latest version of a module. If a module of the same name already exists in your Extensions directory,
        an error will be thrown.
        example: ptconfigure module-manager install --module-name="MyModule" --module-source="http://git.cleo-modules.com/MyModule.git"

        - ensure
        Ensures the existence of a module. The module will only be installed if it currently doesn't exist.
        example: ptconfigure module-manager ensure --module-name="MyModule" --module-source="http://git.cleo-modules.com/MyModule.git"

        - uninstall
        Uninstalls a Module. This will delete all of the files for this Module
        example: ptconfigure module-manager enable --module-name="MyModule"

        - enable
        Enables a Module. All installed Modules are enabled by default.
        example: ptconfigure module-manager enable --module-name="MyModule"

        - disable
        Disables a Module. The files for this module will still exist, but none will be automatically loaded during execution.
        example: ptconfigure module-manager disable --module-name="MyModule"

 ------------------------------
 End Help
 ******************************



installation
----------------

La commande utilisée pour l'installation du gestionnaire de module dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash

		ptconfigure module-manager install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +---------------------+--------------------------------------+-------------+-----------------------------------------+
 | paramètres          | Autres Paramètres                    | options     | Commentaires                            |
 +=====================+======================================+=============+=========================================+
 |Install              | au lieu de module-manager,           | Y(Yes)      | Si l'utilisateur souhaite procéder le   |
 |ModuleManager? (Y/N) | nous pouvons utiliser modulemanager, |             | processus d'installation qu'ils peuvent |
 |                     | ModuleManager aussi.                 |             | entrée comme Y.                         |
 +---------------------+--------------------------------------+-------------+-----------------------------------------+
 |Install              | au lieu de module-manager,           | N(No)       | Si l'utilisateur souhaite quitter le    |
 |ModuleManager? (Y/N) | nous pouvons utiliser modulemanager, |             | processus d'installation qu'ils peuvent |
 |                     | ModuleManager aussi.                 |             | entrée comme N.|                        |
 +---------------------+--------------------------------------+-------------+-----------------------------------------+

Si l'utilisateur procède à l'installation, au cours du processus d'installation, le processus suivant est réalisé comme indiqué dans le format tabulaire:

.. cssclass:: table-bordered

 +-----------------------+-----------------------+-------------+---------------------------------------------------------+
 | paramètres            | Autres Paramètres     | options     | Commentaires                                            |
 +=======================+=======================+=============+=========================================================+
 |Program executor       | “/usr/bin”            | Yes         | Si l'utilisateur de procéder installation avec le       |  
 |directory (Par défaut) |                       |             | répertoire programme d'exécuteur défaut qu'ils peuvent  |
 |                       |                       |             | entrée comme Oui                                        |
 +-----------------------+-----------------------+-------------+---------------------------------------------------------+
 |Program executor       | utilisateur           | No(Slash de | Si l'utilisateur de procéder installation avec leur     |
 |directory (Par défaut) | spécifique            | fin)        | propre répertoire programme de l'exécuteur qu'ils       |
 |                       |                       |             | peuvent entrée comme N, et dans la main indiquer qu'ils |
 |                       |                       |             | possèdent de lieu|                                      |
 +-----------------------+-----------------------+-------------+---------------------------------------------------------+


Enfin volonté d'installation se rempli comme décrit dans la capture d'écran ci-dessous.

permettre
-----------

Le processus vise à permettre l'activation du module. Tous les modules installés sont activés par défaut en utilisant la commande ci-dessous:

.. code-block:: bash

	ptconfigure module-manager enable --module-name="MyModule"

Après avoir saisi cette commande, le module qui est spécifié se activer.


désactiver
-----------

Le processus vise à désactiver la désactivation du module. Les fichiers des modules handicapés reste existe, mais ils ne seront pas chargés au moment de l'exécution. Ceci peut être réalisé par la commande suivante

.. code-block:: bash

	ptconfigure module-manager disable --module-name="MyModule"


Après avoir saisi cette commande, le module qui est spécifié se désactivée.

assurer
----------

Le rôle de veiller à ce processus est de vérifier la disponibilité de modules. Après le processus de veiller à se rempli les modules seront installés que si les modules se rapportent ne pas installé. Le processus d'assurer qu'il peut être fait en utilisant la commande ci-dessous:

.. code-block:: bash

		ptconfigure module-manager ensure

Au cours du processus d'assurer, les versions des modules ne sont pas vérifiées. Représentent imagée La capture d'écran ci-dessous le processus de veiller.

.. code-block:: bash

 kevell@corp:/# ptconfigure module-manager ensure

 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ModuleManager reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ******************************


 Single App Installer:
 --------------------------------------------
 ModuleManager: Success
 ------------------------------
 Installer Finished
 ******************************


Désinstaller
-------------

Le processus de désinstallation permet de supprimer tous les fichiers pour les modules. La commande utilisée pour désinstaller le gestionnaire de module est présenté ci-dessous:

.. code-block:: bash

		ptconfigure module-manager uninstall

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered


 +-----------------------+-----------------------------------------------+-------------+-------------------------------------------+
 | paramètres            | Autres Paramètres                             | options     | Commentaires                              |
 +=======================+===============================================+=============+===========================================+
 |Un Install             | au lieu de module-manager nous pouvons        | Y(Yes)      | Si l'utilisateur souhaite procéder le     |
 |ModuleManager? (Y/N)   | utiliser modulemanager, ModuleManager aussi.  |             | processus d'installation de l'ONU qu'ils  |
 |                       |                                               |             | peuvent entrée comme Y.                   |
 +-----------------------+-----------------------------------------------+-------------+-------------------------------------------+
 |Un Install             | au lieu de module-manager nous pouvons        | N(No)       | Si l'utilisateur souhaite quitter le      |
 |ModuleManager? (Y/N)   | utiliser modulemanager, ModuleManager aussi.  |             | processus d'installation de l'ONU qu'ils  |
 |                       |                                               |             | peuvent entrée comme N.|                  |
 +-----------------------+-----------------------------------------------+-------------+-------------------------------------------+


Si l'utilisateur procède à l'installation de l'ONU, au cours du processus d'installation de l'ONU, le processus suivant est réalisé comme indiqué dans le format tabulaire:

.. cssclass:: table-bordered

 +------------------------+------------------------+-------------------+------------------------------------------------------------+
 | paramètres             | Autres Paramètres      | options           | Commentaires                                               |
 +========================+========================+===================+============================================================+
 |Program executor        | “/usr/bin”             | Yes               | Si l'utilisateur de procéder installation avec le          |
 |directory (Par défaut)  |                        |                   | répertoire programme d'exécuteur défaut qu'ils peuvent     |
 |                        |                        |                   | entrée comme Oui                                           |
 +------------------------+------------------------+-------------------+------------------------------------------------------------+
 |Program executor        | utilisateur spécifique | No(Slash de fin)  | Si l'utilisateur de procéder installation avec leur propre |
 |directory (Par défaut)  |                        |                   | répertoire programme de l'exécuteur qu'ils peuvent entrée  |
 |                        |                        |                   | comme N, et dans la main indiquer qu'ils possèdent         |
 |                        |                        |                   | emplacement|                                               |
 +------------------------+------------------------+-------------------+------------------------------------------------------------+



Enfin, l'installation de l'ONU se rempli comme décrit dans la capture d'écran ci-dessous.

.. code-block:: bash


avantages
-------------

* Les paramètres utilisés dans l'aide et l'installation, désinstallation, activer, désactiver, assurez-vous ne sont pas sensibles à la casse 
  qui est un avantage supplémentaire tout par rapport à d'autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Le processus facilite assurer la disponibilité de vérification des modules avant l'installation.
* Si l'utilisateur souhaite désactiver un module particulier, ils peuvent les désactiver sans effacer ses fichiers correspondants.
* Au cours de l'installation, désinstallez l'utilisateur peut spécifier l'emplacement pour le répertoire programme de l'exécuteur.
