==========
PHP Unit
==========

synopsis
--------------

Ce module facilite les utilisateurs à installer PHPUnit d'un Repo GC. Cadre tests unitaires PHP est un framework de test unitaire qui permet aux développeurs de découvrir des bogues et à son tour faire baisser les coûts associés au développement de logiciels PHP. Le framework de test unitaire PHP génère des rapports en XML, XHTML ou ASCII. Voyons, comment fait ce module aide à l'installation d'une unité de PHP.

Commande Aide
--------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module de l'unité de PHP. Il décrit également la syntaxe pour l'installation de l'unité de PHP. La commande d'aide de PHP module unité est représentée ci-dessous.

.. code-block:: bash

		ptconfigure PHPUnit help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide sous l'unité PHP.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPUnit help
 ******************************

  This command allows you to install PHPUnit from a GC Repo.

  PHPUnit

        - install
        Installs the latest GC Repo version of PHPUnit
        example: ptconfigure phpunit install

 ------------------------------
 End Help
 ******************************

installation
---------------

La commande utilisée pour l'installation de l'unité de PHP à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash

		ptconfigure PHPUnit install

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +-------------------------+-------------+-----------------------------------------------------------------------------------+
 | Paramètre               | Options     | Commentaires                                                                      |
 +=========================+=============+===================================================================================+
 |Install PHP Unit? (Y/N)  | Y(Yes)      | Si l'utilisateur souhaite procéder le processus d'installation qu'ils peuvent     |
 |                         |             | entrée comme Y.                                                                   |
 +-------------------------+-------------+-----------------------------------------------------------------------------------+
 |Install PHP Unit? (Y/N)  | N(No)       | Si l'utilisateur souhaite quitter le processus d'installation qu'ils peuvent      |
 |                         |             | entrée comme N.|                                                                  |
 +-------------------------+-------------+-----------------------------------------------------------------------------------+





