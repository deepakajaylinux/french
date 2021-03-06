============
Chmode
============

synopsis
-------------

Fichiers et répertoires appartiennent à la fois propriétaire et un groupe. Un groupe est généralement constitué d'un ensemble d'utilisateurs, tous appartenant à un même groupe. La première série de trois est la lecture, d'écriture et d'exécution pour le propriétaire du fichier.

chmod est utilisé pour changer les permissions des fichiers ou des répertoires. Sur les autres systèmes d'exploitation de type Unix Linux et, il ya un ensemble de règles pour chaque fichier qui définit qui peut accéder à ce fichier, et comment ils peuvent y accéder. Ces règles sont appelées autorisations de fichiers ou des modes de fichiers. Le nom de la commande chmod signifie "changement de mode", et il est utilisé pour définir la façon dont un fichier peut être consulté.

Il ya trois classes générales des utilisateurs:

* L'utilisateur qui possède le fichier ("Utilisateur")
* Les utilisateurs appartenant au groupe de propriété définie du fichier («Groupe»)
* Tout le monde («Autres»)


À son tour, pour chacune de ces catégories d'utilisateurs, il ya trois types d'accès de fichier:

* La capacité de regarder le contenu du fichier ("Read")
* La possibilité de changer le contenu du fichier ("Write")
* La possibilité d'exécuter le contenu du fichier comme un programme sur le système ("Execute")

Pour chacune des trois catégories d'utilisateurs, il existe trois types d'accès.

.. cssclass:: table-bordered

 +----------------+----------------------------------------------------------------------+
 | symbols        | Signification                                                        |
 +================+======================================================================+
 |rwx             | le propriétaire du fichier peut lire, écrire ou exécuter ce fichier  |
 |                | comme un processus sur le système.                                   |
 +----------------+----------------------------------------------------------------------+
 |r-x             | ne importe qui dans le groupe du fichier peut lire ou exécuter ce    |
 |                | fichier, mais pas écrire                                             |
 +----------------+----------------------------------------------------------------------+
 |r–              | ne importe qui peut lire ce fichier, mais pas y écrire ou exécuter   |
 |                | son contenu comme un processus.|                                     |
 +----------------+----------------------------------------------------------------------+



Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de changement module de mode. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure Chmod help

La représentation picturale de la commande ci-dessus est listé ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure Chmod help
 ******************************


  This command handles file permission functions.

  Chmod, chmod

        - path
        Will change the file permission mode of a path
        example: ptconfigure chmod path --yes --guess --recursive --path=/a/file/path --mode=0777


 ------------------------------
 End Help
 ******************************

chemin
-----------

Chemin chmod est la commande qui modifient les autorisations d'accès pour déposer les objets du système (fichiers et répertoires).

Le nombre 1, 2 et 4 représente exécuter, écrire et lire. Ces numéros sont utilisés parce que toute combinaison de ces trois numéros seront
être unique.

Lorsque l'utilisateur a besoin de changer le mode de fichier, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
        
	        ptconfigure chmod path –yes –guess –recursive –path=/”File path” –mode=0777

Alternative Paramètre
--------------------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande.

chmod, Chmod

Par exemple: chemin de chmod ptconfigure CHMODE chemin / ptconfigure


avantages
--------------


chmod modifie les permissions du fichier spécifié par nom de fichier pour les autorisations spécifiées par les autorisations. Permission        définit les autorisations pour le propriétaire du fichier («l'utilisateur»), les membres du groupe qui possède le fichier (le «groupe»), et     toute autre personne («autres»). Il existe deux manières de représenter ces autorisations: avec des symboles (caractères alphanumériques), ou avec des chiffres en octal (les chiffres de 0 à 7).

