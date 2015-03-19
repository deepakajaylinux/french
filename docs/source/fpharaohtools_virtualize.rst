=============
PharaohTools
=============

synopsis
------------

Le module outil de Pharaon aide à installer ptdeploy, pttest, Jrush, génération de rapports ptvirtualize. Il facilite les utilisateurs pour s'assurer de la disponibilité avant les aménagements. Manque seulement les modules peut être installé spécifiquement.


Commande Aide
---------------------

La commande help guide les utilisateurs sur la façon de rendre l'utilisation de ce module particulier sous ptvirtualize.
Il également les sensibiliser les options qui peuvent être effectuées sur ce module spécifique.
Il énumère les aboutissants des paramètres alternatifs ainsi que la syntaxe pour l'installation des outils de Pharaon.
La commande pour l'utilisation de l'option d'aide est indiquée ci-dessous,


.. code-block:: bash

	ptvirtualize pharaoh-tools help


La page-écran comme indiqué ci-dessous vous donne une représentation picturale au sujet de l'utilisation de la commande help.


.. code-block:: bash


installation
--------------

Le module outil de Pharaon agit comme un itinéraire plus court qui enveloppe l'installation de ptdeploy, pttest, Jrush. S'il manque parmi les trois tout un module particulier, le module spécifique seul sera installé qui est un atout supplémentaire. Le processus de s'assurer que joue un rôle important en saisissant des données sur la disponibilité des modules.

La commande utilisée pour la procédure d'installation sous le pharaon outil est donnée ci-dessous,


.. code-block:: bash

	ptvirtualize pharaoh-tools install

Après avoir entré la commande ci-dessus, le processus d'installation commence à s'exécuter et procède de la manière suivante, comme l'illustre le tableau, de



.. cssclass:: table-bordered

 +---------------------------------+------------------------------+--------------------------------------------------------+
 | paramètres			   | Options d'entrée disponibles | commentaires					   |
 +=================================+==============================+========================================================+
 |Install Pharaoh Tools? (Y/N)     | Y(Yes)		          | Si l'utilisateur souhaite continuer avec le processus  |
 |				   | 			          | d'installation , ils peuvent entrée comme Y            |
 +---------------------------------+------------------------------+--------------------------------------------------------+
 |Install Pharaoh Tools? (Y/N)	   | N(No)		          | Si l'utilisateur souhaite quitter le processus         |
 |				   |			          | d'installation , ils peuvent cesser de fumer           |
 |                                 |                              | en utilisant simplement N|                             |
 +---------------------------------+------------------------------+--------------------------------------------------------+

Lors de l'installation le pharaon outil l'étapes suivantes a lieu :


Ensure
----------

* L'outil Pharaon assure les modules disponibles. 
* Tout en veillant, il ne sera pas vérifier sur les versions.


ptdeploy
------------------

* Le module ptdeploy se signale comme installé, dans le cas d'existence.  * Il contrôle en outre la version de module ptdeploy. 
* Si le module ptdeploy n'est pas disponible dans la machine, puis automatiquement ptdeploy va progresser pour installer.

pttest
------------------

* Après l'achèvement de l'installation de ptdeploy, elle assurera le module pttest.  
* Le module pttest se signale comme installé, dans le cas d'existence. 
* Si le module pttest n'est pas disponible dans la machine, puis automatiquement pttest va progresser pour installer.


Jrush
--------

* Après l'achèvement de l'installation de pttest, elle assurera le module Jrush. 
* Le module Jrush se signale comme installé, dans le cas d'existence.  
* Si le module Jrush n'est pas disponible dans la machine, puis automatiquement Jrush va progresser pour installer. 
* Si tous les trois modules existent déjà, puis il affiche message exceptionnel tel qu'indiqué dans la capture d'écran ci-dessous..

options supplémentaires
-------------------------

Lors de l'installation ptdeploy, pttest, Jrush, les options suivantes sont exigées comme entrée de l'utilisateur. Nous verrons, les options supplémentaires qui peuvent être spécifiées par les utilisateurs, s'ils le souhaitent, est représenté sous forme de tableau comme indiqué ci-dessous.




.. cssclass:: table-bordered

 +----------------------------+-------------------------------------------+----------------+------------------------------------------------+
 | paramètres		      | chemin					  | option	   | commentaire		  		    |
 +============================+===========================================+================+================================================+
 |Program data directory      | "/opt/pttest(corresponding module)"       | Yes		   | Si l'utilisateur de procéder installation avec |
 |(Default)		      | 					  |		   | le répertoire de données par défaut du         |
 |			      |						  |		   | programme qu'ils peuvent entrée comme Oui      |
 +----------------------------+-------------------------------------------+----------------+------------------------------------------------+
 |Program data directory      | User specific				  | No(End slash)  | Si l'utilisateur souhaite procéder à leur      |
 |			      |						  |		   | propre répertoire de données de programme,     |
 |			      |						  |		   | ils peuvent entrée comme N , et dans la        |
 |                            |                                           |                | main indiquer qu'ils possèdent emplacement.    |
 +----------------------------+-------------------------------------------+----------------+------------------------------------------------+
 |Program executor directory  | "/usr/bin"			          | Yes		   | Si l'utilisateur de procéder installation      |
 |(Default)		      |						  |		   | avec le répertoire programme d' exécuteur      |
 |			      | 				          |		   | défaut qu'ils peuvent entrée comme Oui         |
 +----------------------------+-------------------------------------------+----------------+------------------------------------------------+
 |Program executor directory  | User specific				  | No(End slash)  | Si l'utilisateur souhaite procéder à leur      |
 |			      |						  |		   | propre répertoire programme d' exécuteur       |
 |			      |						  |		   | testamentaire, ils peuvent entrée comme N ,    |
 |			      |						  | 		   | et dans la main indiquer qu'ils possèdent      |
 |                            |                                           |                | emplacement.|                                  |
 +----------------------------+-------------------------------------------+----------------+------------------------------------------------+



Alors que l'installation il précisera l'emplacement du git clone, affiche le nombre d'objets, recevoir des objets, résoudre les deltas, connectivité.


La capture d'écran suivante vous explique graphiquement le processus impliqué dans l'installation de l'outil de Pharaon.



.. code-block:: bash


Avantages
-----------

* Elle facilite aux utilisateurs de s'assurer avant l'installation. 
* Dans le cas d'un module particulier est manquant, l'utilisateur peut procéder à l'installation de ce module particulier seul. 
* L'utilisateur peut spécifier leur propre chemin d'accès ou l'emplacement de répertoire de données de programme et le répertoire de 
  l'exécuteur testamentaire. 
* Si un module particulier existe déjà dans la machine, l'outil d'installation lèvera un message d'exception car il est déjà installé. 
* Elle évite le surgravage indésirables des modules, il est donc temps de sauver.


