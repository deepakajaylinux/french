===============
Mysqlserver
===============


synopsis
------------

Ce module agit comme un facilitateur d'installer mysql-serveur avec la version mise à jour via apt-get. Si le serveur MySQL existe déjà dans votre machine, il vérifie la disponibilité d'un module nouvellement mis à jour.

Le Commandement Aide
------------------------

La commande help guide les utilisateurs au sujet de la méthodologie de l'utilisation et aussi sur les actions qui peuvent être réalisées en vertu de ces modules. Il décrit également les autres noms pour mysql-serveur. La commande pour utiliser l'option d'aide est donnée ci-dessous

.. code-block:: bash

	ptconfigure mysql-server help

Cette commande permet aux utilisateurs de prendre conscience de son but et aussi sur la commande utilisée pour l'installation du serveur MySQL.
Montre une présentation picturale sur la commande d'aide de la capture d'écran ci-dessous.

.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlServer help
 ******************************


  This command allows you to install the MySQL Server. Currently only
  Mysql Workbench, the Database management GUI provided by Oracle for
  Mysql.

  MysqlServer, mysql-server, mysqlserver

        - install
        Install some Mysql Server Tools through apt-get.
        example: ptconfigure mysql-server install

  Notes, during mysql install a root password will be set. First, it'll look
  for the parameter --mysql-root-pass, if this is not set, it'll look in the
  ptconfigure config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure.

 ------------------------------
 End Help
 ******************************


installation
--------------

La commande utilisée pour l'installation du serveur mysql est donnée ci-dessous.

.. code-block:: bash

	ptconfigure mysql-server install

Lors de l'installation, le processus suivant se produit
--------------------------------------------------------------

* Ce module aide à installer quelques outils pour le serveur mysql via apt-get.
* Initialement, un mot de passe root sera fixé.
* Lors de l'installation, il va chercher un paramètre de root-passe---mysql.
* Si la racine-passe---mysql ne est pas disponible, il recherche la config de ptconfigure pour les réglages de-root-passe mysql-défaut.
* Dans le cas des deux étapes mentionnées ci-dessus se échouait, il procédera par la mise en mot de passe root à ptconfigure.

Options supplémentaires
-------------------------
Voyons à propos, les options supplémentaires impliquées dans l'installation du serveur MySQL.

.. cssclass:: table-bordered

 +------------------------+------------------------------------------------+--------------+----------------------------------------------+
 | paramètres             | Autres Paramètres                              | Option       | Commentaires                                 |
 +========================+================================================+==============+==============================================+
 |Install MySQL Server?   | A la place du serveur MySQL ces autres noms    | Y(Yes)       | Si l'utilisateur souhaite procéder le        |
 |(Y/N)                   | peuvent être utilisés: MySQLServer,            |              | processus d'installation qu'ils peuvent      |
 |                        | mysql-server, mysqlserver.                     |              | entrée comme Y.                              |
 +------------------------+------------------------------------------------+--------------+----------------------------------------------+
 |Install MySQL Server?   | A la place du serveur MySQL ces autres noms    | N(No)        | Si l'utilisateur souhaite quitter le         |
 |(Y/N)                   | peuvent être utilisés: MySQLServer,            |              | processus d'installation qu'ils peuvent      |
 |                        | mysql-server, mysqlserver.                     |              | entrée comme N|                              |
 +------------------------+------------------------------------------------+--------------+----------------------------------------------+

La capture d'écran ci-dessous vous donne une présentation graphique concernant le processus d'installation.

Si le serveur mysql est existe déjà dans votre machine, il jettera un message à l'utilisateur comme il est déjà installé. La capture d'écran ci-dessous représente le processus d'assurer:



avantages
----------

* Lors de l'installation du serveur mysql, il se installe avec la version mise à jour.
* Il se assure avant d'installer, et vérifier la disponibilité des modules.
* En cas de nouveaux modules inclus dans la version mise à jour, le module manquant sera installé individuellement.
* Il vérifie la disponibilité des fonctions de la bibliothèque dans le serveur mysql.
