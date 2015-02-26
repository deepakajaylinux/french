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

 kevell@corp:/# ptconfigure apacheserver install
 Install Apache Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Server!        *
 *******************************
 [Pharaoh Logging] Package apache2 from the Packager Apt is already installed, so not installing
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