Si l'utilisateur procède le processus d'installation les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered


 +---------------------+-------------------------+----------------+-------------------------------------------------------------------+
 | Paramètre           | chemin                  | Options        | Commentaires                                                      |
 +=====================+=========================+================+===================================================================+
 |Program data         | “/opt/phpunit (module   | Yes            | Si l'utilisateur de procéder installation avec le répertoire      |
 |directory (défaut)   | correspondant)”         |                | de données par défaut du programme qu'ils peuvent entrée          |
 |                     |                         |                | comme Oui                                                         |
 +---------------------+-------------------------+----------------+-------------------------------------------------------------------+
 |Program data         | Spécifique de           | No(Slash de    | Si l'utilisateur souhaite procéder à leur propre répertoire       |
 |directory            | l'utilisateur           | fin)           | de données de programme, ils peuvent entrée comme N, et dans la   |
 |                     |                         |                | main préciser leur propre emplacement                             |
 +---------------------+-------------------------+----------------+-------------------------------------------------------------------+
 |Program executor     | “/usr/bin”              | Yes            | Si l'utilisateur de procéder installation avec le répertoire      |
 |directory (défaut)   |                         |                | programme d'exécuteur défaut qu'ils peuvent entrée                |
 |                     |                         |                | comme Oui                                                         |
 +---------------------+-------------------------+----------------+-------------------------------------------------------------------+
 |Program executor     | Spécifique de           | No(Slash de    | Si l'utilisateur souhaite procéder à leur propre répertoire       |
 |directory            | l'utilisateur           | fin)           | programme d'exécuteur testamentaire, ils peuvent entrée comme N,  |
 |                     |                         |                | et dans la main indiquer qu'ils possèdent emplacement.|           |
 +---------------------+-------------------------+----------------+-------------------------------------------------------------------+

Enfin, l'installation de l'unité PHP est terminée. Représentant de manière visuelle sur le processus d'installation de la capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpunit install
 Install PHP Unit ? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          PHP Unit !         *
 *******************************
 What is the program data directory? Found "/opt/phpunit" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone -b 3.5 'https://github.com/sebastianbergmann/phpunit.git'  /tmp/phpunit/phpunitCloning into '/tmp/phpunit/phpunit'...

 remote: Counting objects: 50529, done.
 Receiving objects:  71% (35876/50529), 12.02 MiB | 41.00 KiB/s
 Receiving objects:  95% (48003/50529), 16.82 MiB | 38.00 KiB/s
 Receiving objects:  95% (48254/50529), 16.86 MiB | 40.00 KiB/s
 Receiving objects:  96% (48508/50529), 16.95 MiB | 43.00 KiB/s



 remote: Total 50529 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (50529/50529), 17.91 MiB | 36.00 KiB/s, done.
 Resolving deltas: 100% (26834/26834), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/dbunit.git'  /tmp/phpunit/dbunitCloning into '/tmp/phpunit/dbunit'...
 remote: Counting objects: 4596, done.
 remote: Total 4596 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4596/4596), 1.04 MiB | 31.00 KiB/s, done.
 Resolving deltas: 100% (3183/3183), done.
 Checking connectivity... done.
 git clone -b 1.2 'https://github.com/sebastianbergmann/php-file-iterator.git'  /tmp/phpunit/php-file-iteratorCloning into '/tmp/phpunit/php-file-iterator'...
 remote: Counting objects: 453, done.
 remote: Total 453 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (453/453), 60.66 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (188/188), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-code-coverage.git'  /tmp/phpunit/php-code-coverageCloning into '/tmp/phpunit/php-code-coverage'...
 remote: Counting objects: 7650, done.
 remote: Total 7650 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (7650/7650), 2.77 MiB | 17.00 KiB/s, done.
 Resolving deltas: 100% (3671/3671), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-token-stream.git'  /tmp/phpunit/php-token-streamCloning into '/tmp/phpunit/php-token-stream'...
 remote: Counting objects: 1234, done.
 remote: Total 1234 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (1234/1234), 201.76 KiB | 41.00 KiB/s, done.
 Resolving deltas: 100% (565/565), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-mock-objects.git'  /tmp/phpunit/phpunit-mock-objectsCloning into '/tmp/phpunit/phpunit-mock-objects'...
 remote: Counting objects: 4703, done.
 remote: Total 4703 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4703/4703), 837.24 KiB | 104.00 KiB/s, done.
 Resolving deltas: 100% (2910/2910), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-selenium.git'  /tmp/phpunit/phpunit-seleniumCloning into '/tmp/phpunit/phpunit-selenium'...
 remote: Counting objects: 8115, done.
 remote: Total 8115 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (8115/8115), 2.07 MiB | 28.00 KiB/s, done.
 Resolving deltas: 100% (4762/4762), done.
 Checking connectivity... done.
 git clone 'https://github.com/phpengine/ptconfigure-phpunit-php-timer'  /tmp/phpunit/php-timerCloning into '/tmp/phpunit/php-timer'...
 remote: Counting objects: 253, done.
 remote: Total 253 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (253/253), 31.55 KiB | 12.00 KiB/s, done.
 Resolving deltas: 100% (126/126), done.
 Checking connectivity... done.
 git clone 'https://github.com/sebastianbergmann/php-text-template.git'  /tmp/phpunit/php-text-templateCloning into '/tmp/phpunit/php-text-template'...
 remote: Counting objects: 209, done.
 remote: Total 209 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (209/209), 33.69 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (92/92), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPUnit35: Success
 ------------------------------
 Installer Finished
 ******************************

avantages
------------

* Ce module facilite l'utilisateur dans l'installation de PHP Unité de la version GC Repo.
* L'utilisateur peut choisir leur propre chemin pour le répertoire des données du programme et l'exécuteur
* Les paramètres utilisés pour déclarer l'aide et les installations ne sont pas sensibles à la casse, qui est ajouté tout avantage par rapport 
  aux autres.
* Il est bien de choses à faire dans les deux cent OS et ainsi que dans ubuntu.
