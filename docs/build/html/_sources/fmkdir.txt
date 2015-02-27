========
Mkdir
========


synopsis
------------

Ce module aide à créer un répertoire. L'utilisateur peut spécifier le chemin tout en déclarant création de répertoire ou au moment de l'exécution de la création d'un répertoire. Elle peut être réalisée soit dans la machine à distance ou local. Voyons comment ce module contribue à créer un répertoire.

Commande Aide
---------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le Mk Dir. La commande help répertorie les autres paramètres de MK Dir. . Il décrit également la syntaxe pour la création d'un répertoire de deux manières différentes, soit au moment de la déclaration ou au moment de l'exécution. . La commande d'aide pour MKdir est indiqué ci-dessous.

.. code-block:: bash

	ptconfigure mkdir help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de MK dir.

.. code-block:: bash

	kevell@corp:/# ptconfigure Mkdir help
	******************************


        This command handles file copying functions.

         Mkdir, mkdir

        - path
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure mkdir path
        example: ptconfigure mkdir path --yes --path="/path/to/new/directory"

	------------------------------
	End Help
	******************************

	
Autres paramètres
-------------------------

Tout en utilisant les commandes de l'aide et la création d'un répertoire, au lieu de mkdir Mkdir peuvent également être utilisés.

Création d'un Mk Dir
---------------------

Création d'un Dir Mk peut se faire de deux façons différentes:

.. rubric:: Either at run-time

.. code-block:: bash

	Example: ptconfigure mkdir path

.. rubric:: Or, at the time of declaration

.. code-block:: bash

	Example: ptconfigure mkdir path --yes --path="/path/to/new/directory"

La capture d'écran ci-dessous illustre la seconde façon de créer un répertoire.

.. code-block:: bash

	kevell@corp:/# ptconfigure mkdir path --yes --path="/kevellsdoc"
	
	[Pharaoh Logging] [Mkdir] Executing mkdir /kevellsdoc
	******************************


	Mkdir Result: Success
	------------------------------
	Mkdir Finished
	******************************

avantages
------------

* Les paramètres utilisés dans l'aide et la création d'un opérations d'annuaire ne sont pas sensibles à la casse qui est un avantage 
  supplémentaire en rapport aux autres.
* Création d'un répertoire peut être définie de deux manières différentes que le temps de déclaration ou au moment de l'exécution.
* Elle peut être réalisée à la fois dans la machine locale ou distante.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
