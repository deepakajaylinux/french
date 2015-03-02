===========
PTTest 
===========

synopsis
---------

Module pttest est pour la manipulation de la configuration de la suite de tests et l'exécution en utilisant un ensemble commun de règles à travers une gamme d'outils et de technologies. Il peut être utilisé pour générer des suites de tests démarrage pour vos applications, et de test automatisé scripts d'exécution en quelques minutes.

Ce module vise à l'installation de la dernière version de pttest outil.

Commande Aide
----------------

La commande help guide l'utilisateur à fournir ce qui est nécessaire pour accomplir la tâche. La commande de faire usage de l'aide sous la borne est donnée comme suit,

.. code-block:: bash

	ptconfigure pttest help


Le cliché ci-dessous vous donne une représentation picturale de commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptconfigure pttest help
 ******************************


  This command allows you to update pttest.

  pttest, cleo, pttest

        - install
        Installs the latest version of pttest
        example: pttest pttest install

 ------------------------------
 End Help
 ******************************

 
installation
-------------

La meilleure façon d'installer l'une des applications pharaon est par ptconfigure. Si vous avez déjà installé ptconfigure alors vous pouvez installer pttest en utilisant la commande suivante,

.. code-block:: bash

	ptconfigure pttest install

Le cliché ci-dessous vous donne une représentation picturale de commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptconfigure pttest install
 Install pttest - Update to latest version ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          pttest!         *
 *******************************
 What is the program data directory? Found "/opt/pttest" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/pttest.git'  /tmp/pttest/pttestCloning into '/tmp/pttest/pttest'...
 remote: Counting objects: 909, done.
 remote: Total 909 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (909/909), 361.15 KiB | 87.00 KiB/s, done.
 Resolving deltas: 100% (412/412), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 pttest: Success
 ------------------------------
 Installer Finished
 ******************************


Options
------------

.. cssclass:: table-bordered


 +----------------------+-------------------------+-----------+---------------------------------------------------------------------+
 | paramaters           | Autres paramètres       | requis    | Commentaires                                                        |
 +======================+=========================+===========+=====================================================================+
 |ptconfigure pttest    | PTTest, cleo, pttest    | Yes       | Cette commande va installer le module pttest                        |
 |install               |                         |           |                                                                     |
 +----------------------+-------------------------+-----------+---------------------------------------------------------------------+
 |Install pttest ?      | PTTest, cleo, pttest    | Y         | Si l'utilisateur saisit Y, ce module vérifie version précédemment   |
 |( Y/N)                |                         |           | installée, se il a été mis à jour sorties à la dernière version     |
 |                      |                         |           | ou bien il installe le nouveau package. Pour enregistrer les        |
 |                      |                         |           | fichiers de programme à l'utilisateur spécifique de chemin doit     |
 |                      |                         |           | entrer touche touche '/' ou bien il utilise le chemin par défaut    |
 |                      |                         |           | comme indiqué dans la figure.                                       |
 +----------------------+-------------------------+-----------+---------------------------------------------------------------------+
 |Install pttest ?      |  PTTest, cleo, pttest   | N         | Si l'Utilisateur saisit Y, Ce module de version verifie             |
 |( Y/N)                |                         |           | précédemment Installée, se il was mis à jour sorties à La Dernière  |
 |                      |                         |           | Version ous bien il Installe le nouveau package. Verser Enregistrer |
 |                      |                         |           | Les fichiers de programme à l'Utilisateur Spécifique de chemin Doit |
 |                      |                         |           | ENTRER touche touche '/' ou bien il utiliser le chemin par défaut   |
 |                      |                         |           | Comme Indique Dans la figure.|                                      |
 +----------------------+-------------------------+-----------+---------------------------------------------------------------------+
 
Avantages pour les utilisateurs
---------------------------------

* Utilisation facile d'accès et l'installation
* Le codage est insensible à la casse
* Source complet est disponible et il n'y a pas de frais de licence.
