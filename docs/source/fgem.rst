====
Gem
====

synopsis
-----------

Ce module enveloppe tous les besoins des utilisateurs pour travailler avec GEM. Il couvre diverses fonctions, et dans la main favorise diverses fonctions à exercer.

RubyGems est un gestionnaire de paquets pour le langage de programmation Ruby qui fournit un format standard pour la distribution de programmes et bibliothèques Ruby (dans un format autonome appelé un "bijou"), un outil conçu pour gérer facilement l'installation de pierres précieuses, et un serveur pour les distribuer.

Voyons les diverses caractéristiques et la façon d'utiliser ce module parmi les sujets à venir.

Commande Aide
-------------------

La commande help instruit les utilisateurs quant à la finalité et diverses caractéristiques et la syntaxe pour la mise en œuvre de ces différentes caractéristiques. Il indique également les sorties de paramètres alternatifs qui peuvent être utilisés dans les déclarations. Le format de la syntaxe pour appliquer option d'aide en vertu de ce module, est donnée ci-dessous,

.. code-block:: bash

	ptconfigure gem help

Visualiser la sortie et le travail de l'option d'aide en vertu de ce module L'écran suivant.

.. code-block:: bash

 kevell@corp:/# ptconfigure gem help

 ******************************


  This command allows you to modify create or modify gems

  Gem, gem

        - create
        Create a new system gem, overwriting if it exists
        example: ptconfigure gem create --gemname="somename"

        - remove
        Remove a system gem
        example: ptconfigure gem remove --gemname="somename"

        - set-password
        Set the password of a system gem
        example: ptconfigure gem set-password --gemname="somename" --new-password=                                                                                        "somepassword"

        - exists
        Check the existence of a gem
        example: ptconfigure gem exists --gemname="somename"

        - show-groups
        Show groups to which a gem belongs
        example: ptconfigure gem show-groups --gemname="somename"

        - add-to-group
        Add gem to a group
        example: ptconfigure gem add-to-group --gemname="somename" --groupname="so                                                                                        megroupname"

        - remove-from-group
        Remove gem from a group
        example: ptconfigure gem remove-from-group --gemname="somename" --groupnam                                                                                        e="somegroupname"

 ------------------------------
 End Help
 ******************************


Différentes caractéristiques de Gem
--------------------------------------

Comme le montre de la commande d'aide ci-dessus, les diverses caractéristiques de Gem est énumérés ci-dessous,

* Créer
* Retirer
* Définir mot de passe
* Existe
* Show_groups
* Add_to_group
* Remove_from_group


Voyons en détail sur ces fonctions.

créer
--------

Cette fonction vise à créer un nouveau joyau du système, et ainsi que écrase en cas de déjà existant. Cette fonction de gemme utilisant ce module peut être atteint par la syntaxe suivante,

.. code-block:: bash

	ptconfigure gem create --gemname="somename"

A la place de gemname l'utilisateur peut spécifier le nom de la gemme qui doit être créé. Après avoir saisi la commande comme indiqué ci-dessus, le nouveau bijou sera créé avec le nom spécifié.

RETIRER
-----------

Cette fonction vise à la suppression d'un joyau existant. Cette fonction de gemme utilisant ce module peut être atteint par la syntaxe suivante,

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"

A la place de gemname l'utilisateur peut spécifier le nom de la gemme qui doit être supprimé. Après avoir saisi la commande comme indiqué ci-dessus, le joyau spécifié sera supprimé.

MOT DE PASSE SET
--------------------

Cette fonction facilite la création d'un nouveau mot de passe pour un joyau du système selon les exigences. Ceci peut être effectué en appliquant la commande comme indiqué ci-dessous,

.. code-block:: bash

	ptconfigure gem set-password --gemname="somename" --new-password="somepassword"

Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les deux champs,

* Nom Gem
* Nouveau mot de passe

Après avoir spécifié les deux champs dans le format de commande mentionné ci-dessus, le nouveau mot de passe pour le joyau spécifiée sera créé.

EXISTS
--------

Cette fonction vise à vérifier l'existence d'un bijou. Cela peut être fait simplement, en utilisant la commande ci-dessous,

.. code-block:: bash

	ptconfigure gem exists --gemname="somename"

Après l'application de la commande comme ci-dessus, l'existence d'un bijou mentionné sera assurée avec les résultats.

Afficher les groupes
--------------------

Cette fonction aide les utilisateurs de connaître à quel groupe ne le joyau appartient. Ceci peut être réalisé simplement en utilisant la commande ci-dessous,

.. code-block:: bash

	ptconfigure gem show-groups --gemname="somename"

L'utilisateur doit indiquer le nom de la gemme dans le domaine de gemname, afin de connaître les détails de son groupe.

AJOUTER _TO_GROUP
-----------------------

L'objectif principal de cette fonction est d'ajouter le joyau nécessaire pour le groupe requis en appliquant simplement la commande comme indiqué ci-dessous,

.. code-block:: bash

	ptconfigure gem add-to-group --gemname="somename" --groupname="somegroupname"

Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les deux domaines suivants selon leurs besoins dans le format de commande ci-dessus mentionné,

* Gemname
* Nom de groupe

REMOVE_FROM_GROUP
------------------

L'objectif principal de cette fonction est de supprimer le joyau d'un groupe en appliquant simplement la commande comme indiqué ci-dessous,

.. code-block:: bash

	ptconfigure gem remove-from-group --gemname="somename" --groupname="somegroupname"

Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les deux domaines suivants selon leurs besoins dans le format de commande ci-dessus mentionné,

* Gemname
* Nom de groupe

Autres paramètres
-------------------

Les autres paramètres de ce module, chacun pouvant être utilisés dans la déclaration est,

* Gem
* gem

avantages
---------

* Les paramètres utilisés déclarant aide et d'autres caractéristiques différentes de gemme ne sont pas sensibles à la casse.
* Il est bien de choses à faire dans les deux cents os et ainsi que dans Ubuntu.
* L'utilisation de ce module, l'utilisateur peut créer et modifier ainsi que la gemme selon leurs besoins.
* L'existence d'un bijou peut être assuré dans ce module.
