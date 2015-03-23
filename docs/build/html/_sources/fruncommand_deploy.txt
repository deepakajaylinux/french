=============
Run Command
=============

synopsis
------------

Les modules de commande RUN permet aux utilisateurs d'exécuter une commande du système d'exploitation. Ce est principalement utilisé dans un pilote automatique. L'utilisation de ce terme commande, l'utilisateur peut spécifier la commande, le nom de l'utilisateur et aussi pour exécuter le soit en arrière-plan ou front-end. Voyons les utilisations de commande de marche.

Commande Aide
---------------------

La commande d'aide décrit les utilisations de commande de marche, sa fonctionnalité majeure, ses autres paramètres, les commandes utilisées pour exécuter une commande, et aussi sur la syntaxe pour spécifier la commande, le nom de l'utilisateur et aussi pour exécuter le soit en arrière-plan ou l'avant -fin. La syntaxe utilisée pour déclarer la commande d'aide est indiqué ci-dessous.

.. code-block:: bash

		ptdeploy RunCommand help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptdeploy RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************


Comment utiliser la commande Exécuter
-------------------------------------------


La syntaxe utilisée pour spécifier l'ordre de marche dans illustré ci-dessous.

.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered


 +------------------------+-------------------------------------------------+--------------------------------------------------------+
 | Parameter              | fonction                                        | usage                                                  |
 +========================+=================================================+========================================================+
 |command=”ls -lah /tmp”  | Il permet à l'utilisateur de spécifier la       | En utilisant ce, l'utilisateur peut spécifier leur     |
 |                        | commande et son but.                            | propre commande selon leurs besoins.                   |
 +------------------------+-------------------------------------------------+--------------------------------------------------------+
 |run-as-user=”ubuntu”    | En utilisant ce que l'utilisateur peut          | En utilisant ce, l'utilisateur peut spécifier leur     |
 |                        | spécifier le nom de l'utilisateur.              | identifiant d'utilisateur requis selon leurs besoins.  |
 +------------------------+-------------------------------------------------+--------------------------------------------------------+
 |” –background           | Il permet à l'utilisateur de spécifier où pour  | En utilisant ce, l'utilisateur peut spécifier la       |
 |                        | exécuter la commande particulière, soit en      | plateforme de leur utilisation selon leurs besoins.    |
 |                        | arrière-plan ou dans le front-end.|             |                                                        |
 +------------------------+-------------------------------------------------+--------------------------------------------------------+



La syntaxe et la table comme décrit ci-dessus peut aide à l'utilisateur comment utiliser la commande de marche.


.. code-block:: bash

 kevell@corp:/# ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background 

 ******************************* 
 *   Golden Contact Computing  * 
 *         Run Command        * 
 ******************************* 
 Use NoHup?: (Y/N) 
 y 
 cd /home/karunakaran 
 su  ubuntu 
 nohup ls -lah /tmp & 
 exit 
 Creating /tmp/ptconfigure-temp-script-56005480696.sh 
 chmod 755 /tmp/ptconfigure-temp-script-56005480696.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-56005480696.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-56005480696.sh 
 No passwd entry for user 'ubuntu' 
 nohup: redirecting stderr to stdout 
 total 92K 
 drwxrwxrwt 10 root        root        4.0K Mar 20 17:06 . 
 drwxr-xr-x 29 root        root        4.0K Mar 20 16:18 .. 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonKEKGVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonMKENVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 10:07 .bamficonN2NXVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonSM8KVX 
 -rwxr-xr-x  1 root        root          58 Mar 20 17:06 ptconfigure-temp-script-56005480696.sh 
 -rw-------  1 karunakaran karunakaran    0 Mar 20 09:50 config-err-UrGst6 
 -rw-------  1 root        root        1000 Mar 20 09:49 .configtest.KiQIacNN 
 -rw-r--r--  1 root        root          33 Mar 20 09:50 cxtracker.start.log 
 drwxr-xr-x  2 root        root        4.0K Mar 20 09:50 hsperfdata_root 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:50 .ICE-unix 
 -rw-r--r--  1 root        root           3 Mar 20 15:40 kk.txt 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 16:58 luh3hawd.tmp 
 srwxrwxrwx  1 mongodb     nogroup        0 Mar 20 09:49 mongodb-27017.sock 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 10:07 .org.chromium.Chromium.VRBmwX 
 srwxrwxr-x  1 karunakaran karunakaran    0 Mar 20 10:06 OSL_PIPE_1000_SingleOfficeIPC_8a32f718ac801a6e525d3030e0878e45 
 -rw-r--r--  1 root        root           0 Mar 20 15:42 papyrusfile 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 14:33 plugtmp 
 drwxr-xr-x  2 root        root        4.0K Mar 20 14:42 ServerBlocktemp 
 -rw-rw-r--  1 karunakaran karunakaran    0 Mar 20 09:50 unity_support_test.0 
 drwxr-xr-x  2 root        root        4.0K Mar 20 13:02 vhosttemp 
 -r--r--r--  1 root        root          11 Mar 20 09:49 .X0-lock 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:49 .X11-unix 
 Temp File /tmp/ptconfigure-temp-script-56005480696.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.gcsoftshop.co.uk for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 

 RunCommand: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 


avantages
------------

* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
* Les utilisateurs peuvent spécifier la commande, le nom de l'utilisateur et aussi pour exécuter le either in background or front-end.
* The help command guides the users in how to execute the run command an also its purpose.

