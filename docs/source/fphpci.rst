===============
Phpci
===============

synopsis
--------------

PHPCI est un outil d'intégration continue open source spécifiquement conçu pour ptconfigure. L'utilisateur ont construit avec simplicité à l'esprit, de sorte alors qu'il ne fait pas tout Jenkins peut faire, ce est un jeu d'enfant à installer et à utiliser. Ce est la facilité avec Ubuntu et cent OS.

Commande Aide
-----------------------

 Cette commande d'aide à guider l'utilisateur d'effectuer certaines opérations sur sur le module Phpci. Ceci est approprié pour tous les types d'utilisateurs de l'entreprise.

.. code-block:: bash
   
	ptconfigure PHPCI help

La commande d'aide montre une courte liste des commandes intégrées dans le module Phpci. La capture d'écran suivante le visualiser.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCI help
 ******************************


  This command allows you to install PHPCI, the popular Build Server.

  PHPCI, phpci

        - install
        Installs PHPCI through git, with its dependencies
        example: ptconfigure phpci install

        - config-default, default-config
        Installs a default config.yml file for PHPCI
        example: ptconfigure phpci config-default --yes --guess

        - install-default-database
        Installs a default database and user for PHPCI
        example: ptconfigure phpci install-default-database --yes --guess
            --mysql-admin-user="root" # guess will provide root
            --mysql-admin-pass="some-pass" # guess will provide ptconfigure

  You can install a complete local version of PHPCI with the following:

  sudo ptconfigure phpci install --yes --guess
  sudo ptconfigure phpci install-default-database --yes --guess
  sudo ptconfigure phpci config-default --yes --guess

 ------------------------------
 End Help
 ******************************



installation
-----------------

	Ce module permet d'installer phpci. Première étape de ce module ont pour vérifier compositeur est disponible dans le système ou non. Se il ne est pas disponible dans le système automatiquement, il sera l'installer.

.. code-block:: bash

                   ptconfigure Phpci install



Après avoir saisi la commande ci-dessus, le processus suivant sont impliqués au cours du processus d'installation comme décrit dans le format tabulaire,

.. cssclass:: table-bordered

 +-----------------------+--------------------------------------+--------------+--------------------------------------------------+
 | paramètres            | paramètres alternatifs               | options      | Commentaires                                     |
 +=======================+======================================+==============+==================================================+
 |Install PHPCI? (Y/N)   | Au lieu de PHPCI, nous pouvons       | Y(Yes)       | Si l'utilisateur souhaite procéder le processus  |
 |                       | utiliser phpci également.            |              | d'installation qu'ils peuvent entrée comme Y     |
 +-----------------------+--------------------------------------+--------------+--------------------------------------------------+
 |Install PHPCI? (Y/N)   | Au lieu de PHPCI, nous pouvons       | N(No)        | Si l'utilisateur souhaite quitter le processus   |
 |                       | utiliser phpci également.            |              | d'installation qu'ils peuvent entrée comme N.|   |
 +-----------------------+--------------------------------------+--------------+--------------------------------------------------+
 

Si l'installation utilisateur de produit, au cours du processus d'installation, les étapes suivantes sont impliqués,

* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les forfaits supplémentaires qui sont automatiquement installés.
* Liste outs les forfaits proposés, qui sont installez.
* Liste outs les nouveaux paquets qui installent.
* Détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.



Et puis, il sera demande entrée par les utilisateurs, comme représenté sous forme de tableau

.. cssclass:: table-bordered

 +--------------------+--------------------------+-----------------+------------------------------------------------------------------+
 | Paramètre          | Chemin                   | Option          | Commentaire                                                      |
 +====================+==========================+=================+==================================================================+
 |Program data        | “/opt/phpunit”(module    | Yes             | Si l'utilisateur de procéder installation avec le répertoire     |
 | directory          | correspondant)           |                 | de données par défaut du programme qu'ils peuvent entrée         |
 |(Par défaut)        |                          |                 | comme Oui                                                        |
 +--------------------+--------------------------+-----------------+------------------------------------------------------------------+
 |Program data        | spécifiques à un         | No(Slash Fin)   | Si l'utilisateur souhaite procéder à leur propre répertoire      |
 |directory           | utilisateur              |                 | de données de programme, ils peuvent entrée comme N, et dans la  |
 |                    |                          |                 | main indiquer qu'ils possèdent emplacement.                      |
 +--------------------+--------------------------+-----------------+------------------------------------------------------------------+
 |Program executor    | “/usr/bin”               | Yes             | Si l'utilisateur de procéder installation avec le répertoire     |
 |directory           |                          |                 | programme d'exécuteur défaut qu'ils peuvent entrée comme Oui     |
 |(Par défaut)        |                          |                 |                                                                  |
 +--------------------+--------------------------+-----------------+------------------------------------------------------------------+
 |Program executor    | spécifiques à un         | No(Slash Fin)   | Si l'utilisateur souhaite procéder à leur propre répertoire      |
 |directory           | utilisateur              |                 | programme d'exécuteur testamentaire, ils peuvent entrée comme N, |
 |                    |                          |                 | et dans la main indiquer qu'ils possèdent emplacement.|          |
 +--------------------+--------------------------+-----------------+------------------------------------------------------------------+


