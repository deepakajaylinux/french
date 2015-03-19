==========
AutoSSH
==========


Synopsis
-----------

Ce module facilite les utilisateurs à autoSSH une boîte ptvirtualize. Autossh est un petit front-end pour SSH qui peut surveiller la connexion, redémarrez le tunnel, si elle tombe ou cesse de répondre.


autossh utilise ssh pour construire une boucle de ssh expéditions (celui du local à distance, de la distance au local), et puis envoie les données qu'il s'attend à revenir d'essai.


Nous verrons les fonctions d'auto ssh dans les rubriques à venir.



Commande Aide
-------------------

La commande help guide les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans le module Auto SSH. Il énumère les paramètres alternatifs de module d'Auto SSH. Il décrit également la syntaxe d'utilisation de la cli, les sftp_put, les commandes de sftp_get. La commande help pour Auto SSH module s'affiche comme ci-dessous.


.. code-block:: bash

	ptvirtualize AutoSSH help


La syntaxe servant à déclarer la commande help n'est pas sensible à la casse qui est un atout supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande aide sous Auto SSH.

.. code-block:: bash


 kevell@corp:/# ptvirtualize AutoSSH help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to autoSSH a ptvirtualize box

  AutoSSH, auto-ssh, autossh, ssh, SSH

        - cli
        Open an SSH Cli to your ptvirtualize Box
        example: ptvirtualize auto-ssh cli --yes --guess

        - sftp-put
        SFTP Put a file on to your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-put --yes --guess --source=/path/to/source --target=/path/to/target

        - sftp-get
        SFTP Get a file from your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-get --yes --guess --source=/path/to/source --target=/path/to/target

 ------------------------------
 End Help
 ******************************


Fonctions de autossh
----------------------

Comme l'illustre la commande help ci-dessus, les fonctions principales de cette auto ssh module comprend

* cli
* sftp_put
* sftp_get


Cli
------

Après activation, ou construire une auto ssh dans l'environnement des utilisateurs, la cli peut être créé qui est utilisée pour ouvrir un SSH indicateur composite avancé pour la zone de ptvirtualize d'utilisateurs à l'aide de la commande suivante :


.. code-block:: bash

	ptvirtualize auto-ssh cli --yes --guess


La cli est utilisée pour l'inscription aux disposition des clients dans un environnement particulier où l'auto ssh est généré.


Sftp_put
-----------

Cette fonction est utilisée pour placer ou déplacer les fichiers requis ou les données de la source à destination d'un environnement particulier où l'auto ssh est généré. Cela peut être fait en utilisant la commande ci-dessous :


.. code-block:: bash

	ptvirtualize auto-ssh sftp-put --yes --guess --source="path/to/source --target=/path/to/target

La commande ci-dessus mettra un fichier dans la boîte de ptvirtualize utilisateurs. La capture d'écran suivante représente visuellement le processus.


Sftp_get
-----------

Cette fonction est utilisée pour l'obtention ou aller chercher les fichiers requis ou les données de la source à destination d'un environnement particulier où l'auto ssh est généré. Cela peut être fait en utilisant la commande ci-dessous :


.. code-block:: bash

	ptvirtualize auto-ssh sftp-get --yes --guess --source="path/to/source --target=/path/to/target

La commande ci-dessus va Obtient ou reçoit un fichier de la boîte de ptvirtualize utilisateurs. La capture d'écran suivante représente visuellement le processus.


Alternative Paramètre
-----------------------------

* AutoSSH
* auto-ssh
* autossh
* ssh
* SSH

Dans la liste ci-dessus, aucun des paramètres alternatifs peut être utilisé dans la déclaration.

Avantages
-----------

* Les paramètres utilisés dans l'aide et les opérations d'installation installation et les Nations Unies ne sont pas sensibles à la casse qui
  est un atout supplémentaire alors que par rapport aux autres. 
* Il est aisée dans les deux Ubuntu ainsi que comme OS Cent. 
* La liste de fonctions cli découpes aux disposition des clients dans un environnement particulier aide auto SSH. 
* Sftp_put, Sftp_get Placez et extraire les fichiers respectivement entre source et destination d'un environnement particulier en utilisant 
  autoSSH. 
* La syntaxe servant à déclarer le cli, mettre, get sont clairement décrits dans la commande help.


