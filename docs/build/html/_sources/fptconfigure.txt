=============
PTConfigure
=============

synopsis
------------

Cette installation d'ascenseurs du module dans la version mise à jour. L'automatisation est possible. Situation pour le répertoire de données et le répertoire de l'exécuteur peut être spécifié lors de l'installation de ce module. Il spécifie la configuration de votre environnement. Il est amical avec Ubuntu et cent OS utilisateur.

Commande Aide
-----------------------

  Cette commande d'aide de guider l'utilisateur à propos de ptconfigure. Convient à tous les types d'utilisateurs. Il dépeint les autres paramètres et commandes pour l'installation. La commande d'aide suivant la capture d'écran et aideront l'utilisateur concernant l'utilisation.

.. code-block:: bash

		ptconfigure ptconfigure help

.. code-block:: bash
 
	kevell@corp:/# ptconfigure ptconfigure help
	****************************************


	This command allows you to update ptconfigure.

	ptconfigure, cleo, ptconfigure

        - install
        Installs the latest version of ptconfigure
        example: ptconfigure ptconfigure install

	------------------------------
	End Help
	*******************************************

installation
-------------
              
  Ce est un processus de plus simple à installer le module de ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

  ptconfigure ptconfigure install

Après avoir donné la commande ptconfigure sera installé avec de nouvelles mises à jour.

Après la saisie de l'utilisateur est passé il va vérifier si un fichier est manquant et à la main, il se installera automatiquement.

La capture d'écran ci-dessous énumère il.


.. code-block:: bash


 kevell@corp:/# ptconfigure ptconfigure install

 Install ptconfigure - Update to latest version ? (Y/N)
 y
  *******************************
 *        Pharaoh Tools        *
 *          ptconfigure!         *
 *******************************
 What is the program data directory? Found "/opt/ptconfigure" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/ptconfigure.git'  /tmp/ptconfigure/ptconfigureCloning into '/tmp/ptconfigure/ptconfigure'...
 remote: Counting objects: 19656, done.
 remote: Total 19656 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (19656/19656), 6.15 MiB | 66.00 KiB/s, done.
 Resolving deltas: 100% (11790/11790), done.
 Checking connectivity... done.
 Program Data Folder /opt/ptconfigure Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptconfigure: Success
 ------------------------------
 Installer Finished
 ******************************

option
-------

.. cssclass:: table-bordered


 +----------------------------------+-------------------------------------------+-----------+-------------------------------------+
 | Paramètres                       | Alternative Paramètre                     | options   | commentaires                        |
 +==================================+===========================================+===========+=====================================+
 |Install ptconfigure ptconfigure   | Il existe trois paramètres qui peuvent    | Y(Yes)    | Il va installer ptconfigure sous    |        
 |Update to latest version? (Y/N)   | être utilisés . ptconfigure, Cleo ,       |           | ptconfigure                         |
 |                                  | ptconfigure                               |           |                                     |
 +----------------------------------+-------------------------------------------+-----------+-------------------------------------+
 |Install ptconfigure ptconfigure   | Il existe trois paramètres qui peuvent    | N(No)     | Il sortira de l'installation        |
 |Update to latest version? (Y/N)   | être utilisés . ptconfigure, Cleo ,       |           |                                     |
 |                                  | ptconfigure|                              |           |                                     |
 +----------------------------------+-------------------------------------------+-----------+-------------------------------------+



avantages
--------------

* ptconfigure est utilisé pour installer le fichier de configuration. Lors de l'installation se il ya ne importe quel fichier existant est 
  l'écrasement du contenu.
* Nouvelle version peut mettre à jour automatiquement.
* Updation peut être fait dans ce module sans recherche sur le web.

