=====
PECL
=====

synopsis
----------

PECL signifie «Positive émetteur logique à couplage". Pecl sont sorties logiques différentiels couramment utilisés dans les circuits de distribution d'horloge à grande vitesse. Cette commande permet à l'utilisateur de créer, supprimer, setpassward, existe. Les activités de groupe aussi possible grâce à cette commande. Cette fonction de commande principale est basée sur le système. Il est adapté avec Ubuntu et CentOS.

Commande Aide
--------------

Pecl rend le développement de package une brise: il fonctionne avec existent, modifier, créer, pour soutenir l'ensemble passward pecl système. Avec pecl, la modification d'un package devient si facile que ce sera la configuration par défaut de l'utilisateur lorsque l'utilisateur est en train d'écrire une quantité importante de code.

.. code-block:: bash

		ptconfigure pecl help


Explique sa fonction La capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptconfigure PECL help

 ******************************


  This command allows you to modify create or modify pecls

  PECL, pecl

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************




créer
------

Cette commande permet à l'utilisateur de créer un nouveau système PECL. L'écrasement est possible en cas d'existence. Nouveau nom de PECL peut être mentionné dans une seule commande lui-même.

La commande utilisée pour créer est la suivante

.. code-block:: bash

		ptconfigure pecl create 

Après l'entrée que la commande ci-dessus, il commence à créer PECL. En cas de fichier existant le message d'indication apparaît. La commande et explique sa fonction avec les captures d'écran.

.. code-block:: bash

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"



supprimer
------------

Cette commande permet à l'utilisateur de supprimer un PECL. Amovible nom de PECL peut être mentionné dans une seule ligne de commande elle-même.
La commande utilisée pour créer est la suivante

.. code-block:: bash

		ptconfigure pecl remove 


Après l'entrée que la commande ci-dessus, il commence à enlever PECL. En cas de fichier déjà enlevé de la pecl le message d'indication apparaît. La commande et explique sa fonction avec les captures d'écran.

.. code-block:: bash

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"



Set passward
-------------

Setpassward utilisé pour exécuter une commande particulière avec les permissions root dans PECL. La chose intéressante est que lorsque l'utilisation de l'utilisateur passward pour une commande particulière, le système demande à l'utilisateur le mot de passe de l'utilisateur actuel. La commande utilisée pour créer est la suivante

.. code-block:: bash

	ptconfigure pecl  set-passward


Pecl nom et nouvelle passward mentionnent également dans la même ligne de commande. Cela rend un autre avantage de ce module. La capture d'écran suivante visualiser ses fonctions.

.. code-block:: bash

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"



existe
-----------

Cette commande permet de vérifier l'existence d'un PECL. Commande simple rend ce travail de commande correctement. Tout d'abord il vérifie nom de PECL dans le système, alors il indique se il existe déjà ou non. La commande suivante permet de faire cette function

.. code-block:: bash

		ptconfigure pecl Exists


La capture d'écran suivante visualiser ses fonctions.

.. code-block:: bash

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"


Show-Groupe
------------

Cette commande permet de contrôler le groupe de travail d'un PECL. Commande simple rend ce travail de commande correctement. Tout d'abord, il vérifie le nom du groupe puis pecl nom dans le système, alors il indique le nom du groupe auquel appartient un PECL. La commande suivante permet de faire cette function

.. code-block:: bash

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"


Ajouter à-Groupes
------------------

Cela facilite à l'utilisateur d'ajouter un PECL à un groupe. Tout en ajoutant qu'il peut demande nom de PECL et le nom du groupe. L'utilisateur peut entrer dans le selon leur souhait.

.. code-block:: bash
   
		ptconfigure pecl add-to-group



Après la saisie de la commande il ajouter un pecl dans le groupe.

.. code-block:: bash

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"



Retirez-de-groupe
------------------

Cette commande permet à l'utilisateur de supprimer un pecl du groupe. Amovible nom de PECL peut être mentionné dans une seule ligne de commande elle-même.

La commande utilisée pour créer est la suivante


.. code-block:: bash

		ptconfigure pecl remove-from-group 


Après l'entrée que la commande ci-dessus, il commence à enlever pecl du groupe. En cas de fichier déjà enlevé de la pecl le message d'indication apparaît. La commande et explique sa fonction avec les captures d'écran.

.. code-block:: bash

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"


avantages
----------

* Sensibilité non de cas.
* Eh bien-to-do dans Ubuntu et CentOS.
* Basse consommation d'énergie.
* Créer un nouveau système pecl
* Supprimer un pecl
* Ajouter au groupe est possible
* Supprimer le groupe est possible
* Voir le groupe est possible
