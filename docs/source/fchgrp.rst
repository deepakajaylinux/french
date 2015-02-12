==============
chgrp       
==============

synopsis
-----------

Fichiers et répertoires appartiennent à la fois propriétaire et un groupe. Un groupe est généralement constitué d'un ensemble d'utilisateurs, tous appartenant à un même groupe. La première série de trois est la lecture, d'écriture et d'exécution pour le propriétaire du fichier.

Un groupe peut également être constitué par un seul utilisateur, normalement l'utilisateur qui a créé le fichier. Chaque utilisateur sur le système, y compris l'utilisateur root, est attribué son propre groupe dont il ou elle est le seul membre, l'accès uniquement par l'utilisateur. La deuxième série de trois est la lecture, d'écriture et d'exécution pour toute personne qui appartient au groupe de l'utilisateur pour le fichier.
L'utilisateur root, l'administrateur du système, propriétaire de la plupart des fichiers système qui appartiennent également au groupe racine, dont seul l'utilisateur root est membre. La plupart des fichiers de l'administration, comme les fichiers de configuration dans le répertoire / etc, sont la propriété de l'utilisateur root et appartiennent au groupe racine. Seul l'utilisateur root a le droit de les modifier, alors que les utilisateurs normaux peuvent lire et, dans le cas de programmes, aussi les exécuter

Commande Aide
---------------------

Cette commande permet de déterminer l'utilisation de changement module de groupe. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        cleopatra Chgrp help

La représentation picturale de la capture d'écran ci-dessous est donné,

.. code-block:: bash

 kevell@corp:/#  cleopatra Chgrp help
 ******************************


  This command handles file group ownership changing functions.

  Chgrp, chgrp

        - path
        Will change the file group ownership of a path
        example: cleopatra chgrp path --yes --guess --recursive --path=/a/file/path --group=golden


 ------------------------------
 End Help
 ******************************

chemin
---------

Lorsque l'utilisateur a besoin de changer la propriété de groupe de fichiers d'un chemin, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
        
	        cleopatra chgrp path –yes –guess –recursive –path=/”File path” –group=”group name”

Alternative Paramètre
-----------------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande.

chgrp, Chgrp

Par exemple: cleopatra Chgrp path/ cleopatra chgrp path

avantages
-------------

* Bien que d'autres utilisateurs peuvent être en mesure d'accéder à un fichier, seul le propriétaire peut modifier ses autorisations. Si vous 
  voulez donner un autre utilisateur de contrôler plus d'un des permissions de votre fichier, vous pouvez changer le propriétaire du fichier 
  de vous-même à l'autre utilisateur.
* Vous pouvez également modifier le groupe d'un fichier et de répertoires, en utilisant la commande chgrp. chgrp prend comme premier argument 
  le nom de la nouvelle groupe pendant fichiers ou répertoires.
