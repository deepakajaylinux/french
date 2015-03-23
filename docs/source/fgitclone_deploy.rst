==========
GitClone
==========

synopsis
------------

Le but ultime de ce module est de gérer le contrôle des fonctions. Il peut effectuer le contrôle des fonctions dans le dossier du projet
utilisateur.

La nature de travail de ce module consiste Clonage d'un référentiel dans un répertoire nouvellement créé, crée branches à distance de suivi pour chaque branche dans le référentiel cloné et crée, vérifie sur une branche fourchue initial qui est de la branche cloné repositoryâ actif € ™ s.
Voyons comment ce module facilite les utilisateurs dans la gestion du contrôle des fonctions, et aussi sur la façon d'utiliser ce module parmi les sujets à venir.


Commande Aide
-------------------


La commande d'aide est un manuel d'utilisation brève. Il met en évidence la fonction principale de ce module, répertorie les aboutissants d'autres paramètres qui peuvent être utilisés dans la déclaration, et explique également sur la syntaxe et options possibles de l'utilisation de la vérification des fonctions sous une seule option en utilisant la commande d'aide comme indiqué ci-dessous,

.. code-block:: bash

	ptdeploy GitClone help


La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu git clone.

.. code-block:: bash

 kevell@corp:/# ptdeploy GitClone help
 ******************************


  This command is part of Default Modules and handles Checkout Functions.

  clone, co

          - perform a checkout into configured projects folder. If you don't want to specify target dir but do want
          to specify a branch, then enter the text "none" as that parameter.
          example: ptdeploy git co https://github.com/phpengine/yourmum {optional target dir} {optional branch}
          example: ptdeploy git co https://github.com/phpengine/yourmum none {optional branch}

 ------------------------------
 End Help
 ******************************


Comment faire pour utiliser les fonctions de caisse
-----------------------------------------------------

La syntaxe pour utiliser le contrôle des fonctions en vertu git clone est donnée ci-dessous.

.. code-block:: bash

	ptdeploy git co https: // github.com/ phpengine/yourmum

Après être entré dans l'ordre donné ci-dessus, l'exécution de la fonction de commande commence comme décrit dans le tableau ci-dessous,

.. cssclass:: table-bordered

 +-------------------------+--------------------------------+-------------+-----------------------------------------------------------+
 | paramètre               | Autres paramètres              | Option      | commentaires                                              |
 +=========================+================================+=============+===========================================================+
 |Perform a clone/download | au lieu de co nous pouvons     | Y(Yes)      | Si l'utilisateur doit effectuer un clone / téléchargement |
 |of files? (Y/N)	   | utiliser, clone                |             | de fichiers qu'ils peuvent entrée comme Y.                |
 +-------------------------+--------------------------------+-------------+-----------------------------------------------------------+
 |Perform a clone/download | au lieu de co nous pouvons     | N(No)       | Si l'utilisateur ne est pas besoin d'effectuer un clone / |
 |of files? (Y/N)	   | utiliser, clone                |             | téléchargement de fichiers qu'ils peuvent comme N|        |
 +-------------------------+--------------------------------+-------------+-----------------------------------------------------------+

 

.. code-block:: bash


 kevell@corp:/# ptdeploy gitclone co https://github.com/PharaohTools/ptvirtualize.git 

 Perform a clone/download of files? (Y/N) 
 y 
 What's git repo to clone from? 
 https://github.com/PharaohTools/ptvirtualize.git 
 Cloning into 'ptvirtualize'... 
 remote: Counting objects: 4673, done. 
 remote: Total 4673 (delta 0), reused 0 (delta 0), pack-reused 4673 
 Receiving objects: 100% (4673/4673), 2.20 MiB | 128.00 KiB/s, done. 
 Resolving deltas: 100% (2971/2971), done. 
 Checking connectivity... done. 
 Also change permissions/owner? (Y/N) 
 n 
 ****************************** 


 1In GitClone View 
 ****************************** 

						




avantages
-----------

* Il est bien de choses à faire dans les deux Ubuntu et ainsi que dans cent OS.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse.
* L'utilisateur peut effectuer et de surveiller les fonctions de caisse sous git clone.
* Lors de la vérification des fonctions, l'utilisateur peut spécifier le répertoire cible, pas besoin de spécifier la branche.
