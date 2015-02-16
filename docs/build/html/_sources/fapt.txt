====
Apt
====

synopsis
-----------

Le principal objectif de ce module est apte à créer de nouveaux apparts et vise à modifier les apparts déjà existants ainsi. Ce module possède une collection de diverses caractéristiques pour accéder et modifier les apparts sur la base des exigences des utilisateurs.

Les thèmes à venir porte sur la façon d'utiliser ce module et également sur les différents aspects de ce module pour accéder apt.

Commande Aide
------------------------

La commande d'aide est un manuel d'utilisation brève qui facilite les utilisateurs d'obtenir conscience concernant l'utilisation, la manipulation des méthodologies de ce module pour effectuer des fonctions différentes. Il indique également les sorties de paramètres alternatifs qui peuvent être utilisés dans les déclarations. Il souligne l'exemple de syntaxe pour l'utilisation et l'accès à différentes fonctions en vertu Apt.

La commande utilisée pour déclarer aide option sous Apt est illustré ci-dessous
.. code-block:: bash

	cleopatra Apt help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu apt.

.. code-block:: bash

 kevell@corp:/# cleopatra apt help
 ******************************


  This command allows you to modify create or modify apts

  Apt, apt

        - create
        Create a new system apt, overwriting if it exists
        example: cleopatra apt create --aptname="somename"

        - remove
        Remove a system apt
        example: cleopatra apt remove --aptname="somename"

        - set-password
        Set the password of a system apt
        example: cleopatra apt set-password --aptname="somename" --new-password="somepassword"

        - exists
        Check the existence of a apt
        example: cleopatra apt exists --aptname="somename"

        - show-groups
        Show groups to which a apt belongs
        example: cleopatra apt show-groups --aptname="somename"

        - add-to-group
        Add apt to a group
        example: cleopatra apt add-to-group --aptname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove apt from a group
        example: cleopatra apt remove-from-group --aptname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

Différentes caractéristiques d'Apt
-------------------------------------------

Ce sujet traite avec des caractéristiques différentes de apt sous ce module, ainsi que les façons d'utiliser ces différentes fonctions.

Les différents aspects de ce module sous apt est énumérés ci-dessous,

* Créer
* Retirer
* Définir un mot de passe
* existe
* Show-groupes
* Ajouter à groupe
* Remove-de-groupe



CREATE
----------

Cette fonction vise à créer un nouveau système apt, et ainsi que écrase en cas de déjà existant. Cette fonction d'apt utilisant ce module peut être réalisé par la syntaxe suivante,

.. code-block:: bash

	cleopatra apt create --aptname="somename"

A la place de aptname l'utilisateur peut spécifier le nom de l'appartement qui doit être créé. Après avoir saisi la commande comme indiqué ci-dessus, le nouveau système apt sera créé avec le nom spécifié.

RETIRER
-----------

Cette fonction vise à supprimer un apt existant. Cette fonction d'apt utilisant ce module peut être réalisé par la syntaxe suivante,
.. code-block:: bash

	cleopatra apt remove --aptname="somename"

A la place de aptname l'utilisateur peut spécifier le nom de l'appartement qui est à supprimer. Après avoir saisi la commande comme indiqué ci-dessus, l'apt spécifié seront supprimés.

MOT DE PASSE SET
-------------------------

Cette fonction facilite la fixation d'un nouveau mot de passe à un système apt selon les exigences. Ceci peut être réalisé par application de la commande en tant que donnée
ci-dessous,
.. code-block:: bash

	cleopatra apt set-password --aptname="somename" --new-password="somepassword"

Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les deux champs,

* Nom Apt
* Nouveau mot de passe

Après avoir spécifié les deux champs dans le format de commande mentionné ci-dessus, le nouveau mot de passe pour l'apt spécifiée sera créé.


EXISTS
--------

Cette fonction vise à vérifier l'existence d'un apt. Cela peut être fait simplement, en utilisant la commande ci-dessous,

.. code-block:: bash

	cleopatra apt exists --aptname="somename"

Après l'application de la commande comme ci-dessus, l'existence d'un apt mentionné sera assurée avec les résultats.

Afficher les groupes
----------------------------

Cette fonction aide les utilisateurs de connaître à quel groupe ne l'appartement appartient. Ceci peut être réalisé simplement en utilisant la commande ci-dessous,

.. code-block:: bash

	cleopatra apt show-groups --aptname="somename"

L'utilisateur doit indiquer le nom de l'appartement dans le domaine de aptname, afin de connaître les détails de son groupe.

AJOUTER _TO_GROUP
-------------------------------

L'objectif principal de cette fonction est d'ajouter le nécessaire apte à le groupe requis en appliquant simplement la commande comme indiqué ci-dessous,

.. code-block:: bash

	cleopatra apt add-to-group --aptname="somename" --groupname="somegroupname"

Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les deux domaines suivants selon leurs besoins dans le format de commande ci-dessus mentionné,

* Aptname
* Nom de groupe

REMOVE_FROM_GROUP
-------------------------------------

L'objectif principal de cette fonction est de supprimer l'appartement d'un groupe en appliquant simplement la commande comme indiqué ci-dessous,

.. code-block:: bash

	cleopatra apt remove-from-group --aptname="somename" --groupname="somegroupname"

Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les deux domaines suivants selon leurs besoins dans le format de commande ci-dessus mentionné,

* Aptname
* Nom de groupe


Autres paramètres
-----------------------------

Les autres paramètres de ce module, chacun pouvant être utilisés dans la déclaration est,

* Apt
* apt


avantages
---------------

* Les paramètres utilisés déclarant aide et d'autres caractéristiques différentes de apt ne sont pas sensibles à la casse.
* Il est bien de choses à faire dans les deux cents os et ainsi que dans Ubuntu.
* L'utilisation de ce module, l'utilisateur peut créer et modifier ainsi que l'appartement selon leurs besoins.
* L'existence d'un apt peut être assuré dans ce module.


