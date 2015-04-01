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

        - install
        Install
        example: ptconfigure pear pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure pear pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure pear pkg-ensure --package-name="somename"
        
 ------------------------------
 End Help


Install
----------

Lorsque l'utilisateur devez installer une poire , la commande ci-dessous donnée exécuter le processus .


.. code-block:: bash

	ptconfigure pear pkg-install --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-install --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************



Remove
------------

Lorsque l'utilisateur doit supprimer une poire du système , la commande ci-dessous donnée exécuter le processus .


.. code-block:: bash

	ptconfigure pear pkg-remove --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-remove --package-name="file"
 pear/File (version >= 1.4.0) is required by installed package "pear/File_CSV"
 pear/File (version >= 1.4.0) is required by installed package "pear/File_Util"
 pear/File cannot be uninstalled, other installed packages depend on this package
 [Pharaoh Logging] Removing Package file from the Packager Pear did not execute correctly
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Failure

 ------------------------------
 Pear Mods Finished
 ******************************



Ensure
---------

Lorsque l'utilisateur a besoin pour assurer une poire , la commande ci-dessous donnée exécuter le processus .


.. code-block:: bash

	ptconfigure pear pkg-ensure --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-ensure --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************






Alternative Paramètre
----------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande.

Pear, pear


avantages
--------------
 
Pear.php.net fournit à la fois un homme de l'environnement (HTML) et facile à la machine (actuellement REST) interface pour les forfaits disponibles à partir pear.php.net. Toute communication se produit via le protocole HTTP. Autres fonctions du site pear.php.net offre sont:


* La gestion de compte d'utilisateur (indépendant du serveur SVN)
* Gestion des paquets
* Gestion des versions
* Well-to-do dans Ubuntu et Cent OS
* Sensibilité non de cas
