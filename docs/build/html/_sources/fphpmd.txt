=========
PHPMD
=========

synopsis
----------------

PHP MessDeductor est un spin-off de PHP dépendent et vise à être un équivalent de PHP de l'outil Java bien connu PMD. PHPMD peut être considéré comme une application frontend conviviale pour le flux de métriques brute mesurée par PHP dépendent. Garantie générale ou GC est la gamme des actifs qui sont acceptées, à un moment donné, à titre de garantie dans le marché des pensions par la majorité des intermédiaires du marché et à un taux de repo très similaire. Ce est approprié avec Ubuntu et cent OS.

Commande Aide
----------------------

  Il faut une base de code source de PHPMD donné et chercher plusieurs problèmes potentiels dans cette source. PHPMD est un jeune projet et il ne fournit un ensemble limité de règles pré définis, comparativement à PMD, qui détectent le code odeurs et les erreurs possibles dans le code source analysé. La caisse de la section des règles pour en savoir plus sur les règles allimplemented. La commande d'aide suivant guide l'utilisateur à installer le module phpmd.

.. code-block:: bash

		ptconfigure PHPMD help

La capture d'écran suivante vizualize ses fonctions.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPMD help
 ******************************


  This command allows you to install PHPMD from a GC Repo.

  PHPMD

        - install
        Installs the latest GC Repo version of PHPMD
        example: ptconfigure phpmd install

 ------------------------------
 End Help
 ******************************



installation
-------------------------

Au moment PHPMD est livré avec les trois moteurs de rendu suivants:

* Xml, qui formate le rapport au format XML.
* Texte, format textuel simple.
* Html, seul fichier HTML avec des problèmes possibles.

La commande utilisée pour installer le PHPMD à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash

		ptconfigure PHPMD install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format d'écran.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpmd install
 Install PHP Mess Detector ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mess Dt.        *
 *******************************
 What is the program data directory? Found "/opt/phpmd" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/ptconfigure-phpmd.git'  /tmp/phpmd/phpmdCloning into '/tmp/phpmd/phpmd'...
 remote: Counting objects: 356, done.
 remote: Total 356 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (356/356), 306.45 KiB | 9.00 KiB/s, done.
 Resolving deltas: 100% (239/239), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 PHPMD: Success
 ------------------------------
 Installer Finished
 ******************************



Options
------------


.. cssclass:: table-bordered


 +---------------------------------+-----------+--------------------------+-----------------------------------------------------------+
 | paramètres                      | options   | Annuaire (par défaut)    | commentaires                                              |
 +=================================+===========+==========================+===========================================================+
 |Data directory (par défaut)      | Yes       | “/opt/PHPMD”             | Il va installer le module PHPMD sous ptconfigure          |
 +---------------------------------+-----------+--------------------------+-----------------------------------------------------------+
 |Data directory                   | No        | End slash                | L'utilisateur doit spécifier le chemin d'un.              |
 +---------------------------------+-----------+--------------------------+-----------------------------------------------------------+
 |Executor directory (par défaut)  | Yes       | “/usr/bin”               | Il répertoire d'installation de l'exécuteur               |
 +---------------------------------+-----------+--------------------------+-----------------------------------------------------------+
 |Executor directory               | No        | No trailing slash        | L'utilisateur donne entrée comme nom de répertoire|       |
 +---------------------------------+-----------+--------------------------+-----------------------------------------------------------+
         

 


avantages
------------------

Excessive PublicCount:

Un grand nombre de méthodes publiques et attributs déclarés dans une classe peut indiquer la classe peut avoir besoin d'être brisé comme un effort accru sera
être nécessaire pour tester vivement.

Excessive ParameterList:

Listes de paramètres longs peuvent indiquer qu'un nouvel objet devrait être créé pour envelopper les nombreux paramètres. Fondamentalement, essayez de regrouper les paramètres ensemble.


Cyclomatic Complexity:

La complexité est déterminée par le nombre de points de décision dans un procédé plus un pour l'entrée de méthode.


Superglobales:

Accéder à une variable super-globale directement est considéré comme une mauvaise pratique. Ces variables doivent être encapsulées dans des objets qui sont fournis
par un cadre, par exemple.


Short Variable:

Détecte quand un champ, local, ou le paramètre a une très courte nom.


VariableLongue:

Détecte quand un champ, une variable formelle ou locale est déclarée avec un nom long.

