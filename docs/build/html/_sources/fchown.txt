=======
Chown
=======

synopsis
-------------

Ce module permet de changer la permission du propriétaire. Il peut changer la permission sur fichier ou répertoire individuel. Avant que vous devez être conscient de l'autorisation par défaut attribué à vos fichiers et répertoires au moment de sa création.

Commande Aide
-----------------------

Cette commande d'aide explique à propos de l'installation d'un module particulier. La commande d'aide est facile à utiliser par l'utilisateur final. Il indique également les paramètres de substitution qui sont utilisés dans la déclaration. La commande suivante guide l'utilisateur sur la manipulation de ce module.

.. code-block:: bash
	
	cleopatra chown help

Après avoir donné la commande, la commande affiche la liste des options d'aide. Les captures d'écran suivantes donneront effet visuel pour l'utilisation de ce module.

.. code-block:: bash

	Kevell@corp:/# cleopatra chown help
	******************************

	 This command handles file user ownership changing functions.

	  Chown, chown

        - path
        Will change the user ownership of a path
        example: cleopatra chown path --yes --guess --recursive --path=/a/file/path --owner=golden

	------------------------------
	End Help
	******************************

chemin
--------

Ce est un excellent processus pour ce module sous Cléopâtre légèrement en utilisant la commande ci-dessous,

.. code-block:: bash

	cleopatra chown path –yes—guess—recursive—path=/Cleopatra—owner=Kevells

Ensuite, nous pouvons entrer dans l'entrée.
Entrez propriété utilisateur
Après avoir tapé le nom du propriétaire
Il affichera Chown résultat succès.


Ce est visuellement représentée par la capture d'écran suivante.


.. code-block:: bash

	kevell@corp:/# cleopatra chown path --yes --guess --recursive --path=/phj.php --owner=deepak

	Enter ownership user:
	deepak
	[Pharaoh Logging] [Chown] Executing chown -R deepak /phj.php
	******************************


	Chown Result: Success
	------------------------------
	Chown Finished
	******************************

option
---------

.. cssclass:: table-bordered



        +------------------------------------------------+------------+----------------------------+-----------------------------+
        |       Parameters                               | Required   | option                     | Comments                    |
        +================================================+============+============================+=============================+
        |Chown                                           | Yes        |                            |                             |
        +------------------------------------------------+------------+----------------------------+-----------------------------+
        |Path                                            | Yes        |                            |L'utilisateur doit donner le |     
        |                                                |            |                            |chemin                       |
        +------------------------------------------------+------------+----------------------------+-----------------------------+
        |Owner                                           | Yes        | Chown                      |                             |
        +------------------------------------------------+------------+----------------------------+-----------------------------+
        |Owner                                           | No         | Chown                      |L'utilisateur donne entrée   |
        |                                                |            |                            |que non, il vous demandera   |
        |                                                |            |                            |le nom du propriétaire|      |
        +------------------------------------------------+------------+----------------------------+-----------------------------+




avantages
----------------

  * Le module peut changer le propriétaire à tout moment avec Cléopâtre.
  * Tout en faisant processus récursif si vous changez un seul fichier l'ensemble du dossier peut également être modifié.
  * Nous pouvons vérifier l'état actuel du propriétaire.

