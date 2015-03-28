=======
SFTP
=======

synopsis
---------

           ThisModule aider à dossiers d'anneau de transfert d'un système à l'autre. Il peut télécharger ou de télécharger les fichiers sur le système. L'automatisation est possible. PUT et GET options sont disponibles dans ce module. Il spécifie la configuration de votre environnement. Il est amical avec Ubuntu et OS cent utilisateur.

commande Aide
-------------

Aide commande utilisée pour trouver des informations sur une commande spécifique. Pour plus d'informations sur les changements de fonctions sur cette page de SFTP nous pouvons utiliser cette commande d'aide.

.. code-block:: bash

 		ptconfigure sftp help


La capture d'écran suivante vous guidera.

.. code-block:: bash


 kevell@corp:/# ptconfigure sftp help
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



installation
-------------

En tant que société, et en tant que particuliers fortunés, SFTP a été consacrée à répondre aux défis technologiques de chaque Partnera € ™, se acquitter de leurs exigences techniques, et de satisfaire leurs objectifs d'affaires. Ce est un processus évident pour installer le module de SFTP sous ptconfigure en utilisant simplement la commande ci-dessous givenName,

.. code-block:: bash

		ptconfigure SFTP put


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter local source file path
 /home/kevells/Desktop/graphs
 Enter remote target file path
 /home/murali/Desktop/graphs
 [Pharaoh Logging] Opening SFTP Connections...
 [192.168.1.4]Connection failure. Will not execute commands on this box..
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************



 SFTP Put: Success

 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash



 kevell@corp:/# ptconfigure sftp get

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter remote source file path
 /home/murali/Desktop/graphs
 Enter local target file path
 /hoem/kevells/Desktop/graphs1
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] [192.168.1.4] Executing SFTP Get...
 [Pharaoh Logging] No SFTP Object
 [Pharaoh Logging] 
 [Pharaoh Logging] [192.168.1.4] SFTP Get Completed...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************





Options
----------

.. cssclass:: table-bordered


 +--------------------+------------------------+----------------------------------------------------------------+
 | paramètre          | paramètres alternatifs | commentaires                                                   |
 +====================+========================+================================================================+
 |put                 | SFTP, sftp             | Source et la cible- Peut transférer le fichier                 |
 +--------------------+------------------------+----------------------------------------------------------------+
 |get                 | SFTP, sftp             | Chemin d'accès à la source -Le fichier peut être téléchargé à  |
 |                    |                        | Partir du système distant|                                     |
 +--------------------+------------------------+----------------------------------------------------------------+
 

avantages
-------------

* Multi Server de région éloignée.
* Le fichier spécifié ne est pas message d'erreur disponibles viendra.
* Accès Capacité est difficile sans autorisation.
* Écraser automatiquement en cas de déjà en cas de fichier exister.
* Non sensible à la casse.
* Le secret et la sécurité est possible.

Résolution clients problèmes technologiques les plus difficiles et permettant Leur succès est la mission de SFTP et la passion.

