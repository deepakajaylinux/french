======================
MysqlServerGalera
======================

synopsis
------------------

Galera Cluster est un cluster de base de données multi-maître synchrone, sur la base de la réplication synchrone et MySQL / Oracle de InnoDB . Lorsque Galera Cluster est en cours d'utilisation , vous pouvez diriger lit et écrit sur ne importe quel nœud , et vous pouvez perdre tout noeud individuel sans interruption dans les opérations et sans la nécessité de gérer les procédures de basculement complexes . Galera Cluster est une solution de haute disponibilité facile à utiliser , qui fournit une disponibilité élevée du système , sans perte de données et d'évolutivité pour la croissance future .


Commande Aide
-----------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de mysqlservergalera . Il énumère les autres paramètres du module de mysqlservergalera . Il décrit également la syntaxe pour l'installation du module de mysqlgqlera . La commande d'aide pour le module de mysqlservergalera est représentée ci-dessous .

.. code-block:: bash

	ptconfigure MysqlServerGalera help

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure MysqlServerGalera help
 ******************************


  This command allows you to install the MySQL Server Galera version.

  MysqlServerGalera, mysql-server-galera, mysqlservergalera

        - install
        Install the Galera Cluster compatible version of Mysql Server
        example: ptconfigure mysql-server-galera install

        - config-galera-starter
        Configure the wsrep.cnf file for a cluster starter
        example: ptconfigure mysql-server-galera config-galera-starter

        - config-galera-joiner
        Configure the wsrep.cnf file for a cluster joiner
        example: ptconfigure mysql-server-galera config-galera-joiner


  Notes, during mysql install a root password will be set. First, it'll look for the parameter --mysql-root-pass, if
  this is not set, it'll look in the ptconfigure config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure.

 ------------------------------
 End Help
 ******************************


installation
--------------

La commande utilisée pour l'installation du module de docker sur le terminal est listé ci-dessous ,

