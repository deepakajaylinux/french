=========
Version
=========

synopsis
----------------

Ce module permet d' installer la version mise à jour sous ptdeploy . Le contrôle de version plus couramment exécutent comme des applications autonomes , mais le contrôle de révision est également intégré dans divers types de système d'exploitation comme Ubuntu et Cent OS . Version la plus permet à plusieurs développeurs de modifier le même fichier en même temps . Le premier développeur de "archiver " changements dans le référentiel central réussit toujours . Le système peut fournir des installations de fusionner d'autres changements dans le référentiel central, et de préserver les changements de la première développeur quand d'autres développeurs vérifier in.It soutient Ubuntu et CentOS .

Commande Aide
-----------------------

La commande help conduit les utilisateurs concernant la version du ptdeploy . Les options qui sont inclus dans les modules de version. La commande help répertorie les autres paramètres de la version sous module de ptdeploy . Il décrit également la syntaxe pour la version . La commande d'aide pour la version est indiquée ci-dessous.

.. code-block:: bash

	ptdeploy  version help

La capture d'écran ci-dessous montre l'effort plein de ptdeploy .


.. code-block:: bash


 kevell@corp:/# ptdeploy Version help
 ******************************


  This command is part of Default Modules and handles Application Versioning, allowing for rollbacks and the like.

  Version, version, vrs

          - specific
          Will change back the *current* symlink to whichever available version you pick
          example: ptdeploy version specific --limit=4 --container=/var/www/applications/the-app --version=2

          - latest
          Will change back the *current* symlink to the latest created version
          example: ptdeploy version latest
          example: ptdeploy version latest --limit=3 --container=/var/www/applications/the-app

          - rollback
          Will change back the *current* symlink to the latest created version but one
          example: ptdeploy version rollback
          example: ptdeploy version rollback --limit=3 --container=/var/www/applications/the-app


      You can also apply a limit to the number of Versions to keep by using the --limit parameter
          example: ptdeploy version latest --limit=3

 ------------------------------
 End Help
 ******************************


paramètre alternatif
--------------------------------

Il existe deux solutions de rechange disponibles en version . ils sont

Version, version, vrs


Specific
-----------

L'option spécifique permet à l'utilisateur de changer de retour le répertoire de la version actuelle de faire une version spécifique. La commande pour l'option spécifique est indiqué ci-dessous ,

.. code-block:: bash

        ptdeploy version specific

or

.. code-block:: bash

        ptdeploy version specific --limit=4 --container=/opt/versiontest/ --version=2

.. code-block:: bash


 kevell@corp:/# ptdeploy version specific

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 Please Choose Version to make current (Showing newest first, Enter none for newest):
 --- All Versions: ---
 (0) karuna 

 0
 How many Versions to limit to? Enter 0 to ignore version limits
 2
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************
 
.. code-block:: bash

 kevell@corp:/# ptdeploy version specific --limit=4 --container=/opt/versiontest/ --version=2

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 


Latest
----------

La dernière option permet à l'utilisateur de changer le lien de retour à la dernière version disponible . La commande pour le dernier processus d'exécution est illustré ci-dessous ,

.. code-block:: bash 

        ptdeploy version latest

or

.. code-block:: bash

        ptdeploy version latest --limit=3 --container=/var/www/applications/the-app

.. code-block:: bash


 kevell@corp:/# ptdeploy version latest

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 How many Versions to limit to? Enter 0 to ignore version limits
 5
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy version latest --limit=3 --container=/opt/versiontest/

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************


Rollback
----------

L'option de restauration permet à l'utilisateur d'apporter des modifications à la version existante . Le processus d'exécution de rollback est illustré ci-dessous ,

.. code-block:: bash

        ptdeploy version rollback

or

.. code-block:: bash

        ptdeploy version rollback --limit=3 --container=/opt/versiontest/

.. code-block:: bash


 kevell@corp:/# ptdeploy version rollback

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 How many Versions to limit to? Enter 0 to ignore version limits
 4
 Removed Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy version rollback --limit=3 --container=/opt/versiontest/

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************



Option
------------

.. cssclass:: table-bordered

 +--------------------------+-----------------+----------------------------------------------+--------------------------------------+
 | paramètres		    | option 	      | Alternative Paramètre		             | commentaires			    |
 +==========================+=================+==============================================+======================================+
 |Install version?(Y/N)	    | Yes	      | Au lieu d'utiliser la version                | installé avec succès		    |
 |			    |		      | l'utilisateur peut utiliser Version,         | le cadre du module de ptdeploy       |
 |                          |                 | version, vrs                                 |                                      |
 +--------------------------+-----------------+----------------------------------------------+--------------------------------------+
 |Install version?(Y/N)	    | No	      | Au lieu d'utiliser la version                | Quittez l'écran                      |
 |			    |		      |	l'utilisateur peut utiliser Version,         | 	               			    |
 |                          |                 | version, vrs|                                |                                      |
 +--------------------------+-----------------+----------------------------------------------+--------------------------------------+


avantages
---------------

* Nouvelle version peut être mis à jour.
* Il est adapté avec Ubuntu et CentOS.
* Sensibilité non de cas
* L'automatisation est possible
* Simple à tapez les commandes

