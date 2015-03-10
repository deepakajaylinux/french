=======
SVN
=======


synopsis
------------

Ce module aide les utilisateurs à la manipulation des fonctions de caisse. Apache Subversion (souvent abrégé SVN, après le nom de la commande svn) est un système de gestion des versions de logiciels et de contrôle de révision distribué comme logiciel libre sous licence Apache. [1] Les développeurs utilisent Subversion pour conserver les versions actuelles et historiques de fichiers tels que le code source, web pages, et la documentation. Son objectif est d'être un successeur essentiellement compatible avec Versions System largement utilisé (CVS). Voyons comment ce module facilite la manipulation des fonctions de caisse.

Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le SVN. Il énumère les autres paramètres de SVN. Il décrit également la syntaxe pour utiliser les fonctions de caisse. La commande d'aide pour le module SVN est représentée ci-dessous.

.. code-block:: bash

	ptdeploy svn help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide sous SVN.

.. code-block:: bash

 kevell@corp:/# ptdeploy svn help
 ******************************


  This command is part of Default Modules and handles Checkout Functions.

  Checkout, checkout, co

          - perform a checkout into configured projects folder. If you don't want to specify target dir but do want
          to specify a branch, then enter the text "none" as that parameter.
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum {optional target dir} {optional branch}
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum none {optional branch}

 ------------------------------
 End Help
 ******************************

Comment faire pour utiliser les fonctions de caisse
-------------------------------------------------------

La syntaxe pour utiliser le contrôle des fonctions en vertu svn est donnée ci-dessous.
.. code-block:: bash

		ptdeploy svn co https: // svnhub.com/ phpengine/yourmum



Après être entré dans l'ordre donné ci-dessus, l'exécution de la fonction de commande commence comme décrit dans le tableau ci-dessous,

.. cssclass:: table-bordered


 +------------------------------+-------------------------------------------+----------+----------------------------------------------+
 | Paramètres                   | Autres paramètres                         | options  | Commentaires                                 |
 +==============================+===========================================+==========+==============================================+
 |Perform a clone/download of   | Au lieu de co, nous pouvons utiliser      | Y(Yes)   | Si l'utilisateur doit effectuer un clone /   |
 |files? (Y/N)                  | Checkout aussi                            |          | téléchargement de fichiers qu'ils peuvent    |
 |                              |                                           |          | entrée comme Y.                              |
 +------------------------------+-------------------------------------------+----------+----------------------------------------------+
 |Perform a clone/download of   | Au lieu de co, nous pouvons utiliser      | N(No)    | Si l'utilisateur ne est pas dans le besoin   |
 |files? (Y/N)                  | Checkout aussi                            |          | d'effectuer un clone / téléchargement de     |
 |                              |                                           |          | fichiers qu'ils peuvent entrée comme N.|     |
 +------------------------------+-------------------------------------------+----------+----------------------------------------------+

Si l'utilisateur procède la fonction de commande par l'entrée en Y, les étapes suivantes sont impliqués comme décrit ci-dessous.

Etape 1:

Également modifier les autorisations / propriétaire? (Y / N)

L'utilisateur dispose à l'entrée que Y ou N en fonction de leur volonté de changement des permissions / propriétaire.

Étape 2:

Quel utilisateur est Apache Web Server fonctionne comme?

L'utilisateur doit entrer le nom d'utilisateur exécutant le serveur Web Apache.

Etape 3:

Elle implique le processus de modification des autorisations de dossier, et le propriétaire du dossier.

La capture d'écran ci-dessous représente imagée sur le processus et le fonctionnement de commander les fonctions.

.. code-block:: bash




avantages
-----------

* Il est bien de choses à faire dans les deux Ubuntu et ainsi que dans cent OS.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse.
* L'utilisateur peut effectuer et de surveiller les fonctions de caisse en utilisant cette SVN.
