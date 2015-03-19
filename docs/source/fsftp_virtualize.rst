=======
SFTP
=======


Synopsis
-------------

Ce module aider à transférer des fichiers d'un système à l'autre. Il peut charger ou télécharger les fichiers sur le système. L'automatisation est possible. Mettre et obtenir des options sont disponibles dans ce module. Il gère également la machine virtuelle. Il est facile à utiliser avec Ubuntu et cent OS.

Commande Aide
-------------------------

Commande help permet de rechercher des informations sur une commande spécifique. Pour plus d'informations sur les modifications des fonctionnalités de Secure File Transfer Protocol(SFTP) sous ptvirtualize, l'utilisateur peut utiliser cette commande help.


.. code-block:: bash

	ptvirtualize  sftp help


La capture d'écran suivante vous guide.


.. code-block:: bash

 kevell@corp:/# ptvirtualize sftp help

 ******************************
 Pharaoh Tools - ptvirtualize
 ******************************


  This command handles SFTP Transfer Functions.

  SFTP, sftp

        - put
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure sftp put
        example: ptconfigure sftp put --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp put --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

        - get
        Will ask you for details for servers, then copy a file or directory from remote to local
        example: ptconfigure sftp get
        example: ptconfigure sftp get --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp get --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

 ------------------------------
 End Help
 ******************************


Alternative Paramètre
---------------------------------

Il existe deux autres paramètres sont disponibles. Ils sont SFTP et sftp. Au lieu d'utiliser sftp, l'utilisateur peut utiliser SFTP.



Put
------

Le transfert de fichiers peut être fait du niveau local à un serveur distant. Cette option de vente demande la datails de l'utilisateur pour les serveurs. La commande suivante utilisée pour l'option de vente.



.. code-block:: bash

	ptvirtualize  sftp put – yes –source=”/tmp/file” – target=”/home/user/file”

La capture d'écran suivante indique l'utilisation de cette commande.

.. code-block:: bash

 kevell@corp:ptconfigure sftp put
 
 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds
 90
 Please Enter remote SSH Port
 22
 Use Environments Configured in Project? (Y/N) 
 N
 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter local source file path
 /root/vv
 Enter remote target file path
 /root/gg/vv
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************


SFTP on server group? Y/N

Si les entrées d'utilisateur en tant qu'Y puis

SSh timeout section?

L'utilisateur doit entrer la valeur


S'il vous plaît entrez distance ssh port


Valeur par défaut est de 22. L'utilisateur peut entrer n'importe quelle valeur


Enter environments configured in project? (Y/N)

L'utilisateur doit entrer y puis il commence le chargement.


Enter local source file path?

L'utilisateur doit entrer le chemin d'accès du fichier


Alors tout sera connecté.

Si l'utilisateur a entré comme N, il peut être résilié.




Get
-------

Transfert de fichiers peut être fait à distance au serveur local. Il demande à l'utilisateur d'entrer dans le groupe de serveurs. La commande suivante utilisée pour obtenir option.


.. code-block:: bash

	ptvirtualize  sftp get – yes –source=”/tmp/file” – target=”/home/user/file”

Il explique la capture d'écran suivante.



.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds

 Please Enter remote SSH Port

 Use Environments Configured in Project? (Y/N) 

 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter remote source file path

 Enter local target file path

 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************


SFTP on server group? Y/N

Si les entrées d'utilisateur en tant qu'Y puis


SSh timeout section?

L'utilisateur doit entrer la valeur


S'il vous plaît entrez distance ssh port


Valeur par défaut est de 22. L'utilisateur peut entrer n'importe quelle valeur


Enter environments configured in project? (Y/N)

L'utilisateur doit entrer y puis il commence le chargement.


Enter local target file path?

L'utilisateur doit entrer le chemin d'accès du fichier local cible


Alors tout sera connecté.

Si l'utilisateur a entré comme N, il peut être résilié. Les captures d'écran ci-dessous montre sa fonction.



.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 N
 ******************************


 Shell Result: Failure
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************



options
-------------

.. cssclass:: table-bordered

 +------------------------+---------------------------+--------------------------------------------------------------+
 | paramètres		  | paramètres alternatifs    | commentaires						     |
 +========================+===========================+==============================================================+
 |put			  | SFTP, sftp        	      | Source de cibler -Le fichier peut transférés  		     |
 +------------------------+---------------------------+--------------------------------------------------------------+
 |get			  | SFTP, sftp                | Chemin d'accès à la source -Le fichier peut téléchargé       |
 |                        |                           | à partir de système distant|                                 |
 +------------------------+---------------------------+--------------------------------------------------------------+



avantages
-------------

* Multi serveur de domaine distant. 
* Fichier spécifié n'est pas disponible erreur message viendra. 
* Accessability est difficile sans permission. 
* Automatiquement remplacer en cas de déjà en cas de fichier existent. 
* Non casse. 
* Secret et la sécurité est possible.

