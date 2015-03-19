=============
Test module
=============

synopsis
--------------

TestModule est le plus populaire jrush tests de module, à partir de ce contrôle sur l'extension de fichier et de faire un usage. TestModule est un cadre, mais peut être utilisé de concert avec les autre article de test. Ainsi, TestModule fournit uniquement la ligne de base test de fonctionnement, laissant les autres bibliothèques pour implémenter une fonctionnalité plus précise et sophistiquée. Il montre les actions en cours. C'est à l'aise avec Ubuntu et cent OS.


Commande Aide
-----------------------

La commande help guide les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans le testmodule. Il énumère les paramètres alternatifs de testmodule. Il décrit également la syntaxe pour le fonctionnement du module Jrush. La commande help pour testmodule s'affiche comme ci-dessous.


.. code-block:: bash

	jrush testmodules help

Après avoir tapé la commande, il répertorie les options comme action. L'image suivante le visualiser évidemment.



.. code-block:: bash

 kevell@corp:/# jrush TestModule help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update TestModule.

  TestModule, testmodule, test-module

        - action-one
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-one

        - action-two
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-two

 ------------------------------
 End Help
 ****************************************



Alternative Paramètre
--------------------------------

Alternativement à l'aide de Testmodule l'utilisateur peut utiliser les options suivantes.


Test Module, testmodule, test-module.

options
-------------

Il ya deux options sont disponibles. Ils sont comme suit.

* Action-one
* Action-two

Action-one
-----------------

Il montre les titres des articles. La commande utilisée pour faire un action est comme suit,


.. code-block:: bash

	jrush test-module action-one

Après donne la commande, il montre les détails actuels et les titres des articles. La capture d'écran représente le même.



.. code-block:: bash

 kevell@corp:/# jrush test-module action-one --config-file="/var/www/html/joomla/configuration.php"
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 TestModule Action One:
 -------------------------
 array(6) {
  [0]=>
  string(8) "About Us"
  [1]=>
  string(15) "Article 1 Title"
  [2]=>
  string(18) "Creating Your Site"
  [3]=>
  string(9) "article-1"
  [4]=>
  string(9) "article-2"
  [5]=>
  string(9) "article-3"
 }

 ------------------------------
 TestModule Action One Finished
 ****************************************



Action-two
-----------------

Il montre les titres des articles. La commande utilisée pour faire un action est comme suit,


.. code-block:: bash

	jrush testmodule action-two

Après donne la commande, il montre les détails actuels et les titres des articles.


avantages
----------------

* Vérifier les modules de façon correcte. 
* Non casse. * Moins de temps. 
* Le moins cher pour mettre à niveau de site simple.       
* Dernière mise à jour est disponible 
* adaptés aux travaux avec Ubuntu et centOS.
