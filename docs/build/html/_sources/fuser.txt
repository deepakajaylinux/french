====
User
====

Synopsis
--------------

Un utilisateur est une personne qui utilise un ordinateur. Ordinateur possède un nom pour chaque compte qu'il crée, et ce est ce nom par lequel une personne accède à utiliser l'ordinateur. Certains services de système d'exécution en utilisant également des comptes d'utilisateurs restreints ou privilégiés.

Gestion des utilisateurs se fait dans le but de la sécurité en limitant l'accès à certains égards spécifiques. Le super-utilisateur (root) a accès à tout le système d'exploitation et sa configuration; il est destiné à un usage administratif. Les utilisateurs non privilégiés peuvent utiliser les programmes su et sudo pour escalade de privilège contrôlée.

Une partie fondamentale de l'administration du système est la configuration et la gestion des utilisateurs et des groupes. Une partie de cette tâche consiste à surveiller le journal dans les capacités de toutes les entités du système.

Nous allons explorer ces concepts sur une Ubuntu 12.04 VPS, mais vous pouvez suivre sur ne importe quelle distribution Linux mise à jour.

Aide Command
----------------------

Cette commande permet de déterminer l'utilisation de module de l'utilisateur. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.



.. code-block:: bash

        ptconfigure user help

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash 

 kevell@corp:/# ptconfigure user help
 ******************************
 This command allows you to modify create or modify users

 User, user

       - create
       Create a new system user, overwriting if it exists
       example: ptconfigure user create --username="somename"

       - remove
       Remove a system user
       example: ptconfigure user remove --username="somename"

       - set-password
       Set the password of a system user
       example: ptconfigure user set-password --username="somename" --new-password="somepassword"

       - exists
       Check the existence of a user
       example: ptconfigure user exists --username="somename"

       - show-groups
       Show groups to which a user belongs
       example: ptconfigure user show-groups --username="somename"

       - add-to-group
       Add user to a group
       example: ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

       - remove-from-group
       Remove user from a group
       example: ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

Create
-----------

Lorsque l'utilisateur a besoin de créer un nouveau compte utilisateur du système, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

        ptconfigure user create --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user create
 
 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************


Remove
--------------

Lorsque l'utilisateur doit supprimer un compte d'utilisateur du système, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

	ptconfigure user remove --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user remove

 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************



Set password
---------------------------

Lorsque l'utilisateur doit définir le mot de passe d'un utilisateur du système, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

	ptconfigure user set-password --username="somename" --new-password="somepassword"

.. code-block:: bash


 kevell@corp:/# ptconfigure user set-password

 Enter Username:
 kevell
 Enter New Password:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 

 ------------------------------
 User Mods Finished
 ******************************


Exists
------------

Lorsque l'utilisateur doit vérifier l'existence d'un utilisateur, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash


	ptconfigure user exists --username="somename"

.. code-block:: bash


 kevell@corp:/# ptconfigure user exists

 Enter Username:
 kevell
 ****************************** 


 User Modifications:
 --------------------------------------------

 User: Success = User Exists
 User Name: 

 ------------------------------
 User Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure user exists

 Enter Username:
 karuna
 ******************************


 User Modifications:
 --------------------------------------------

 User: Failure - User Does Not Exist
 User Name: 

 ------------------------------
 User Mods Finished
 ******************************

Show Groups
---------------------

Lorsque l'utilisateur a besoin de montrer groupes auxquels appartient un utilisateur, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

	ptconfigure user show-groups --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user show-groups

 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: kevell


 ------------------------------
 User Mods Finished
 ******************************


Add to group
----------------------

Lorsque l'utilisateur doit ajouter un utilisateur à un groupe, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

	ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

.. code-block:: bash


 kevell@corp:/# ptconfigure user add-to-group --username="kevell" --groupname="kumar"

 Enter New Password:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************


Remove from Group
------------------------------

Lorsque l'utilisateur doit supprimer l'utilisateur d'un groupe, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

	ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

.. code-block:: bash


 kevell@corp:/# ptconfigure user remove-from-group --username="kevell" --groupname="kumar"

 Enter New Password:
 kevell

 /usr/sbin/deluser: You may not remove the user from their primary group.
 [Pharaoh Logging] [User] Removing User kevell from the Group kevell did not execute correctly
 ******************************


 User Modifications:
 --------------------------------------------

 User: 

 ------------------------------
 User Mods Finished
 ******************************



Autres paramètres
--------------------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande.

User, user

example: ptconfigure User help /ptconfigure user help


avantages
--------------

L'authentification de l'utilisateur sur Linux est une zone relativement souple de la gestion du système. Il ya plusieurs façons d'accomplir le même objectif avec des outils très simples.
