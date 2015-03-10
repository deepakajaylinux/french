==========
FireFox
==========

synopsis
--------------

Ce module permet d'installer firefox. Ubuntu publie périodiquement des versions mises à jour. Il met en œuvre les normes Web actuelles et prévues. Soutien à long terme comprend les mises à jour pour le nouveau matériel, les correctifs de sécurité et mises à jour de l'infrastructure de cloud computing. Il est à l'aise avec Ubuntu et Cent OS.

Commande Aide
-------------------------

Cette commande peut fonctionner sur les objectifs et les commandes disponibles pour le module Firefox. Il explique également la commande pour installer firefox. Avant l'installation, l'utilisateur peut lire cette commande d'aide explique sa fonction.

.. code-block:: bash

              ptconfigure firefox help

L'image suivante vous aide également à comprendre clairement ce module.

.. code-block:: bash

	 kevells@corp:/# ptconfigure firefox help

	 ******************************


	 This command is part of Core and provides you  with a method by which you can install Firefox from your package
         manager

	 Firefox, firefox

        - install
        Installs Firefox
        example: ptconfigure firefox install

	------------------------------
	End Help
	******************************

installation
-------------------

Ce est un processus flagrante à installer le module firefox sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

              ptconfigure firefox install

Après clé dans la commande, il peut demande

Install Firefox? (Y/N) 

Dans le cas où l'entrée d'utilisateur en tant que Y, on peut installer firefox de l'emballage. Sinon, il peut quitter l'écran. Les captures d'écran suivantes peuvent l'expliquer.

.. code-block:: bash
	
	kevell@corp:/# ptconfigure firefox install

	Install Firefox? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          Firefox            *
	*******************************
	Creating /tmp/ptconfigure-temp-script-51942043520.sh
	chmod 755 /tmp/ptconfigure-temp-script-51942043520.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-51942043520.sh Permissions
	Executing /tmp/ptconfigure-temp-script-51942043520.sh
	Cloning into 'firefox'...
	remote: Counting objects: 78, done.
	remote: Total 78 (delta 0), reused 0 (delta 0)
	Unpacking objects: 100% (78/78), done.
	Checking connectivity... done.
	Temp File /tmp/ptconfigure-temp-script-51942043520.sh Removed
	Program Executor Deleted if existed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	Firefox: Success
	------------------------------
	Installer Finished
	******************************


Options
--------

.. cssclass:: table-bordered

 +-----------------------+-----------------------------------------------+-------------+--------------------------------------+
 | paramètres            | paramètre alternatif                          | option      | commentaires                         |
 +=======================+===============================================+=============+======================================+
 |ptconfigure firefox    | Au lieu d'utiliser firefox nous pouvons       | Y(Yes)      | Le système démarre processus         |
 |Install                | utiliser Firefox, firefox                     |             | d'installation qu'ils peuvent        |
 |                       |                                               |             | entrée comme Y                       |
 +-----------------------+-----------------------------------------------+-------------+--------------------------------------+
 |ptconfigure Firefox    | Au lieu d'utiliser firefox nous pouvons       | N(No)       | Système arrête processus             |
 |Install                | utiliser Firefox, firefox                     |             | d'installation|                      |
 +-----------------------+-----------------------------------------------+-------------+--------------------------------------+

avantages
-------------

* Firefox utilise support de nouveaux matériels et l'intégration de toutes les mises à jour publiées dans cette série à ce jour.
* Il est à l'aise avec Ubuntu et CentOS.
* Firefox ne est pas sensible à la casse.
* Confidentialité et sécurité mesures, la recherche intelligente

