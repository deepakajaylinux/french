==============
JUser
==============

synopsis
-------------

Un utilisateur est une personne qui utilise un service informatique ou un réseau. Les utilisateurs utilisent généralement un système ou un produit logiciel sans l'expertise technique nécessaire pour comprendre pleinement.


Souvent, un utilisateur a un compte d'utilisateur et est identifié au système par un nom d'utilisateur (ou le nom d'utilisateur). Autres termes comme nom d'utilisateur incluent le nom de connexion, nom d'écran.


Un compte d'utilisateur permet à un utilisateur pour s'authentifier sur un système et d'accorder l'autorisation d'accéder aux ressources fournies par ou connecté à ce système ; Cependant, l'authentification n'implique pas d'autorisation. Pour vous connecter à un compte, un utilisateur est généralement tenu pour s'authentifier avec un mot de passe ou autres informations d'identification aux fins de comptabilité, sécurité, exploitation forestière et gestion des ressources.


Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation du module "JUtilisateur". L'utilisateur viendra à connaître le différent façons/format d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.


.. code-block:: bash
        
	jrush juser help

.. code-block:: bash

 kevell@corp:/# jrush juser help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update JUser.

  JUser, juser

        - delete
        Deletes a user
        example: jrush juser delete

        - info
        Display the details of a user
        example: jrush juser info

        - change the password of a user
        Change a users password
        example: jrush juser password

 ------------------------------
 End Help
 ****************************************




Delete
----------------

Lorsque l'utilisateur a besoin de supprimer un utilisateur de la machine, le dessous étant donné de commande exécutera le processus d'installation.

.. code-block:: bash
        
	jrush juser delete ..config file=”bootstrap file path”

La représentation picturale de la commande ci-dessus est listée ci-dessous,


.. code-block:: bash

 kevell@corp:/# jrush juser delete --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Delete:
 -------------------------

 The following user has been deleted:

 User ID: 0
 Name: 
 User Name: 
 Email: 
 ------------------------------
 JUser Delete Finished
 ****************************************


Info
----------------

Lorsque l'utilisateur a besoin afficher les détails d'un utilisateur dans la machine, le dessous étant donné de commande exécutera le processus d'installation.

.. code-block:: bash
        
	jrush juser info ..config file=”bootstrap file path”

La représentation picturale de la commande ci-dessus est listée ci-dessous,


.. code-block:: bash


 kevell@corp:/# jrush juser info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Info:
 -------------------------
 
 User ID: 
 Name: 
 User Name: 
 Email: 

 ------------------------------
 JUser Info Finished
 ****************************************

Password
----------------

Lorsque l'utilisateur doit changer le mot de passe d'un utilisateur dans la machine, le dessous étant donné de commande exécutera le processus d'installation.


.. code-block:: bash
        
	jrush juser password ..config file=”bootstrap file path”


Alternative Paramètre
-----------------------------


Soit du paramètre alternatif deux peut être utilisé dans la commande-juser et JUser


eg: jrush juser info ..config file=”bootstrap file path” / jrush JUser info ..config file=”bootstrap file path”                            

.. code-block:: bash

 kevell@corp:/# jrush juser password --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 5
 Enter a new Password. To enter as parameter use --password 
 12345
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Password:
 -------------------------

 User ID: 0
 Name: 
 User Name: 
 Email: 
 User Password: NOT SET

 ------------------------------
 JUser Password Finished
 ****************************************


avantages
--------------

* Facile à obtenir des informations sur un utilisateur à l'aide d'une seule commande 
* facile de changer le mot de passe d'un utilisateur du serveur principal à l'aide de la commande unique * facile à gérer les comptes 
  d'utilisateurs

