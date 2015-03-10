==========
Composer
==========

synopsis
-----------

Composer est un gestionnaire de dépendance niveau de l'application pour le langage de programmation PHP qui fournit un format standard pour la gestion des dépendances de logiciels PHP et les bibliothèques requises.

Il vous permet de déclarer les bibliothèques dépendantes votre projet a besoin et il va les installer dans votre projet pour vous. Composer est multi-plate-forme et nous nous efforçons de le faire fonctionner aussi bien sur Windows, Linux et OSX.

Commande Aide
---------------------

Cette commande permet de déterminer l'utilisation de module de compositeur. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final concernant les paramètres alternatifs et commande pour l'installation. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
              
		 ptconfigure composer help

.. code-block:: bash

 kevell@corp:/# ptconfigure composer help
 ******************************


  This command allows you to update Composer.

  Composer, composer

        - install
        Installs the latest version of composer
        example: ptconfigure composer install

 ------------------------------
 End Help
 ******************************



installation
----------------

Lorsque l'utilisateur doit installer le module de compositeur dans la machine, la commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
               
	 ptconfigure composer install

Lors de l'installation, le système demande le nom du répertoire, si vous veut mettre en place votre PATH, vous pouvez définir votre chemin. Définissez votre chemin doit être suivie par le symbole «/». Appuyez sur Entrée pour utiliser le chemin par défaut.

"Quel est le répertoire des données du programme?" / Opt / compositeur "- utiliser cette fonction?

Lors de l'installation, le système demande pour exécuter nom de répertoire, si vous veut mettre en place votre PATH, vous pouvez définir votre chemin. Définissez votre chemin doit être suivie par le symbole «/». Appuyez sur Entrée pour utiliser le chemin par défaut.

"Quel est le répertoire programme de exécuteur Trouvé?" / Usr / bin "- Utilisez ce?"

.. cssclass:: table-bordered



 +-------------------------+-------------------------------------------+---------------+--------------------------------------------+
 | paramètres	           | Autres paramètres                         | requis        | commentaire	                            |
 +=========================+===========================================+===============+============================================+
 |Install composer? (Y/N)  | à la place du composor, nous pouvons      | Yes           | système démarre processus d'installation   |
 |                         | utiliser également Composor               |               |                                            |
 +-------------------------+-------------------------------------------+---------------+--------------------------------------------+
 |Install composer? (Y/N)  | à la place du composor, nous pouvons      | No            | système se arrête processus d'installation |
 |                         | utiliser également Composor|              |               |                                            |
 +-------------------------+-------------------------------------------+---------------+--------------------------------------------+




Est listé ci-dessous la capture d'écran pour la commande d'installation,

.. code-block:: bash

 kevell@corp:/$ ptconfigure composer install
 Install Composer - Update to latest version ? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *          Composer!          *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...
 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 PHP Warning:  mkdir(): Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 192
 cp: cannot create directory ‘/opt/composer’: Permission denied
 Program Data folder populated
 Program Executor Deleted if existed
 PHP Warning:  scandir(/opt/composer): failed to open dir: No such file or directory in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 172
 PHP Warning:  scandir(): (errno 2): No such file or directory in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 172
 PHP Warning:  Invalid argument supplied for foreach() in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 174
 PHP Warning:  scandir(/opt/composer): failed to open dir: No such file or directory in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 172
 PHP Warning:  scandir(): (errno 2): No such file or directory in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 172
 PHP Warning:  Invalid argument supplied for foreach() in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 174
 PHP Warning:  file_put_contents(/usr/bin/composer): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BasePHPApp.php on line 214
 chmod: cannot access ‘/opt/composer’: No such file or directory
 chmod: cannot access ‘/usr/bin/composer’: No such file or directory
 ... All done!
 ************************************************
 Thanks for installing , visit www.pharaohtools.com for more
 
 *************************************************
 

 Single App Installer:
 --------------------------------------------
 Composer: Success
 ------------------------------
 Installer Finished
 **************************************************


avantages
----------

* Il installe les dépendances (bibliothèques) pour une application.
* Il permet également aux utilisateurs d'installer des applications PHP qui sont disponibles sur "Packagist" qui est son principal référentiel 
  contenant les packages disponibles.
* Il fournit également des capacités de charge de l'automobile pour les bibliothèques qui spécifient des informations de chargement automatique   pour faciliter l'utilisation de code tiers.