.. code-block:: bash

	ptconfigure mysql-server-galera install

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash



 kevell@corp:/# ptconfigure mysql-server-galera install

 Install MySQL Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Server!        *
 *******************************
 [Pharaoh Logging] Not removing Package mysql-server, it's required by these Modules: PHPVM, Memcached
 Creating /tmp/ptconfigure-temp-script-387244026.sh
 chmod 755 /tmp/ptconfigure-temp-script-387244026.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-387244026.sh Permissions
 Executing /tmp/ptconfigure-temp-script-387244026.sh
 --2015-03-30 16:05:52--  https://launchpad.net/codership-mysql/5.6/5.6.16-25.5/+download/mysql-server-wsrep-5.6.16-25.5-amd64.deb
 Resolving launchpad.net (launchpad.net)... 91.189.89.223, 91.189.89.222
 Connecting to launchpad.net (launchpad.net)|91.189.89.223|:443... connected.
 HTTP request sent, awaiting response... 302 Moved Temporarily
 Location: https://launchpadlibrarian.net/169360930/mysql-server-wsrep-5.6.16-25.5-amd64.deb [following]
 --2015-03-30 16:05:53--  https://launchpadlibrarian.net/169360930/mysql-server-wsrep-5.6.16-25.5-amd64.deb
 Resolving launchpadlibrarian.net (launchpadlibrarian.net)... 91.189.89.229, 91.189.89.228
 Connecting to launchpadlibrarian.net (launchpadlibrarian.net)|91.189.89.229|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 15652198 (15M) [application/x-debian-package]
 Saving to: â€˜mysql-server-wsrep-5.6.16-25.5-amd64.debâ€™

 30% [===========================>                                                                 ] 48,04,576   --.-K/s   in 4m 14s  

 2015-03-30 16:10:09 (18.5 KB/s) - Connection closed at byte 4804576. Retrying.

 --2015-03-30 16:10:10--  (try: 2)  https://launchpadlibrarian.net/169360930/mysql-server-wsrep-5.6.16-25.5-amd64.deb
 Connecting to launchpadlibrarian.net (launchpadlibrarian.net)|91.189.89.229|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 15652198 (15M) [application/x-debian-package]
 Saving to: â€˜mysql-server-wsrep-5.6.16-25.5-amd64.debâ€™

 21% [===================>                                                                         ] 34,00,856   63.0KB/s   in 2m 48s 

 2015-03-30 16:13:01 (19.8 KB/s) - Connection closed at byte 4804576. Retrying.

 --2015-03-30 16:13:03--  (try: 3)  https://launchpadlibrarian.net/169360930/mysql-server-wsrep-5.6.16-25.5-amd64.deb
 Connecting to launchpadlibrarian.net (launchpadlibrarian.net)|91.189.89.229|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 15652198 (15M) [application/x-debian-package]
 Saving to: â€˜mysql-server-wsrep-5.6.16-25.5-amd64.debâ€™

 100%[============================================================================================>] 1,56,52,198 29.0KB/s   in 8m 38s 

 2015-03-30 16:21:42 (29.5 KB/s) - â€˜mysql-server-wsrep-5.6.16-25.5-amd64.debâ€™ saved [15652198/15652198]

 dpkg: error processing archive mysql-server-wsrep-5.6.16-25.5-amd64.deb (--install):
 trying to overwrite '/usr/sbin/mysqld', which is also in package mysql-server-core-5.5 5.5.41-0ubuntu0.14.04.1
 dpkg-deb (subprocess): decompressing archive member: internal gzip write error: Broken pipe
 dpkg-deb: error: subprocess <decompress> returned error exit status 2
 dpkg-deb (subprocess): cannot copy archive member from 'mysql-server-wsrep-5.6.16-25.5-amd64.deb' to decompressor pipe: failed to write     
 (Broken pipe)
 Errors were encountered while processing:
 mysql-server-wsrep-5.6.16-25.5-amd64.deb
 Selecting previously unselected package mysql-server-wsrep.
 (Reading database ... 233400 files and directories currently installed.)
 Preparing to unpack mysql-server-wsrep-5.6.16-25.5-amd64.deb ...
 Unpacking mysql-server-wsrep (5.6.16-25.5) ...
 Replacing files in old package mysql-server-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Reading package lists...
 Building dependency tree...
 Reading state information...
 0 upgraded, 0 newly installed, 0 to remove and 250 not upgraded.
 Temp File /tmp/ptconfigure-temp-script-387244026.sh Removed
 Creating /tmp/ptconfigure-temp-script-69617254643.sh
 chmod 755 /tmp/ptconfigure-temp-script-69617254643.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-69617254643.sh Permissions
 Executing /tmp/ptconfigure-temp-script-69617254643.sh
 /usr/bin/mysqladmin: connect to server at 'localhost' failed
 error: 'Access denied for user 'root'@'localhost' (using password: NO)'
 /tmp/ptconfigure-temp-script-69617254643.sh: 4: /tmp/ptconfigure-temp-script-69617254643.sh: password: not found
 150330 16:21:54 [Warning] Using unique option prefix key_buffer instead of key_buffer_size is deprecated and will be removed in a future 
 release. Please use the full name instead.  

 /usr/bin/mysqladmin  Ver 8.42 Distrib 5.5.41, for debian-linux-gnu on x86_64
 Copyright (c) 2000, 2014, Oracle and/or its affiliates. All rights reserved.

 Oracle is a registered trademark of Oracle Corporation and/or its
 affiliates. Other names may be trademarks of their respective
 owners.
 
 Administration program for the mysqld daemon.
 Usage: /usr/bin/mysqladmin [OPTIONS] command command....
  -c, --count=#       Number of iterations to make. This works with -i
                      (--sleep) only.
  --debug-check       Check memory and open file usage at exit.
  --debug-info        Print some debug info at exit.
  -f, --force         Don't ask for confirmation on drop database; with
                      multiple commands, continue even if an error occurs.
  -C, --compress      Use compression in server/client protocol.
  --character-sets-dir=name 
                      Directory for character set files.
  --default-character-set=name 
                      Set the default character set.
  -?, --help          Display this help and exit.
  -h, --host=name     Connect to host.
  -b, --no-beep       Turn off beep on error.
  -p, --password[=name] 
                      Password to use when connecting to server. If password is
                      not given it's asked from the tty.
  -P, --port=#        Port number to use for connection or 0 for default to, in
                      order of preference, my.cnf, $MYSQL_TCP_PORT,
                      /etc/services, built-in default (3306).
  --protocol=name     The protocol to use for connection (tcp, socket, pipe,
                      memory).
  -r, --relative      Show difference between current and previous values when
                      used with -i. Currently only works with extended-status.
  -s, --silent        Silently exit if one can't connect to server.
  -S, --socket=name   The socket file to use for connection.
  -i, --sleep=#       Execute commands repeatedly with a sleep between.
  --ssl               Enable SSL for connection (automatically enabled with
                      other flags).
  --ssl-ca=name       CA file in PEM format (check OpenSSL docs, implies
                      --ssl).
  --ssl-capath=name   CA directory (check OpenSSL docs, implies --ssl).
  --ssl-cert=name     X509 cert in PEM format (implies --ssl).
  --ssl-cipher=name   SSL cipher to use (implies --ssl).
  --ssl-key=name      X509 key in PEM format (implies --ssl).
  --ssl-verify-server-cert 
                      Verify server's "Common Name" in its cert against
                      hostname used when connecting. This option is disabled by
                      default.
  -u, --user=name     User for login if not current user.
  -v, --verbose       Write more information.
  -V, --version       Output version information and exit.
  -E, --vertical      Print output vertically. Is similar to --relative, but
                      prints output vertically.
  -w, --wait[=#]      Wait and retry if connection is down.
  --connect-timeout=# 
  --shutdown-timeout=# 
  --plugin-dir=name   Directory for client-side plugins.
  --default-auth=name Default authentication client-side plugin to use.
  --enable-cleartext-plugin 
                      Enable/disable the clear text authentication plugin.

 Variables (--variable-name=value)
 and boolean options {FALSE|TRUE}  Value (after reading options)
 --------------------------------- ----------------------------------------
 count                             0
 debug-check                       FALSE
 debug-info                        FALSE
 force                             FALSE
 compress                          FALSE
 character-sets-dir                (No default value)
 default-character-set             auto
 host                              murali
 no-beep                           FALSE
 port                              3306
 relative                          FALSE
 socket                            /var/run/mysqld/mysqld.sock
 sleep                             0
 ssl                               FALSE
 ssl-ca                            (No default value)
 ssl-capath                        (No default value)
 ssl-cert                          (No default value)
 ssl-cipher                        (No default value)
 ssl-key                           (No default value)
 ssl-verify-server-cert            FALSE
 user                              root
 verbose                           FALSE
 vertical                          FALSE
 connect-timeout                   43200
 shutdown-timeout                  3600
 plugin-dir                        (No default value)
 default-auth                      (No default value)
 enable-cleartext-plugin           FALSE 

 Default options are read from the following files in the given order:
 /etc/my.cnf /etc/mysql/my.cnf /usr/etc/my.cnf ~/.my.cnf 
 The following groups are read: mysqladmin client
 The following options may be given as the first argument:
 --print-defaults        Print the program argument list and exit.
 --no-defaults           Don't read default options from any option file.
 --defaults-file=#       Only read default options from the given file #.
 --defaults-extra-file=# Read this file after the global files are read.

 Where command is a one or more of: (Commands may be shortened)
  create databasename	Create a new database
  debug			Instruct server to write debug information to log
  drop databasename	Delete a database and all its tables
  extended-status       Gives an extended status message from the server
  flush-hosts           Flush all cached hosts
  flush-logs            Flush all logs
  flush-status		Clear status variables
  flush-tables          Flush all tables
  flush-threads         Flush the thread cache
  flush-privileges      Reload grant tables (same as reload)
  kill id,id,...	Kill mysql threads
  password [new-password] Change old password to new-password in current format
  old-password [new-password] Change old password to new-password in old format
  ping			Check if mysqld is alive
  processlist		Show list of active threads in server
  reload		Reload grant tables
  refresh		Flush all tables and close and open logfiles
  shutdown		Take server down
  status		Gives a short status message from the server
  start-slave		Start slave
  stop-slave		Stop slave
  variables             Prints variables available
  version		Get version info from server
 Temp File /tmp/ptconfigure-temp-script-69617254643.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  mysql-client
 0 upgraded, 1 newly installed, 0 to remove and 250 not upgraded.
 Need to get 12.3 kB of archives.
 After this operation, 129 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-client all 5.5.41-0ubuntu0.14.04.1 [12.3 kB]
 Fetched 12.3 kB in 1s (7,469 B/s)
 Selecting previously unselected package mysql-client.
 (Reading database ... 233400 files and directories currently installed.)
 Preparing to unpack .../mysql-client_5.5.41-0ubuntu0.14.04.1_all.deb ...
 Unpacking mysql-client (5.5.41-0ubuntu0.14.04.1) ...
 Setting up mysql-client (5.5.41-0ubuntu0.14.04.1) ...
 [Pharaoh Logging] Adding Package mysql-client from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlServerGalera: Success
 ------------------------------
 Installer Finished
 ******************************



Autres paramètres
-------------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande .


MysqlServerGalera, mysql-server-galera, mysqlservergalera


avantages
-----------


Galera Cluster fournit une amélioration significative de haute disponibilité pour l'écosystème MySQL . Les différents moyens de parvenir à haute disponibilité ont généralement prévu que certaines des fonctionnalités disponibles par le biais Galera Cluster , de faire le choix d'une solution de haute disponibilité d'un exercice de compromis .


Les fonctions suivantes sont disponibles via Cluster Galera :


* Vrai multi- maître lire et écrire sur ne importe quel nœud à tout moment .
* Réplication synchrone Aucun esclave horaire, aucune donnée ne est perdue au crash du noeud .
* Tous les noeuds étroitement couplé détiennent le même état . Aucune donnée divergés entre les noeuds autorisés .
* Multi- thread esclave pour une meilleure performance . Pour toute charge de travail.
* Pas de Maître-Esclave opérations de basculement ou de l'emploi des VIP .
* Hot Standby Pas de temps mort au cours du basculement ( puisqu'il n'y a pas de basculement ) .
* Automatique Node Provisioning Pas besoin de sauvegarder manuellement la base de données et le copier dans le nouveau nœud .
* Prise en charge InnoDB .
* Transparent pour les applications obligatoires aucun ( ou minime ) changements ) à l'application .
* Pas de Lire et Ecrire Fractionnement nécessaire.
