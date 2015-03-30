=============
Run Command
=============

synopsis
-----------

Les modules de commande RUN permet aux utilisateurs d'exécuter des commandes du système d'exploitation. Ce est principalement être utilisé dans sur le pilote automatique. Grâce à cette commande, l'utilisateur peut spécifier exécuter la ligne de commande, le nom de l'utilisateur et donc d'exécuter le soit en arrière-plan ou front-end. Voyons les utilisations de commande de marche.

HelpCommand
----------------

La commande d'aide décrit les utilisations de commande de marche, ses principales fonctions à ce sujet, ses autres paramètres, les commandes utilisées pour exécuter une commande, et donc sur la syntaxe pour la spécification de la commande, le nom de l'utilisateur et donc d'exécuter l'une ou l'autre en arrière-plan ou l'avant -fin. La syntaxe utilisée pour déclarer la commande d'aide est indiqué ci-dessous.

.. code-block:: bash

		ptconfigure RunCommand help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptconfigure RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************


La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered

 
 +-----------------------+---------------------------------------------------+------------------------------------------------------+
 | paramètre             | fonction                                          | utilisation                                          |
 +=======================+===================================================+======================================================+
 |command=”ls -lah /tmp” | Il permet à l'utilisateur de spécifier la         | En utilisant ce, l'utilisateur peut spécifier        |
 |                       | commande et de son but.                           | leur propre instruction en fonction de leurs         |
 |                       |                                                   | exigences.                                           |
 +-----------------------+---------------------------------------------------+------------------------------------------------------+
 |run-as-user=”ubuntu”   | En utilisant ce, l'utilisateur peut spécifier le  | En utilisant ce, l'utilisateur peut spécifier        |
 |                       | nom de l'utilisateur.                             | l'enregistrement de l'utilisateur requis selon       |
 |                       |                                                   | leurs besoins.                                       |
 +-----------------------+---------------------------------------------------+------------------------------------------------------+
 |En utilisant ce,       | Il permet à l'utilisateur de spécifier l'endroit  | En utilisant ce, l'utilisateur peut spécifier la     |
 |l'utilisateur peut     | où la commande spécifique soit dans le fond ou    | plate-forme de leur utilisation en fonction de       |
 |spécifier la plate-    | dans le front-end terme.                          | leurs exigences.                                     |
 |forme de leur          |                                                   |                                                      |
 |utilisation en         |                                                   |                                                      |
 |fonction de leurs      |                                                   |                                                      |
 |besoins, "-background| |                                                   |                                                      |
 +-----------------------+---------------------------------------------------+------------------------------------------------------+


.. code-block:: bash


 kevell@corp:/# ptconfigure run-command install --yes --command="ls -lah /tmp" --run-as-user="kevells" --background

 *******************************
 *        Pharaoh Tools        *
 *         Run Command        *
 *******************************
 Use NoHup?: (Y/N) 
 y
 cd /home/kevells
 su kevells -c ls -lah /tmp
 nohup ls -lah /tmp &
 exit
 Creating /tmp/ptconfigure-temp-script-11430033105.sh
 chmod 755 /tmp/ptconfigure-temp-script-11430033105.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-11430033105.sh Permissions
 Executing /tmp/ptconfigure-temp-script-11430033105.sh
 su: invalid option -- 'a'
 Usage: su [options] [LOGIN] 

 Options:
  -c, --command COMMAND         pass COMMAND to the invoked shell
  -h, --help                    display this help message and exit
  -, -l, --login                make the shell a login shell
  -m, -p,
  --preserve-environment        do not reset environment variables, and
                                keep the same shell
  -s, --shell SHELL             use SHELL instead of the default in passwd

 nohup: redirecting stderr to stdout
 total 17M
 drwxrwxrwt  9 root          root          4.0K Mar 30 20:05 .
 drwxr-xr-x 28 root          root          4.0K Mar 28 17:58 ..
 -rwxr-xr-x  1 root          root           229 Mar 30 10:39 ptconfigure-temp-script-10148944050.sh
 -rwxr-xr-x  1 root          root           155 Mar 30 12:52 ptconfigure-temp-script-1093307841.sh
 -rwxr-xr-x  1 root          root            68 Mar 30 20:05 ptconfigure-temp-script-11430033105.sh
 -rwxr-xr-x  1 root          root           146 Mar 30 15:46 ptconfigure-temp-script-29072719650.sh
 -rwxr-xr-x  1 root          root           261 Mar 30 14:30 ptconfigure-temp-script-39464139952.sh
 -rwxr-xr-x  1 root          root           155 Mar 30 14:03 ptconfigure-temp-script-4842774525.sh
 -rwxr-xr-x  1 root          root            64 Mar 30 19:04 ptconfigure-temp-script-64533089928.sh
 -rwxr-xr-x  1 root          root           229 Mar 30 14:00 ptconfigure-temp-script-78930437679.sh
 -rwxr-xr-x  1 root          root           146 Mar 30 14:03 ptconfigure-temp-script-81890547014.sh
 -rw-r--r--  1 root          root            65 Mar 30 09:53 cxtracker.start.log
 drwxr-xr-x  2 elasticsearch elasticsearch 4.0K Mar 30 09:54 elasticsearch
 drwxr-xr-x  2 elasticsearch elasticsearch 4.0K Mar 30 09:54 hsperfdata_elasticsearch
 drwxr-xr-x  2 root          root          4.0K Mar 30 09:53 hsperfdata_root
 drwxr-xr-x  2 tomcat7       tomcat7       4.0K Mar 30 09:54 hsperfdata_tomcat7
 drwxrwxrwt  2 root          root          4.0K Mar 30 09:54 .ICE-unix
 srwxrwxrwx  1 mongodb       nogroup          0 Mar 30 09:53 mongodb-27017.sock
 -rw-r--r--  1 root          root           15M Mar 13  2014 mysql-server-wsrep-5.6.16-25.5-amd64.deb
 -rw-r--r--  1 root          root          668K Mar 30 14:03 netbeans-8.0-linux.sh
 -rw-r--r--  1 root          root           85K Mar 30 14:03 netbeans-8.0-linux.sh.1
 -rw-r--r--  1 root          root          1.1M Mar 30 15:46 netbeans-8.0-linux.sh.2
 srwxrwxr-x  1 kevells        kevells           0 Mar 30 09:57 qtsingleapp-hipcha-2c5e-3e8
 -rw-rw-r--  1 kevells        kevells           0 Mar 30 09:57 qtsingleapp-hipcha-2c5e-3e8-lockfile
 drwxr-xr-x  2 tomcat7       root          4.0K Mar 30 09:54 tomcat7-tomcat7-tmp
 -r--r--r--  1 root          root            11 Mar 30 09:53 .X0-lock
 drwxrwxrwt  2 root          root          4.0K Mar 30 09:53 .X11-unix
 Temp File /tmp/ptconfigure-temp-script-11430033105.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 RunCommand: Success
 ------------------------------
 Installer Finished
 ******************************


paramètres alternatifs
----------------------

nous pouvons utiliser les paramètres suivants,

RunCommand, runcommand, run-command


avantages
------------

* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire dans les deux Cent OS et ainsi que dans Ubuntu.
* Les utilisateurs peuvent spécifier la commande, le nom de l'utilisateur et donc d'exécuter l'une ou l'autre en arrière-plan ou front-end.
* La commande help guide les utilisateurs à la façon d'exécuter la commande de marche sur de sorte que son effet.
