==============
Project
==============

Synopsis
-------------

Dans les affaires et la science contemporaine un projet est définie comme une entreprise collaborative, impliquant la recherche ou de la conception, qui est soigneusement planifié pour atteindre un objectif particulier. Les projets peuvent encore être définis comme temporaire plutôt que permanente des systèmes sociaux ou des systèmes de travail qui sont constitués par des équipes à l'intérieur ou à travers les organisations pour accomplir des tâches particulières dans des contraintes de temps. Un projet en cours est généralement appelé (ou évolue vers) un programme.

Cette commande fait partie des modules par défaut et gère les fonctions d'initialisation du projet, comme la configuration d'un projet, ou d'un conteneur de projet et également l'installation Jenkins fichiers de construction dans une instance en cours d'exécution Jenkins.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de projet. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
	
		ptdeploy project help
       
.. code-block:: bash

 kevell@corp:/# ptdeploy Project help
 ******************************


  This command is part of Default Modules and handles Project initialisation functions, like configuring a project, or a project
  container and also installing Jenkins build files into a running Jenkins instance.

  Project, project, proj


          - container
          make a container folder for revisions (like /var/www/applications/*APP NAME*)
          example: ptdeploy proj container
          example: ptdeploy proj container --yes --proj-container="/var/www/applications/the-app"

          - init
          initialize Dapper project
          example: ptdeploy proj init
          example: ptdeploy proj init --yes

          - build-install
          copy jenkins project stored in repo to running jenkins so you can run builds
          example: ptdeploy proj build-install
          example: ptdeploy proj build-install
                        --jenkins-fs-dir=/var/lib/jenkins # --guess will set this to /var/lib/jenkins
                        --original-build-dir="/var/www/applications/the-app/build/config/ptconfigure/Project/jenkins-builds"
                        --target-job-name="Project_Build"
                        --new-job-dir="Project_Build_Alternate_Name"  # If target one is not available

 ------------------------------
 End Help
 ******************************


Container
----------------

This command helps make a container folder for revisions (like /var/www/applications/*APP NAME*). 
When the user needs to install, the user can issue the following commands for DBIstall. The system will execute the process of installation.

.. code-block:: bash
	
	 ptdeploy proj container

.. code-block:: bash

 kevell@corp:/# ptdeploy proj container
 Do you want to Modify Project Container Settings? (Y/N) 
 y
 Do you want to initialize this as a ptdeploy project Container? (Y/N) 
 y
 What is your Project Container directory?
 /var/www/applications/the-app
 Project Container directory created
 /var/www/applications/the-app space /var/www/applications/the-appMoving to Container
 /var/www/applications/the-app
 Showing Container Directory
 Project Container file created
 ******************************


 Seems Fine...Project Editor Finished
 ******************************




initialisation
----------------

Lorsque l'utilisateur a besoin pour initialiser projet Dapper, l'utilisateur peut émettre les commandes suivantes. Le système exécute le processus.

.. code-block:: bash
	
		 ptdeploy proj init


.. code-block:: bash

 kevell@corp:/# ptdeploy proj init
 Do you want to Modify Project Settings To initialise Project? (Y/N) 
 Y
 Do you want to initialize this as a ptdeploy project? (Y/N) 
 Y
 ******************************


 Seems Fine...Project Editor Finished
 ******************************



Build-Installez
----------------

Lorsque les besoins des utilisateurs copient projet Jenkins stockée dans repo à l'exécution de Jenkins, l'utilisateur peut émettre les commandes suivantes. Le système exécute le processus.

.. code-block:: bash
	
		 ptdeploy proj build-install

alternatifs Paramètre
--------------------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la commande.

Project, project and proj

eg: ptdeploy Project help/  ptdeploy proj help
                       
avantages
--------------

* Aide faire un dossier contenant des révisions
* Aide à initialiser projet dapper
