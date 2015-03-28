===============
Appsettings
===============

synopsis
-----------------

AppSetting qui nous permet de garder les paramètres configurables et d'application larges qu'une demande a besoin pour effectuer les tâches correctement. Cela contribue à l'entretien facile et le déploiement de l'application . En utilisant appsetting nous pouvons définir des valeurs définies par l'utilisateur .


Commande Aide
------------------

Cette commande permet de déterminer l'utilisation de appsettings . Il énumère les autres paramètres et la syntaxe pour le fonctionnement du appsettings module. La commande d'aide pour appsettings est représentée ci-dessous .


.. code-block:: bash

	ptdeploy appsettings help

La représentation picturale de la commande d'aide est donnée ci-dessous ,


.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings help

 ******************************


  This command is part of Default Modules and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  AppSettings, appsettings
	
        - set
        Set a configuration value
        example: ptdeploy appsettings set

        - get
        Get the value of a setting you have configured
        example: ptdeploy appsettings get

        - delete
        Delete a setting you have configured
        example: ptdeploy appsettings delete

        - list
        Display a list of all default available settings
        example: ptdeploy appsettings list

 ------------------------------
 End Help
 ******************************


Set
---------

La commande set permet de définir une valeur de configuration . La commande ci-dessous va exécuter le processus .

.. code-block:: bash

	ptdeploy appsettings set

La représentation picturale de la commande ci-dessus est listé ci-dessous ,


.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings set

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 What Value do you want to give this variable?
 /tmp/
 ******************************

 Seems Fine...
 In Application Config
 ******************************


Get
--------

La commande Get permet d'obtenir la valeur d'un paramètre que vous avez déjà configuré . La commande ci-dessous va exécuter le processus .


.. code-block:: bash

	ptdeploy appsettings get


La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings get

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 4
 ******************************


 Variable Name: linux-user
 Variable Value: karuna
 
 In Application Config
 ******************************


Delete
--------

La commande delete permet de supprimer un paramètre que vous avez configuré . La commande ci-dessous va exécuter le processus .

.. code-block:: bash

	ptdeploy appsettings delete

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings delete

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 ******************************


 Seems Fine...
 In Application Config
 ******************************



List
-------

La commande de liste permet d'afficher une liste de tous les paramètres par défaut disponibles . Le commad ci-dessous va exécuter le processus .


.. code-block:: bash

	ptdeploy appsettings list

La représentation picturale de la commande ci-dessus est listé ci-dessous ,


.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings list

 Do you want to Configure Application Settings? (Y/N) 
 y
 ******************************


   Variable Type is: allSet 
   linux-user is: karuna 
   mysql-admin-user is: mani 
   Variable Type is: allTotal 
   mysql-admin-user 
   mysql-admin-host 
   mysql-admin-pass 
   linux-user 
   linux-user-dir 
   program-dir 
   temp-base-dir 
   distro 
   op-sys 
   linux-type 

 In Application Config
 ******************************



Autres paramètres
--------------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande .

AppSettings, appsettings


avantages
-----------

* Accès fortement typé
* Sensibilité non de cas


