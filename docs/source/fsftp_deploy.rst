======
SFTP
======



synopsis
--------------

   Ce module aider à transférer des fichiers d'un système à un autre. Il peut télécharger ou de télécharger les fichiers sur le système. L'automatisation est possible. PUT et GET options sont disponibles dans ce module. Il spécifie la configuration de votre environnement. Il est amical avec Ubuntu et cent OS utilisateur.

Commande Aide
-----------------------

Aide commande utilisée pour trouver des informations sur une commande spécifique. Pour plus d'informations sur les changements à la fonctionnalité des SFTP nous pouvons utiliser cette commande d'aide.

.. code-block:: bash
   
	        ptdeploy SFTP help


La capture d'écran suivante vous guide.

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp help
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
-----------------

En tant que société, et en tant qu'individus, SFTP a été consacrée à répondre aux défis technologiques de chaque partenaire, se acquitter de leurs exigences techniques, et de satisfaire leurs objectifs d'affaires. Ce est un processus évident pour installer le module de SFTP sous ptdeploy en utilisant simplement la commande ci-dessous,

.. code-block:: bash
  
		ptdeploy SFTP  install 


Après avoir donné la commande alors le système se poser la question,

Install SFTP server group? Y/N

Si l'entrée de l'utilisateur en tant que Y, puis

SSh timeout section?

L'utilisateur doit entrer la valeur

Se il vous plaît entrer dans le port de ssh à distance

La valeur par défaut est 22. L'utilisateur peut entrer ne importe quelle valeur

Enter server host IP?

L'utilisateur doit entrer le nom d'utilisateur, mot de passe, et le chemin clé.

Ajouter un autre serveur?

Si l'entrée de l'utilisateur comme Y il doit entrer un nouveau nom de serveur

Alors tout sera connecté.

Si l'entrée de l'utilisateur comme N nom de serveur précédente peut être consultée.

.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put
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



 SFTP Put: Success

 ------------------------------
 Installer Finished
 ******************************


Options
------------


.. cssclass:: table-bordered

 
 +-------------+------------------------+----------------------+----------------------------------------------+
 | Paramètres  | Autres paramètres      | syntaxe              | Commentaires                                 |
 +=============+========================+======================+==============================================+
 |put          | SFTP, sftp             | Source to target     | Source de cibler -Le fichier peut transférés |
 +-------------+------------------------+----------------------+----------------------------------------------+
 |get          | SFTP, sftp             | Path to source       | Chemin d'accès à la source -Le fichier peut  |
 |             |                        |                      | téléchargé à partir du système à distance|   |
 +-------------+------------------------+----------------------+----------------------------------------------+


avantages
----------


* Multi Server de région éloignée.
* Le fichier spécifié ne est pas message d'erreur disponibles viendra.
* Accessability est difficile sans autorisation.
* Écraser automatiquement en cas de déjà en cas de fichier exister.
* Non sensible à la casse.
* Le secret et la sécurité est possible.


 Résolution clients problèmes technologiques les plus difficiles et en favorisant leur réussite est la mission de SFTP et la passion.
