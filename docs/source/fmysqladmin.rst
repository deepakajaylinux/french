================
MysqlAdmins
================

synopsis
---------

Ce module aide à l'installation et ainsi que la gestion des utilisateurs admin pour mysql sans utiliser l'utilisateur root. En utilisant ce, les utilisateurs peuvent gérer leurs fonctions administratives.

Commande Aide
-------------

La commande Aide guide les utilisateurs au sujet de la commande utilisée pour installer les admins de mysql, et aussi ses avantages. La commande utilisée pour l'option d'aide en vertu de ce admins MySQL est illustré ci-dessous.

.. code-block:: bash

	ptconfigure MysqlAdmins help

La capture d'écran comme ci-dessous peut conduire l'utilisateur dans le traitement de la commande d'aide pour les admins de mysql.

.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlAdmins help
 ******************************


  This command allows you to install admin users for MySQL so that MySQL can
  be managed without using the Root User.

  MysqlAdmins, mysql-admins, mysqladmins

        - install
        Installs Mysql Admin Users.
        example: ptconfigure mysql-admins install

 ------------------------------
 End Help
 ******************************

installation
-------------

Installation admins mysql à votre machine facilite les utilisateurs de spécifier et de gérer leurs actions administratives. La commande utilisée pour l'installation admins mysql est marqué ci-dessous.

.. code-block:: bash

	ptconfigure MysqlAdmins install

En outre, les opérations suivantes se affichent dans un format tabulaire se produit.

.. cssclass:: table-bordered

 +-------------------------+-------------------------------------------+-----------+---------------------------------------------------+
 | paramètres              | Autres Paramètres                         | Option    | Commentaires                                      |
 +=========================+===========================================+===========+===================================================+
 |Install Admin User for   | A la place de ces MysqlAdmins autres noms | Y(Yes)    | Si l'utilisateur souhaite procéder le processus   |
 |MySQL? (Y/N)             | peuvent être utilisés: mysql-admins,      |           | d'installation qu'ils peuvent entrée comme Y.     |
 |                         | mysqladmins.                              |           |                                                   |
 +-------------------------+-------------------------------------------+-----------+---------------------------------------------------+
 |Install MySQL Server?    | A la place de ces MysqlAdmins autres noms | N(No)     | Si l'utilisateur souhaite quitter le processus    |
 |(Y/N)                    | peuvent être utilisés: mysql-admins,      |           | d'installation qu'ils peuvent entrée comme N      |
 |                         | mysqladmins.|                             |           |                                                   |
 +-------------------------+-------------------------------------------+-----------+---------------------------------------------------+

Si l'utilisateur procède le processus d'installation, ils peuvent formuler leurs fonctions administratives en précisant les contraintes 
suivantes.

* MySQL utilisateur root
* MySQL Racine col
* MySQL New utilisateur Admin
* MySQL nouvel admin passe

Si l'utilisateur souhaite traiter des admins installation de mysql dans un système à distance ils peuvent spécifier:

* Serveur MySQL.

La capture d'écran ci-dessous vous donne une représentation picturale sur le processus d'installation comme décrit ci-dessus.

.. code-block:: bash



 kevell@corp:/# ptconfigure mysql-admins install 
 Install Admin User for MySQL? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         MySQL Admins!        * 
 ******************************* 
 Enter MySQL Root User: 
 root 
 Enter MySQL Root Pass: 
 root123 
 Enter MySQL New Admin User: 
 kevells 
 Enter MySQL New Admin Pass: 
 kevells
 Enter MySQL Host: Enter nothing for 127.0.0.1 
 127.0.0.1   
 Creating /tmp/ptconfigure-temp-script-4745646149.sh 
 chmod 755 /tmp/ptconfigure-temp-script-4745646149.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-4745646149.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-4745646149.sh 
 Warning: Using a password on the command line interface can be insecure. 
 Temp File /tmp/ptconfigure-temp-script-4745646149.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 MysqlAdmins: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  


avantages
----------

* En cas d'admins MySQL est déjà installé dans la machine de l'utilisateur, un message va comparaître pour informer les utilisateurs comme ce 
  est déjà installé.
* En utilisant ce module, les administrateurs peuvent gérer leurs actions administratives selon les exigences.
* On peut effectuer le processus d'installation, même dans un système distant.
* Sans l'aide des utilisateurs root, les utilisateurs peuvent installer les admins de mysql.
