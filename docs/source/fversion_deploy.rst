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

Version, version, VERSION

installation
----------------

L'installation comprend l'installation de la version requise pour rendre l'installation dans une version mise à jour . Ce est un processus manifeste pour installer le module de version sous ptdeploy . Version en utilisant simplement la commande ci-dessous ,

.. code-block:: bash

	ptdeploy version Install

Après dynamiser la commande il catéchiser entrée .

Lorsque l'entrée d'utilisateur comme il sera automatiquement oui installer la version avec la vérification du système. Si pas quitter l'installation . La capture d'écran ci-dessous montrent la version et ses fonctions.

Option
------------

.. cssclass:: table-bordered

 +--------------------------+-----------------+----------------------------------------------+--------------------------------------+
 | paramètres		    | option 	      | Alternative Paramètre		             | commentaires			    |
 +==========================+=================+==============================================+======================================+
 |Install version?(Y/N)	    | Yes	      | Au lieu d'utiliser la version                | installé avec succès		    |
 |			    |		      | l'utilisateur peut utiliser Version,VERSION  | le cadre du module de ptdeploy       |
 +--------------------------+-----------------+----------------------------------------------+--------------------------------------+
 |Install version?(Y/N)	    | No	      | Au lieu d'utiliser la version                | Quittez l'écran                      |
 |			    |		      |	l'utilisateur peut utiliser Version,VERSION| | 	               			    |
 +--------------------------+-----------------+----------------------------------------------+--------------------------------------+


avantages
---------------

* Nouvelle version peut être mis à jour.
* Il est adapté avec Ubuntu et CentOS.
* Sensibilité non de cas
* L'automatisation est possible
* Simple à tapez les commandes

