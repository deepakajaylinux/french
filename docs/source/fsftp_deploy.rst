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


 kevell@corp:/# ptdeploy sftp put 

 SFTP on Server group? (Y/N) 
 y 
 Please Enter SSH Timeout in seconds 
 20 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 Enter local source file path 
 /home/karunakaran/Desktop/server.odt 
 Enter remote target file path 
 /home/karthik/Desktop/server.odt 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 

 SFTP Put: Success 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 


.. code-block:: bash

 kevell@corp:/# ptdeploy sftp put --yes --environment-name=karthik --source="/tmp/kk.txt" --target="/tmp/kk.txt" 

 Please Enter SSH Timeout in seconds 
 20 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 
 
 SFTP Put: Success 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash



 kevell@corp:/# ptdeploy sftp put --yes --source="/home/karunakaran/Desktop/readme.txt" --target="/home/karthik/Desktop/readme.txt" 

 Please Enter SSH Timeout in seconds 
 20 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 

 SFTP Put: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp get 

 SFTP on Server group? (Y/N) 
 y 
 Please Enter SSH Timeout in seconds 
 200 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 Enter remote source file path 
 /tmp/testing 
 Enter local target file path 
 /opt/testr 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 

 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp get --yes --environment-name=karthik --source="/tmp/testing" --target="/opt/testr" 

 Please Enter SSH Timeout in seconds 
 200 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 
 
 Shell Result: Success 
 SFTP Get 

 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp get --yes --source="/tmp/testing" --target="/opt/testr" 

 Please Enter SSH Timeout in seconds 
 200 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 
 
 Shell Result: Success 
 SFTP Get 
 
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
