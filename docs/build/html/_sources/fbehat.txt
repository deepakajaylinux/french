=======
Behat 
=======

synopsis
--------------

Ce module vise à installer Behat avec la version la plus récente-. Cela aide à tester un script php. Il facilite les utilisateurs à identifier les erreurs de script php. Il met en lumière les modèles activés et désactivés. Le git agit comme un logiciel de support pour Behat.

Commande Aide
----------------------


Les guides de la commande d'aide l'utilisateur obtiennent au courant des usages, ainsi que les options et les actions qui peuvent être effectuées. Il énumère les aboutissants des paramètres alternatifs qui peuvent être utilisés dans la déclaration. Il spécifie la commande pour l'installation de la dernière version de Behat.

Le codage de faire usage de commande d'aide en vertu Behat, est donnée comme suit:

.. code-block:: bash

		cleopatra behat help

La capture d'écran ci-dessous vous que donnée explique graphiquement sur l'utilisation de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# cleopatra behat help
 ******************************


  This command allows you to install Behat.

  Behat, behat

        - install
        Installs the latest version of behat
        example: cleopatra behat install

 ------------------------------
 End Help
 ******************************

installation
--------------

Si l'utilisateur a besoin d'installer la dernière version de Behat, ils peuvent réaliser l'installation, en utilisant la commande suivante,
.. code-block:: bash

	cleopatra behat install

Après avoir saisi la commande ci-dessus, le processus suivant sont impliqués dans l'installation comme indiqué dans le format tabulaire,

.. cssclass:: table-bordered


 +-------------------------+------------------------------------+------------+-----------------------------------------------+
 | paramètres              | Autres paramètres                  | Requis     | commentaire	                             |
 +=========================+====================================+============+===============================================+
 |Install behat? (Y/N)     | au lieu de behat, nous pouvons     | Yes        | Si l'utilisateur donne entrée que oui,        | 
 |                         | utiliser Behat                     |            | il procédera installation.                    |
 +-------------------------+------------------------------------+------------+-----------------------------------------------+
 |Install behat? (Y/N)     | au lieu de behat, nous pouvons     | No         | Si l'utilisateur donne entrée que non, ce     |
 |                         | utiliser Behat                     |            | ne sera quitter le processus d'installation.| |
 +-------------------------+------------------------------------+------------+-----------------------------------------------+
  

Si l'utilisateur procède à l'installation en inscrivant, Y , les étapes suivantes sont impliqués dans l'installation Behat ,

.. cssclass:: table-bordered

 +---------------------------+-------------------------------+-------------+----------------------------------------------------+
 | paramètres                | Autres paramètres             | Requis      | commentaire                                        |
 +===========================+===============================+=============+====================================================+
 |Program data directory     | “/opt/behat (corresponding    | Yes	   | Si l'utilisateur de procéder installation avec le  |
 |(default)                  | module)”                      |             | répertoire de données par défaut du programme      |
 |                           |                               |             | qu'ils peuvent entrée comme Oui                    |
 +---------------------------+-------------------------------+-------------+----------------------------------------------------+
 |Program data directory     | User specific                 | No (End     | Si l'utilisateur souhaite procéder à leur propre   |
 |                           |                               | slash)      | répertoire de données de programme, ils peuvent    |
 |                           |                               |             | entrée comme N, et dans la main indiquer qu'ils    |
 |                           |                               |             | possèdent emplacement                              |
 +---------------------------+-------------------------------+-------------+----------------------------------------------------+
 |Program executor directory | “/usr/bin”                    | Yes	   | Si l'utilisateur de procéder installation avec le  |
 |(Default)                  |                               |             | répertoire programme d'exécuteur défaut, ils       |
 |                           |                               |             | pouvez entrer que oui                              | 
 +---------------------------+-------------------------------+-------------+----------------------------------------------------+
 |Program executor directory | User specific                 | No (End     | Si l'utilisateur souhaite procéder installation    |
 |                           |                               | slash)      | avec thir propre répertoire programme d'exécuteur  |
 |                           |                               |             | testamentaire, ils peuvent entrée comme N, et dans |
 |                           |                               |             | la main indiquer qu'ils possèdent emplacement|     |
 +---------------------------+-------------------------------+-------------+----------------------------------------------------+


Vous donne une représentation picturale sur les étapes de l'installation La capture d'écran ci-dessous volonté.

.. code-block:: bash

 kevell@corp:/# cleopatra behat install
 Install Behat ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          Behat         *
 *******************************
 What is the program data directory? Found "/opt/behat" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 Creating /tmp/cleopatra-temp-script-69243074239.sh
 chmod 755 /tmp/cleopatra-temp-script-69243074239.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-69243074239.sh Permissions
 Executing /tmp/cleopatra-temp-script-69243074239.sh
 --2015-01-27 15:31:39--  https://getcomposer.org/installer
 Resolving getcomposer.org (getcomposer.org)... 87.98.253.108
 Connecting to getcomposer.org (getcomposer.org)|87.98.253.108|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: unspecified [text/plain]
 Saving to: ‘installer’

    [              <=>                                                                                     ] 2,74,634    48.9KB/s   in 5.5s   

 2015-01-27 15:31:47 (48.9 KB/s) - ‘installer’ saved [274634]

 All settings correct for using Composer
 Downloading...

 Composer successfully installed to: /opt/behat/behat/composer.phar


Lors de l'installation du Behat, l'utilisateur peut spécifier le répertoire des données du programme et le répertoire programme de l'exécuteur.


Ci-dessus explique la syntaxe concernant la spécification du répertoire des données du programme et le répertoire de l'exécuteur La capture d'écran.


version
----------

Lors de l'installation du Behat, la version la plus récente sera-installé sur votre machine.

Ce est un avantage supplémentaire d'un module Behat sous Cleopatra par rapport à d'autres.


Avantages pour les utilisateurs
-------------------------------------------

* Il guide les utilisateurs à identifier les erreurs de script php.
* Pas besoin de chercher la version la plus récente-, que la version mise à jour est automatiquement disponible pour les utilisateurs pendant 
  l'exécution de l'installation pr ocessus.
* Utilisation des fonctions de Behat les utilisateurs peuvent définir et spécifier le comportement de développement piloté.

