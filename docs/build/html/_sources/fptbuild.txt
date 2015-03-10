=================
PTBuild
=================

synopsis
------------------

Cet outil permet à l'utilisateur d'installer et mettre à jour ptbuild sous ptconfigure dans les outils de pharaon. Automatisation de la construction devrait inclure automatisant l'intégration, qui comprend souvent le déploiement dans un environnement de production comparables. Dans de nombreux cas, le script de compilation non seulement compile les binaires, mais génère aussi de la documentation, pages web, les statistiques et les médias de distribution tels que Red Hat. Il réconforte avec Ubuntu et Cent OS.

Commande Aide
-----------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules de ptbuild. Les listes de commandes de l'aide sur les autres paramètres de ptbuild sous module de ptconfigure. Il décrit également la syntaxe pour l'installation de la updation de l'utilisateur. La commande d'aide pour ptbuild est illustré ci-dessous.

.. code-block:: bash

 		ptconfigure ptbuild help

La capture d'écran ci-dessous montre l'effort plein de ptbuild

.. code-block:: bash

 kevell@corp:/# ptconfigure ptbuild help

 ******************************


  This command allows you to install or update ptbuild.

  ptbuild, ptbuild

        - install
        Installs the latest version of ptbuild
        example: ptconfigure ptbuild install

        - ensure
        Ensures ptbuild is installed
        example: ptconfigure ptbuild ensure

        - uninstall
        Uninstalls the latest version of ptbuild
        example: ptconfigure ptbuild uninstall
 ------------------------------
 End Help
 ******************************


installation
--------------------

Ce est un outil qui se trouve sous ptconfigure et tire vers le bas des copies propres de l'utilisateur base de code et ne se appuie pleinement, à partir de zéro, tout le temps. Cette commande est utilisée pour installer la dernière version de ptbuild. La commande utilisée pour l'installation est le suivant.

.. code-block:: bash

	ptconfigure ptbuild install


Après entrées de la commande du système peut poser

installer ptbuild? (Y / N)

Si l'utilisateur donne Y puis ptbuild sera installé. La capture d'écran suivante le démontrent.

.. code-block:: bash


.. cssclass:: table-bordered


 +--------------------------+-------------------------------------------+-----------+-------------------------------------------------------+
 | Paramètres               | Directory_Default                         | Options   | commentaires                                          |
 +==========================+===========================================+===========+=======================================================+
 |Program data directory    | “/opt/ptbuild(módulo correspondiente)”    | Y(Yes)    | Si l'utilisateur souhaite procéder installation avec  | 
 |(par défaut)              |                                           |           | le même répertoire par défaut spécifié qu'ils peuvent |
 |                          |                                           |           | entrée comme Y.                                       |
 +--------------------------+-------------------------------------------+-----------+-------------------------------------------------------+
 |Program data directory    | spécifiques à un utilisateur              | No(Slash  | Si l'utilisateur a besoin de spécifier leur           |
 |                          |                                           | Fin)      | propre emplacement, ils peuvent entrée comme N. et à  |
 |                          |                                           |           | la main préciser leur propre emplacement              |
 +--------------------------+-------------------------------------------+-----------+-------------------------------------------------------+
 |Program executor          | “/usr/bin”                                | Yes       | Si l'utilisateur souhaite procéder installation avec  |
 |directory (par défaut)    |                                           |           | le même répertoire par défaut spécifié qu'ils peuvent |
 |                          |                                           |           | entrée comme Y.                                       |
 +--------------------------+-------------------------------------------+-----------+-------------------------------------------------------+
 |Program executor          | spécifiques à un utilisateur              | No(Slash  | Si l'utilisateur a besoin de spécifier leur propre    |
 |directory                 |                                           | Fin)      | emplacement, ils peuvent entrée comme N. et à la main |
 |                          |                                           |           | préciser leur propre emplacement|                     |
 +--------------------------+-------------------------------------------+-----------+-------------------------------------------------------+


Désinstaller
--------------

Cette commande est utilisée pour désinstaller la dernière version de ptbuild. La commande utilisée pour la désinstallation est la suivante.

.. code-block:: bash

		ptconfigure ptbuild Uninstall

Après entrées de la commande du système peut poser

Désinstaller ptbuild? (Y / N)

Si l'utilisateur donne Y puis ptbuild sera désinstallé. La capture d'écran suivante le démontrent.


.. cssclass:: table-bordered


 +---------------------------+------------------------------------+-------------+--------------------------------------------------------+
 | Parameters                | Directory_Default                  | Options     | commentaires                                           |
 +===========================+====================================+=============+========================================================+
 |Program data directory     | “/opt/ptbuild(módulo               | Y(Yes)      | Si l'utilisateur souhaite procéder désinstallation     |  
 |(par défaut)               | correspondiente)”                  |             | avec le même répertoire par défaut spécifié qu'ils     |
 |                           |                                    |             | peuvent entrée comme Y.                                |
 +---------------------------+------------------------------------+-------------+--------------------------------------------------------+
 |Program data directory     | spécifiques à un utilisateur       | No(Slash    | Si l'utilisateur a besoin de spécifier leur propre     |
 |                           |                                    | Fin)        | emplacement, ils peuvent entrée comme N. et à la       |
 |                           |                                    |             | main préciser leur propre emplacement                  |
 +---------------------------+------------------------------------+-------------+--------------------------------------------------------+
 |Program executor           | “/usr/bin”                         | Yes         | Si l'utilisateur souhaite procéder désinstallation     |
 |directory (par défaut)     |                                    |             | avec le même répertoire par défaut spécifié qu'ils     |
 |                           |                                    |             | peuvent entrée comme Y.                                |
 +---------------------------+------------------------------------+-------------+--------------------------------------------------------+
 |Program executor directory | spécifiques à un utilisateur       | No(Slash    | Si l'utilisateur a besoin de spécifier leur propre     |
 |                           |                                    | Fin)        | emplacement, ils peuvent entrée comme N. et à la       |
 |                           |                                    |             | main préciser leur propre emplacement|                 |
 +---------------------------+------------------------------------+-------------+--------------------------------------------------------+


assurer
----------

Processus utilisé pour vérifier l'ptbuild installé dans le système ou non de l'utilisateur Vérifiez. La commande suivante permet à l'utilisateur de se assurer.

.. code-block:: bash

		ptconfigure ptbuild ensure

La capture d'écran ci-dessous montre ses fonctions.

paramètre alternatifs
-----------------------

Ce sont les paramètres de substitution,

ptbuild, ptbuild


avantages
----------------

* Utilisé pour installer ptbuilds possible.
* Convient pour travailler avec Ubuntu et CentOS.
* Sensibilité non de cas.
* Automatisation dans la version mise à jour.
* Fiabilité, disponibilité, maintenabilité avec d'autres connexions.
