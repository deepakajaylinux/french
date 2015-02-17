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

	cleopatra cleofy help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu cleofy.

.. code-block:: bash


 kevell@corp:/# cleopatra cleofy help

 ******************************


 This command is part of a default Module Core and provides you with a method by which you can create a standard set of Autopilot files for your project from the command line.  


 Cleofy, cleofy  

 - list        
 	List all of the autopilot files in your build/config/cleopatra/autopilots        
	example: cleopatra cleofy list        

 - standard        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for your project.        
	example: cleopatra cleofy standard        

 - tiny        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "tiny" style infrastructure.        	example: cleopatra cleofy tiny        

 - medium        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "medium" style infrastructure.        	example: cleopatra cleofy medium        

 - medium-web        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "medium" style infrastructure,
        with web but not database.        
 	example: cleopatra cleofy medium-web        

 - db-cluster        

	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for your project.        
 	example: cleopatra cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

 - install-generic-autopilots        
	Install the generic Cleofy autopilot templates for a Tiny or Medium (Current Default) set of Environments        
 example: cleopatra cleofy install-generic-autopilots        
	example: cleopatra cleofy install-generic-autopilots        
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/cleopatra/cleofy/autopilots/                    
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

Cette fonction vise à la liste de tous les fichiers du pilote automatique dans votre emplacement spécifié (build / config / Cléopâtre / pilotes automatiques). La syntaxe pour appliquer cette fonction est illustré ci-dessous,

.. code-block:: bash

	cleopatra cleofy list

standard
------------

Cette fonction contribue à la création d'un ensemble par défaut de pilotes automatiques de Cléopâtre (dans build / config / Cléopâtre / de pilotes automatiques) pour le projet des utilisateurs. Cette fonction peut être appliquée en utilisant simplement la commande ci-dessous,

.. code-block:: bash

	cleopatra cleofy standard

minuscule
---------------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de Cléopâtre (dans build / config / Cléopâtre / de pilotes automatiques) pour un projet avec petite infrastructure. Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	cleopatra cleofy tiny

moyen
-----------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de Cléopâtre (dans build / config / Cléopâtre / de pilotes automatiques) pour un projet d'infrastructures moyenne. Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	cleopatra cleofy medium

Medium_Web
---------------------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de Cléopâtre (dans build / config / Cléopâtre / de pilotes automatiques) pour un projet avec le milieu avec l'infrastructure Web, mais pas la base de données. Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	cleopatra cleofy medium-web

DB_cluster
---------------

Cette fonction vise à créer un ensemble par défaut de pilotes automatiques de Cléopâtre (dans build / config / Cléopâtre / de pilotes automatiques) pour le projet de l'utilisateur.
Pour mettre en œuvre cette fonction utilisez la commande suivante comme ci-dessous,

.. code-block:: bash

	cleopatra cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

Install_generic_autopilots
-------------------------------------

Cette fonction aide à l'installation de modèles de pilote automatique génériques pour petit ou moyen ensemble de l'environnement en utilisant simplement la commande comme donnée
dessous

.. code-block:: bash
	
	cleopatra cleofy install-generic-autopilots        
Or,

.. code-block:: bash

	cleopatra cleofy install-generic-autopilots
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/cleopatra/cleofy/autopilots/                    
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
