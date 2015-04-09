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
 |directory           | correspondant)           |                 | de données par défaut du programme qu'ils peuvent entrée         |
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


 kevell@corp:/#ptconfigure PHPCI install
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 [Pharaoh Logging] Packages php5-mcrypt, curl from the Packager Apt are already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-45785693692.sh
 chmod 755 /tmp/ptconfigure-temp-script-45785693692.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-45785693692.sh Permissions
 Executing /tmp/ptconfigure-temp-script-45785693692.sh
 Temp File /tmp/ptconfigure-temp-script-45785693692.sh Removed
 Creating /tmp/ptconfigure-temp-script-47686609771.sh
 chmod 755 /tmp/ptconfigure-temp-script-47686609771.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47686609771.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47686609771.sh
 Module rewrite already enabled
 Temp File /tmp/ptconfigure-temp-script-47686609771.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Composer reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-71236381661.sh
 chmod 755 /tmp/ptconfigure-temp-script-71236381661.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-71236381661.sh Permissions
 Executing /tmp/ptconfigure-temp-script-71236381661.sh
 Installing block8/phpci (1.6.0)
   - Installing block8/phpci (1.6.0)
    Loading from cache

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
  - Installing symfony/yaml (v2.6.4)
    Loading from cache

  - Installing block8/b8framework (1.1.9)
    Loading from cache

  - Installing ircmaxell/password-compat (v1.0.4)
    Loading from cache

  - Installing psr/log (1.0.0)
    Loading from cache

  - Installing monolog/monolog (1.12.0)
    Loading from cache

  - Installing pimple/pimple (v1.1.1)
    Loading from cache

  - Installing symfony/console (v2.6.4)
    Loading from cache

  - Installing symfony/filesystem (v2.6.4)
    Loading from cache

  - Installing symfony/config (v2.6.4)
    Loading from cache

  - Installing robmorgan/phinx (v0.4.2.1)
    Loading from cache

  - Installing swiftmailer/swiftmailer (v5.3.1)
    Loading from cache

 Generating autoload files
 Temp File /tmp/ptconfigure-temp-script-42085224634.sh Removed
 Creating /tmp/ptconfigure-temp-script-47565859655.sh
 chmod 755 /tmp/ptconfigure-temp-script-47565859655.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47565859655.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47565859655.sh
 [Pharaoh Logging] Lets begin Configuration of a Web Server for PHPCI
 [Pharaoh Logging] Lets Add our Apache VHost
 [Pharaoh Logging] Now lets restart Apache so we are serving our new application 

 Logging Starting
 Logging Complete
 Logging Starting
 Logging Complete
 <VirtualHost 127.0.0.1:80>
	ServerAdmin webmaster@localhost
	ServerName www.phpci.local
	DocumentRoot /opt/phpci/phpci/public/
	<Directory /opt/phpci/phpci/public/>
		Options Indexes FollowSymLinks MultiViews
		AllowOverride All
		Require all granted

        <IfModule mod_rewrite.c>
          RewriteEngine On
          RewriteBase /opt/phpci/phpci/public/
          RewriteCond %{REQUEST_FILENAME} !-f
          RewriteCond %{REQUEST_FILENAME} !-d
          RewriteRule . /index.php [L]
        </IfModule>

	</Directory>

 </VirtualHost>

 Assuming Okay due to yes parameter
 Site www.phpci.local already enabled
 a2ensite www.phpci.local done
 Logging Starting
 Logging Complete
 Temp File /tmp/ptconfigure-temp-script-47565859655.sh Removed
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

.. code-block:: bash

 kevell@corp:/#ptconfigure PHPCI config-default

 Install PHP CI Default Configuration? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPCI Defaults        *
 *******************************
 Set non-default value for db_read_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_write_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_name? Default is phpci (Y/N) 
 n
 Set non-default value for db_username? Default is phpci (Y/N) 
 n
 Set non-default value for db_pass? Default is phpci_pass (Y/N) 
 n
 Set non-default value for phpci_url? Default is http://www.phpci.local (Y/N) 
 n
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
 ------------------------------
 Installer Finished
 ****************************** 

.. code-block:: bash


 kevell@corp:/#ptconfigure phpci install-default-database
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 Database script executed
 ******************************  

 Seems Fine...Database Actions Finished
 ******************************

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
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
