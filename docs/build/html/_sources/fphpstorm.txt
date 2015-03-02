=================
PHPStorm
=================

synopsis
----------------

PhpStorm tient avec les dernières tendances de PHP & ptconfigure, intègre une variété d'outils modernes, et apporte encore plus l'extensibilité avec le soutien des principaux frameworks PHP. Environnement de développement auto-configuration (norme de codage, les associations de fichiers, etc.) est possible. Il est à l'aise avec Ubuntu et cent OS.

Commande Aide
------------------------

Cette commande peut fonctionner sur les objectifs et les commandes disponibles dans le module de tempête ptconfigure Php. Il explique également la commande pour installer le module de tempête Php. Avant l'installation, l'utilisateur peut lire cette commande d'aide explique sa fonction.

.. code-block:: bash
   
	       ptconfigure PHPStorm help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide sous PHP Storm.

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPStorm help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  PHPStorm, phpstorm

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************


installation
------------------

Si l'utilisateur souhaite installer les outils de git à leur machine, ils peuvent utiliser la commande comme indiqué ci-dessous,

.. code-block:: bash

	ptconfigure gittools install

Après avoir saisi la commande ci-dessus, les étapes suivantes sont impliqués au cours du processus d'installation, comme décrit dans le tableau,

.. cssclass:: table-bordered

 +-------------------------+--------------------------------------+------------+--------------------------------------------------+
 | Paramètre               | Autres paramètres                    | Options    | Commentaires                                     |
 +=========================+======================================+============+==================================================+
 |Install Git Tools? (Y/N) | Au lieu d'utiliser PHPStorm Nous     | Y(Yes)     | Si l'utilisateur souhaite procéder le processus  | 
 |                         | pouvons utiliser phpstorm            |            | d'installation qu'ils peuvent entrée comme Y.    |
 +-------------------------+--------------------------------------+------------+--------------------------------------------------+
 |Install Git Tools? (Y/N) | Au lieu d'utiliser PHPStorm Nous     | N(No)      | Si l'utilisateur souhaite quitter le processus   |
 |                         | pouvons utiliser phpstorm            |            | d'installation qu'ils peuvent entrée comme N|    |
 +-------------------------+--------------------------------------+------------+--------------------------------------------------+


La capture d'écran ci-dessous représente graphiquement le processus décrit ci-dessus de l'installation.

.. code-block:: bash

 
 kevell@corp:/# ptconfigure gittools install
 Install Git Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-core from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package gitk from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-cola from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitTools: Success
 ------------------------------
 Installer Finished
 ******************************


avantages
-------------------

* Plus de paramètres pour garder votre code aussi propre que possible
* Meilleure interface avec l'environnement de développement d'auto-configuration.
* Meilleure conseils de code et débogage
* Codage Zen est disponible avec DevOps.
* Curseurs multiples et de simples raccourcis clavier pour créer, éditer, et la navigation entre les questions.
* Plus d'attributs personnalisés, des workflows personnalisables et de personnalisation puissante.
* Utilisé pour installer la dernière version d'outils de développement.
