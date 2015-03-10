=============
PTVirtualize
=============

synopsis
-----------

  ptvirtualize atteindre pour gérer le Virtualbox. Ce module permet d'installer sous ptconfigure. Répertoire de données et le répertoire de l'exécuteur peuvent spécifier lors de l'installation de ce module. Ce module est le plus à l'aise avec Ubuntu et cent OS.

Commande Aide
-------------

Cette commande d'aide à guider l'utilisateur sur module de ptvirtualize. Ce est adapté pour tout type de gens d'affaires. La commande d'aide montre une courte liste des commandes intégrées dans le module de ptvirtualize.

.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize help
	******************************


	This command allows you to install or update ptvirtualize.

	ptvirtualize, ptvirtualize

        - install
        Installs the latest version of ptvirtualize
        example: ptconfigure ptvirtualize install

	------------------------------
	End Help
	******************************

installation
------------

Installation d'un module de ptvirtualize est y compris les pilotes et plugins périphériques, acte de rendre le programme prêt à être exécuté. Lors de l'installation de ce module la commande suivante sera adoptée.

.. code-block:: bash

	ptconfigure ptvirtualize install

Après entrées de la commande du système peut poser

Installez ptvirtualize? (Y / N)

Si l'utilisateur donne ensuite ptvirtualize Y seront installés. La capture d'écran suivante le démontrent.

.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ptvirtualize         *
	*******************************
	What is the program data directory? Found "/opt/ptvirtualize" - use this? (Enter nothing for yes, no end slash)

	What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

	git clone 'https://github.com/PharaohTools/ptvirtualize.git'  /tmp/ptvirtualize/ptvirtualizeCloning into '/tmp/ptvirtualize/ptvirtualize'...
	remote: Counting objects: 4063, done.
	remote: Total 4063 (delta 0), reused 0 (delta 0)
	Receiving objects: 100% (4063/4063), 2.13 MiB | 393.00 KiB/s, done.
	Resolving deltas: 100% (2530/2530), done.
	Checking connectivity... done.
	Program Data folder populated
	Program Executor Deleted if existed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	ptvirtualize: Success
	------------------------------
	Installer Finished
	******************************

Si l'utilisateur donne N, alors il sortira de l'écran. La capture d'écran suivante le démontrent.

.. code-block:: bash

	kevells@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
	n
	******************************


	Single App Installer:
	--------------------------------------------
	ptvirtualize: Failure
	------------------------------
	Installer Finished
	******************************


Option
-----------

.. cssclass:: table-bordered

 +----------------------------------+-----------+------------------------+---------------------------------------------------------+
 | paramètres                       | option    | annuaire               | commentaire                                             |
 +==================================+===========+========================+=========================================================+
 |Data directory(Par défaut)        | YES       | “/opt/ptvirtualize”    | Il va installer ptvirtualize sous ptconfigure           |
 +----------------------------------+-----------+------------------------+---------------------------------------------------------+
 |Data directory                    | No        | Slash Fin              | L'utilisateur doit spécifier le chemin d'un.            |
 +----------------------------------+-----------+------------------------+---------------------------------------------------------+
 |Executor directory (Par défaut)   | Yes       | “/usr/bin”             | Il répertoire d'installation de l'exécuteur             |
 +----------------------------------+-----------+------------------------+---------------------------------------------------------+
 |Executor directory                | No        | Aucune slash           | L'utilisateur donne entrée comme nom de répertoire|     |
 +----------------------------------+-----------+------------------------+---------------------------------------------------------+



avantages
---------

* Utilisateurs d'Ubuntu peuvent simplement installer ptvirtualize du référentiel.
* Le véritable avantage de ptvirtualize réside dans sa performance.
* Intégration avec système d'exploitation hôte.
* Accessibilité de vitesse.
* Gérer boîte virtuelle.
