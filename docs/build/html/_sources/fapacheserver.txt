==============
ApacheServer
==============

synopsis
-----------

Cette modules vise à l'installation du serveur Apache. Sans demande, il se installera automatiquement la version actuelle du serveur Apache lors de l'installation.

Commande Aide
-----------------

La commande d'aide décrit le but et les commandes disponibles dans ces modules. Il explique également la commande pour installer le module particulier.

.. code-block:: bash

 		ptconfigure ApacheServer help


La capture d'écran comme indiqué ci-dessous, représenter visuellement l'utilisation de la commande d'aide en vertu de ce module.

.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  ApacheServer, apache-server, apacheserver

        - install
        Installs Apache HTTP Server
        example: ptconfigure apacheserver install

 ------------------------------
 End Help
 ******************************



installation
-------------

Il est plus facile d'installer cet outil particulier sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

		ptconfigure ApacheServer install

Après avoir donné la commande ci-dessus, l'outil va demander que

Installez Apache Server? (Y / N)

si vous donnez une entrée en Y, le module va se installé avec succès.

La capture d'écran ci-dessous explique visuellement sur les étapes et les commandes implique l'installation.

.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer install
 Install Apache Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Server!        *
 *******************************
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
   php5-cli php5-readline
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  apache2-doc apache2-suexec-pristine apache2-suexec-custom apache2-utils
 The following NEW packages will be installed:
  apache2
 0 upgraded, 1 newly installed, 0 to remove and 39 not upgraded.
 Need to get 0 B/87.4 kB of archives.
 After this operation, 473 kB of additional disk space will be used.
 Selecting previously unselected package apache2.
 (Reading database ... 193457 files and directories currently installed.)
 Preparing to unpack .../apache2_2.4.7-1ubuntu4.4_amd64.deb ...
 Unpacking apache2 (2.4.7-1ubuntu4.4) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up apache2 (2.4.7-1ubuntu4.4) ...
 Enabling module mpm_event.
 Enabling module authz_core.
 Enabling module authz_host.
 Enabling module authn_core.
 Enabling module auth_basic.
 Enabling module access_compat.
 Enabling module authn_file.
 Enabling module authz_user.
 Enabling module alias.
 Enabling module dir.
 Enabling module autoindex.
 Enabling module env.
 Enabling module mime.
 Enabling module negotiation.
 Enabling module setenvif.
 Enabling module filter.
 Enabling module deflate.
 Enabling module status.
 Enabling conf charset.
 Enabling conf localized-error-pages.
 Enabling conf other-vhosts-access-log.
 Enabling conf security.
 Enabling conf serve-cgi-bin.
 Enabling site 000-default.
 * Starting web server apache2
 * 
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 [Pharaoh Logging] Adding Package apache2 from the Packager Apt executed correctly
 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ApacheServer: Success
 ------------------------------
 Installer Finished
 ******************************



options
----------

.. cssclass:: table-bordered

 +--------------------------+------------------------------------------+--------------+----------------------------------------+
 | paramètres               | Autres paramètres                        | requis       | commentaires                           |
 +==========================+==========================================+==============+========================================+
 |Install Apache Server?    | Au lieu de ApacheServer, nous pouvons    | Yes          | Si l'utilisateur donne entrée que oui, |
 |(Y/N)                     | utilizer apache-server, apacheserver     |              | il va procéder l'installation          |
 |                          | aussi.                                   |              |                                        |
 +--------------------------+------------------------------------------+--------------+----------------------------------------+
 |Install Apache Server?    | Au lieu de ApacheServer, nous pouvons    | No           | Si l'utilisateur donne entrée que non, |
 |(Y/N)                     | utilizer apache-server, apacheserver     |              | il va quitter le processus             |
 |                          | aussi.                                   |              | d'installation|                        |
 +--------------------------+------------------------------------------+--------------+----------------------------------------+



version
---------

Bien que l'outil est en cours de traitement, il sera automatiquement attrape la plus récente version mise à jour et permet de se préparer pour l'installation.


Avantages pour les utilisateurs finaux
---------------------------------------

* Cette modules aide les utilisateurs à installer le serveur Apache. Il simplifie le travail des utilisateurs pendant l'installation du 
  serveur ainsi que son vérifier automatiquement la version actuelle du serveur Apache.
* Il est bien de choses à faire dans Cent OS et ainsi que dans Ubuntu.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse, ce qui est un avantage supplémentaire.
