============
Pear
============

Synopsis
-------------

PEAR est l'abréviation de "Extension de PHP et Application Repository" et se prononce comme le fruit. Le but de PEAR est de fournir:

* Une bibliothèque structuré de code open-source pour les utilisateurs PHP
* Un système de distribution de code et l'entretien de l'emballage
* Un style standard pour le code écrit en PHP, spécifié ici
* Le PHP Extension Bibliothèque communautaire (PECL)


La mission de PEAR est de fournir des composants réutilisables, l'innovation plomb en PHP, fournir les meilleures pratiques pour le développement PHP et d'éduquer les développeurs.

Le code de PEAR est divisé en "paquets". Chaque paquet est un projet distinct avec sa propre équipe de développement, numéro de version, cycle de publication, la documentation et une relation définie à d'autres paquets (incluant les dépendances). Paquets sont distribués sous forme de fichiers tar compressé avec un fichier de description à l'intérieur, et installés sur votre système local en utilisant l'installeur PEAR.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de PEAR. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure pear help

La représentation picturale de la commande ci-dessus est listé ci-dessous,

.. code-block:: bash


 kevell@corp:/# ptconfigure pear help
 ******************************


  This command allows you to modify create or modify pears

  Pear, pear

        - create
        Create a new system pear, overwriting if it exists
        example: ptconfigure pear create --pearname="somename"

        - remove
        Remove a system pear
        example: ptconfigure pear remove --pearname="somename"

        - set-password
        Set the password of a system pear
        example: ptconfigure pear set-password --pearname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pear
        example: ptconfigure pear exists --pearname="somename"

        - show-groups
        Show groups to which a pear belongs
        example: ptconfigure pear show-groups --pearname="somename"

        - add-to-group
        Add pear to a group
        example: ptconfigure pear add-to-group --pearname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pear from a group
        example: ptconfigure pear remove-from-group --pearname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************



créer
------------


Lorsque l'utilisateur a besoin de créer un nouveau système de poire ou doit remplacer l'existant, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
	ptconfigure pear create - -pearname=”somename”

supprimer
------------

Lorsque l'utilisateur doit supprimer une poire du système, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

	ptconfigure pear remove - -pearname=”somename”

Définir mot de passe
---------------------

Lorsque l'utilisateur doit définir un mot de passe d'une poire du système, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
	ptconfigure pear setpassword - -pearname=”somename”- - new-password=”somepassword”

existe
---------------------

Lorsque l'utilisateur a besoin de connaître l'existence de la poire, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
	ptconfigure pear exists - -pearname=”somename”

Afficher les groupes
---------------------

Lorsque l'utilisateur doit connaître le groupe auquel appartient une poire, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
	ptconfigure pear show-groups - -pearname=”somename”

Ajouter au groupe
---------------------

Lorsque l'utilisateur doit allouer poire à un groupe particulier, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
 	ptconfigure pear add-to-group - -pearname=”somename” - - groupname=”somegroupname”


Retirer du groupe
----------------------------

Lorsque l'utilisateur doit supprimer la poire d'un groupe, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
 		ptconfigure pear remove-from-group - -pearname=”name” - -groupname=”groupname”


Alternative Paramètre
----------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande.

Pear, pear

.. code-block:: bash

 Eg: ptconfigure pear create - -pearname=”somename”/ ptconfigure Pear create - -pearname=”somename”

avantages
--------------
 
Pear.php.net fournit à la fois un homme de l'environnement (HTML) et facile à la machine (actuellement REST) interface pour les forfaits disponibles à partir pear.php.net. Toute communication se produit via le protocole HTTP. Autres fonctions du site pear.php.net offre sont:


* La gestion de compte d'utilisateur (indépendant du serveur SVN)
* Gestion des paquets
* Gestion des versions
* Well-to-do dans Ubuntu et Cent OS
* Sensibilité non de cas
