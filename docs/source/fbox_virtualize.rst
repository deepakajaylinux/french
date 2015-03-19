=======
Box
=======

Synopsis
------------

Ce module aide les utilisateurs à manipuler et gérer les cases qui sont disponibles dans le ptvirtualize. Attendons de voir comment ce module fonctionne en manipulant les fonctions de boîte.


Commande Aide
---------------------

La commande help guide les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans le module de boîte. Il énumère les paramètres alternatifs de module de boîte. Il décrit également la syntaxe d'utilisation de l'add, remove, paquet liste des commandes. La commande help pour module de boîte s'affiche comme ci-dessous.

.. code-block:: bash
		
	ptvirtualize Box help

La syntaxe servant à déclarer la commande help n'est pas sensible à la casse qui est un atout supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide au titre de la boîte.


.. code-block:: bash

 kevell@corp:/# ptvirtualize Box help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to manage the Base boxes available to you in ptvirtualize

  Box, box

        - add
        Initialises the Box as usable by ptvirtualize
        example: ptvirtualize box add
        example: ptvirtualize box add --yes --guess
            --source="/home/dave/file.box" # where the box file is
            --target="opt/ptvirtualize/boxes" # will guess the dir next to ptvirtualize install dir
            --name="vanillaubuntu"

        - remove
        Removes the box as usable by ptvirtualize
        example: ptvirtualize box remove

        - package
        Packages a box as usable by ptvirtualize
        example: ptvirtualize box package
        example ptvirtualize box package --yes --guess
            --name="Vanilla Ubuntu 12.04 amd 64"
            --vmname="a4dc638f-2721-40c4-a943-2f2565c83fee" # use name or id of virtual machine
            --provider="virtualbox" # guess will use virtualbox
            --group="ptvirtualize"
            --slug="" # guess can generate this based on name field
            --description="A Vanilla install of Ubuntu..."
            --home_location="http://www.someplace.net/" # guess will set this to http://www.ptvirtualizeboxes.co.uk/
            --target="/opt/ptvirtualize/boxes" # save location, will guess /opt/ptvirtualize/boxes

        - list
        List boxes installed in ptvirtualize
        example: ptvirtualize box list

 ------------------------------
 End Help
 ******************************

Fonctions de ptvirtualize Box
----------------------------------

Comme l'illustre les fonctions de la boîte de ptvirtualize la commande help ci-dessus comprend les éléments suivants :

* Add
* Remove
* Package
* List

Add
-----

Add est utilisé pour initialiser la boîte comme utilisable par ptvirtualize. La syntaxe suivante permet d'ajouter une boîte de ptvirtualize.

.. code-block:: bash

	ptvirtualize box add

or

.. code-block:: bash

	ptvirtualize box add --yes --guess
	--source="/home/dave/file.box	(This line describes where the box is)
	--target="opt/ptvirtualize/boxes"	(This line guess the dir next to ptvirtualize install dir)
	--name="vanillaubuntu"

Par les moyens mentionnés ci-dessus, la boîte peut être ajoutée à un ptvirtualize.



Remove
-----------

Cette fonction est utilisée pour enlever la boîte comme utilisable par ptvirtualize. Cela peut se faire à l'aide de la commande ci-dessous :


.. code-block:: bash

	ptvirtualize box remove

Par les moyens mentionnés ci-dessus, la boîte peut être retirée d'un ptvirtualize.


Package
-----------

Cette fonction sert à empaqueter la boîte comme utilisable par ptvirtualize. Cela peut être implémenté à l'aide de la commande suivante :


.. code-block:: bash

	ptvirtualize box package

or

.. code-block:: bash

	ptvirtualize box package --yes --guess
	name="Vanilla Ubuntu 12.04 amd 64"
	vmname="a4.............." (This two lines represents the name and id of virtual machine)
	--provider="virtualbox" (guess will use virtual box)
	--group="ptvirtualize"
	--slug="" (The guess can generate this based on the name field)
	--description="A vanilla install of Ubuntu..."
	--home_location="http://www.someplace.net/" (guess will set this to http://www.ptvirtualizeboxes.co.uk/
	--target="/opt/ptvirtualize/boxes" (The location for saving)



Enfin, une boîte est emballée aussi utilisable par le ptvirtualize.


List
-----

Cette fonction est utilisée pour l'inscription les cases qui sont installés dans ptvirtualize. Cela peut être fait en utilisant la commande suivante,


.. code-block:: bash

	ptvirtualize box list

À l'aide de la commande ci-dessus, la liste des boîtes de ptvirtualize nouvellement installés s'affichera.



Alternative Paramètre
-------------------------------

* Box
* box


Dans la liste ci-dessus, aucun des paramètres alternatifs peut être utilisé dans la déclaration.

Avantages
-----------

* Les paramètres utilisés dans l'aide n'est pas sensible à la casse 
  qui est un atout supplémentaire alors que par rapport aux autres. 
* Il est aisée dans les deux Ubuntu ainsi que comme OS Cent.
* La syntaxe pour l'aide d'ajouter, supprimer, package, la liste ne 
  sont pas sensibles à la casse.

