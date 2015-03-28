========
Cleofy
========

synopsis
-----------

Ce module vise à faciliter les utilisateurs à créer un ensemble standard de fichiers de pilote automatique pour leur projet. Voyons comment utiliser ce module, ainsi que sur les fonctions de cleofy des sujets à venir.

Commande Aide
-----------------------

La commande d'aide est un manuel d'utilisation brève qui facilite les utilisateurs d'obtenir conscience concernant l'utilisation, la manipulation des méthodologies de ce module pour effectuer des fonctions différentes. Il indique également les sorties de paramètres alternatifs qui peuvent être utilisés dans les déclarations. Il souligne l'exemple de syntaxe pour l'utilisation et l'accès à différentes fonctions en vertu cleofy.

La commande utilisée pour déclarer aide option sous cleofy est illustré ci-dessous,

.. code-block:: bash

	ptconfigure cleofy help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu cleofy.

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy help

 ******************************


 This command is part of a default Module Core and provides you with a method by which you can create a standard set of Autopilot files for your project from the command line.  


 Cleofy, cleofy  

 - list        
 	List all of the autopilot files in your build/config/ptconfigure/autopilots        
	example: ptconfigure cleofy list        

 - standard        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
	example: ptconfigure cleofy standard        

 - tiny        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "tiny" style infrastructure.        	example: ptconfigure cleofy tiny        

 - medium        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure.        	example: ptconfigure cleofy medium        

 - medium-web        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure,
        with web but not database.        
 	example: ptconfigure cleofy medium-web        

 - db-cluster        

	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
 	example: ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

 - install-generic-autopilots        
	Install the generic Cleofy autopilot templates for a Tiny or Medium (Current Default) set of Environments        
 example: ptconfigure cleofy install-generic-autopilots        
	example: ptconfigure cleofy install-generic-autopilots        
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    

 ------------------------------
 End Help
 ******************************

Fonctions de cleofy
------------------------


Ce sujet représente sur les diverses fonctions de cleofy sous ce module comme indiqué ci-dessous,

* Liste
* norme
* minuscule
* Medium
* Moyen-web
* DB-cluster
* Install_generic_autopilots


liste
-----

Cette fonction vise à la liste de tous les fichiers du pilote automatique dans votre emplacement spécifié (build / config / ptconfigure / pilotes automatiques). La syntaxe pour appliquer cette fonction est illustré ci-dessous,

.. code-block:: bash

	ptconfigure cleofy list

standard
------------

Cette fonction contribue à la création d'un ensemble par défaut de pilotes automatiques de ptconfigure (dans build / config / ptconfigure / de pilotes automatiques) pour le projet des utilisateurs. Cette fonction peut être appliquée en utilisant simplement la commande ci-dessous,

.. code-block:: bash

	ptconfigure cleofy standard


.. code-block:: bash

 kevell@corp:/# ptconfigure cleofy standard

 Cleofy This? (Y/N) 
 y
 Environment 1  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 test1
 Value for: Default Temp Dir (should usually be /tmp/)

 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-cleo-dapper.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-new.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-update.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-any-box.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-ubuntu.php
 ******************************


 Success
 In Cleofy
 ******************************




minuscule
---------------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de ptconfigure (dans build / config / ptconfigure / de pilotes automatiques) pour un projet avec petite infrastructure. Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	ptconfigure cleofy tiny

moyen
-----------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de ptconfigure (dans build / config / ptconfigure / de pilotes automatiques) pour un projet d'infrastructures moyenne. Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	ptconfigure cleofy medium

Medium_Web
---------------------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de ptconfigure (dans build / config / ptconfigure / de pilotes automatiques) pour un projet avec le milieu avec l'infrastructure Web, mais pas la base de données. Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	ptconfigure cleofy medium-web

DB_cluster
---------------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de ptconfigure (dans build / config / ptconfigure / de pilotes automatiques) pour le projet de l'utilisateur.
Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

Install_generic_autopilots
-------------------------------------

Cette fonction aide à l'installation de modèles de pilote automatique génériques pour petit ou moyen ensemble de l'environnement en utilisant simplement la commande comme donnée
dessous

.. code-block:: bash
	
	ptconfigure cleofy install-generic-autopilots        
Or,

.. code-block:: bash

	ptconfigure cleofy install-generic-autopilots
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    


Pour mettre en œuvre la commande comme indiqué ci-dessus, l'utilisateur doit indiquer les domaines énumérés ci-,

* destination dir
* template group

Autres paramètres
-----------------------------

Les autres paramètres de ce module, chacun pouvant être utilisés dans la déclaration est,

* Cleofy,
* cleofy

avantages
----------------

* Les paramètres utilisés déclarant aide et d'autres caractéristiques différentes de apt ne sont pas sensibles à la casse.
* Il est bien de choses à faire dans les deux cents os et ainsi que dans Ubuntu.
* Ce module enveloppe tous les besoins d'un projet dans la création ensemble standard de pilotes automatiques.