La capture d'écran ci-dessous représente graphiquement le processus décrit ci-dessus de l'installation.

.. code-block:: bash

 kevell@corp:/#  ptconfigure phpci install
 Install PHPCI? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libmcrypt4
 Suggested packages:
  libmcrypt-dev mcrypt
 The following NEW packages will be installed:
  libmcrypt4 php5-mcrypt
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 77.3 kB of archives.
 After this operation, 324 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmcrypt4 amd64 2.5.8-3.1ubuntu1 [61.9 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe php5-mcrypt amd64 5.4.6-0ubuntu5 [15.4 kB]
 Fetched 77.3 kB in 4s (19.1 kB/s)
 Selecting previously unselected package libmcrypt4.
 (Reading database ... 182037 files and directories currently installed.)
 Preparing to unpack .../libmcrypt4_2.5.8-3.1ubuntu1_amd64.deb ...
 Unpacking libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Selecting previously unselected package php5-mcrypt.
 Preparing to unpack .../php5-mcrypt_5.4.6-0ubuntu5_amd64.deb ...
 Unpacking php5-mcrypt (5.4.6-0ubuntu5) ...
 Setting up libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Setting up php5-mcrypt (5.4.6-0ubuntu5) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package php5-mcrypt from the Packager Apt executed correctly
 Creating /tmp/ptconfigure-temp-script-82480901916.sh
 chmod 755 /tmp/ptconfigure-temp-script-82480901916.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-82480901916.sh Permissions
 Executing /tmp/ptconfigure-temp-script-82480901916.sh
 Temp File /tmp/ptconfigure-temp-script-82480901916.sh Removed
 Creating /tmp/ptconfigure-temp-script-43828918328.sh
 chmod 755 /tmp/ptconfigure-temp-script-43828918328.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-43828918328.sh Permissions
 Executing /tmp/ptconfigure-temp-script-43828918328.sh
 Enabling module rewrite.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-43828918328.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: composer: not found
 [Pharaoh Logging] Module Composer reports itself as Not Installed
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *          Composer!         *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...


 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 Creating /tmp/ptconfigure-temp-script-34508236330.sh
 chmod 755 /tmp/ptconfigure-temp-script-34508236330.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-34508236330.sh Permissions
 Executing /tmp/ptconfigure-temp-script-34508236330.sh
 #!/usr/bin/env php
 Installing block8/phpci (1.5.2)
  - Installing block8/phpci (1.5.2)
    Downloading: 100%

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
 Warning: The lock file is not up to date with the latest changes in composer.json. You may be getting outdated dependencies. Run update to update them.
 Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - The requested PHP extension ext-pdo_mysql * is missing from your system.

 Temp File /tmp/ptconfigure-temp-script-34508236330.sh Removed
 Creating /tmp/ptconfigure-temp-script-28990655696.sh
 chmod 755 /tmp/ptconfigure-temp-script-28990655696.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-28990655696.sh Permissions
 Executing /tmp/ptconfigure-temp-script-28990655696.sh
 sudo: dapperstrano: command not found
 Temp File /tmp/ptconfigure-temp-script-28990655696.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCI: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
----------

* PHPCI utilisé pour installer le fichier de configuration et de base de données. Lors de l'installation se il ya ne importe quel fichier est 
  existant, écraser le contenu.
* Nouvelle version peut mettre à jour automatiquement.
* Il peut accepter l'utilisateur en cas de souhait d'installer la base de données.
* L'intégration continue est possible.
* Environnement multiple
* Compiler PHP avec différentes variantes comme AOP, mysql, sqlite, débogage ... etc.
* Détection automatique de fonction.
