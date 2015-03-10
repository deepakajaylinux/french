========
Drupal
========

Synopsis
------------

Drupal module est une partie de modules par défaut. Il fournit des pilotes automatiques pour Drupal, qui est adapté par builderfy et pilotes automatiques dapperfy. En plus de la builderfy et dapperfy, il fournit une configuration de base de données pour le module Drupal DB de configuration.

Drupal est un cadre de gestion de contenu libre et open-source écrit en PHP et distribué sous la GNU General Public License. Il est utilisé comme un cadre back-end pour au moins 2,1% de tous les sites Web dans le monde entier allant de blogs personnels, et à des sites gouvernementaux, entreprises et politiques, y compris WhiteHouse.gov data.gov.uk. Il est également utilisé pour la gestion des connaissances et la collaboration de l'entreprise.

Drupal fonctionne sur ne importe quelle plateforme de calcul qui prend en charge un serveur Web capable d'exécuter PHP (y compris Apache, LiteSpeed, IIS, Lighttpd, Hiawatha, Cherokee ou Nginx) et une base de données (telles que MySQL, MongoDB, MariaDB, PostgreSQL, SQLite, ou Microsoft SQL Server) pour stocker le contenu et les paramètres.

Voyons comment dapperfy l'drupal sous ces modules dans différents aspects.

Commande Aide
--------------------

La commande d'aide est une brève et ainsi que abstraite intéressante pour l'utilisateur. Il fournit des informations concernant son rôle majeur, les détails des autres paramètres qui peuvent être utilisés dans les déclarations, ses trois fonctions principales (builderfy, dapperfy, exécution), et également la syntaxe pour utiliser et déclarer ces trois fonctions intéressantes. La syntaxe utilisée pour déclarer option d'aide, est donnée ci-dessous.

.. code-block:: bash

		ptdeploy Drupal help



Après avoir saisi la commande donnée ci-dessus, l'utilisateur peut visualiser le résultat d'affichage des options d'aide ainsi que les détails décrits ci-dessus, vous pouvez visuellement obtenir ces résultats de l'option d'aide, comme indiqué dans la capture d'écran ci-dessous.

.. code-block:: bash

 kevell@corp:/# ptdeploy Drupal help
 ******************************


  This module is a Default Modules and provides autopilots for drupal tailored Builderfy and Dapperfy Autopilots.
  Also provides Drupal Database Configuration for the DBConfigure Module.

  Drupal, drupal

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Drupal.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy drupal --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************

Comment Dapperfy Drupal
--------------------------------
 
Voyons sur les différents aspects de ce module dans l'dapperfying drupal. La commande utilisée à cet effet est le même pour tous les aspects comme indiqué ci-dessous,

.. code-block:: bash

 		ptdeploy dapperfy drupal


Après être entré dans l'ordre donné ci-dessus, les détails suivants sont enquis lors de l'exécution comme illustré dans le tableau,

.. cssclass:: table-bordered

 +---------------------------+-------------------------------------+-------------+----------------------------------------------------+
 | paramètre                 | Autres paramètres                   | Option      | commentaires                                       |
 +===========================+=====================================+=============+====================================================+
 |Dapperfy This for Drupal?  | au lieu de Drupalnous pouvons       | Y(Yes)      | Si l'utilisateur doit dapperfy l'drupal qu'ils     |
 |(Y/N)	                     | utiliser, drupal aussi              |             | peuvent entrée comme Y.                            |
 +---------------------------+-------------------------------------+-------------+----------------------------------------------------+
 |Dapperfy This for Drupal?  | au lieu de Drupalnous pouvons       | N(No)       | Si l'utilisateur ne est pas dans le besoin à       |
 |(Y/N)	                     | utiliser, drupal aussi              |             | l'dapperfy drupal qu'ils peuvent entrée comme N.|  |
 +---------------------------+-------------------------------------+-------------+----------------------------------------------------+



Si l'utilisateur procède dapperfying l'drupal en inscrivant, Y, les étapes suivantes sont impliqués lors de l'exécution,

Etape 1:

Voulez-vous ajouter un autre environnement? (Y / N)

L'utilisateur dispose à l'entrée O ou N, en fonction de leur besoin d'ajouter un autre environnement.

Représentant de manière visuelle sur ce processus de dapperfying l'drupal La capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************


La deuxième forme de déclarer l'dapperfying de Drupal est expliqué ci-dessous, et la commande utilisée pour ce est la même que

.. code-block:: bash

	ptdeploy dapperfy drupal

Après être entré dans l'ordre donné ci-dessus, les détails suivants sont enquis lors de l'exécution comme illustré dans le tableau,

.. cssclass:: table-bordered

 +----------------------+-------------------------------------------+-------------+---------------------------------------------------------+
 | paramètre            | Autres paramètres                         | Option      | commentaires                                            |
 +======================+===========================================+=============+=========================================================+
 |Dapperfy This for     | au lieu de Drupalnous pouvons utiliser,   | Y(Yes)      | Si l'utilisateur doit dapperfy l'drupal qu'ils          |
 |Drupal? (Y/N)	        | drupal aussi                              |             | peuvent entrée comme Y.                                 |
 +----------------------+-------------------------------------------+-------------+---------------------------------------------------------+
 |Dapperfy This for     | au lieu de Drupalnous pouvons utiliser,   | N(No)       | Si l'utilisateur ne est pas dans le besoin à l'dapperfy |
 |Drupal? (Y/N)	        | drupal aussi                              |             | drupal qu'ils peuvent entrée comme N.                   |
 +----------------------+-------------------------------------------+-------------+---------------------------------------------------------+
 |Use existing          | au lieu de Drupalnous pouvons utiliser,   | Y(Yes)      | Si l'utilisateur souhaite procéder avec les paramètres  |
 |environment           | drupal aussi                              |             | d'environnement existantes qu'ils peuvent entrée        |
 |settings? (Y/N)       |                                           |             | comme Y.                                                |
 +----------------------+-------------------------------------------+-------------+---------------------------------------------------------+
 |Use existing          | au lieu de Drupalnous pouvons utiliser,   | N(No)       | Si l'utilisateur souhaite continuer avec les nouveaux   |
 |environment settings? | drupal aussi                              |             | paramètres de l'environnement qu'ils peuvent entrée     |
 |(Y/N)                 |                                           |             | comme N.|                                               |
 +----------------------+-------------------------------------------+-------------+---------------------------------------------------------+



Après l'achèvement des enquêtes indiquées ci-dessus, les étapes suivantes comme décrit exécuteront,

Etape 1:

Voulez-vous modifier les entrées applicables à ne importe quelle application dans l'environnement local par défaut (Y / N)

L'utilisateur dispose à l'entrée Y ou N.

Étape 2:

Environnement 1 défaut local:

Dans cette étape, la valeur de l'environnement et répertoire temp sont enquis et l'utilisateur ont pour les saisir.

Etape 3:

Entrez Serveurs-ce est un tableau d'entrées

Entrez cibler?

Entrez utilisateur?

Entrez le mot de passe?

L'utilisateur a demandé à l'entrée les données de.

Etape 4:

Ajouter un autre serveur? (Y / N)

L'utilisateur dispose à l'entrée Y ou N selon leur souhait.

Etape 5:

Voulez-vous modifier les entrées applicables à ne importe quelle application dans l'environnement local par défaut -0000 (Y / N)

L'utilisateur dispose à l'entrée Y ou N.

Etape 6:

Les paramètres de l'environnement peuvent être définies manuellement si nécessaire à des valeurs non-entrée par défaut.

Les données de ont demandé pendant l'exécution de l'application des paramètres sont définis comme ci-dessous,

Rapport Git repo URL

Rapport option clé SSH privée pour Git Repo.

Rapport Direction générale des douanes Git

Valeur pour Apache VHost URL

Valeur pour Apache VHost Nom d'hôte / IP

Valeur pour combien de révisions pour garder

Rapport Adresse IP DB

Rapport DB App Nom d'utilisateur

Rapport DB App User Pass

Etape 7:

Voulez-vous ajouter un autre environnement? (Y / N)

L'utilisateur dispose à l'entrée Y ou N en fonction de leurs besoins.

Donnera la capture d'écran ci-dessous une représentation picturale pour les étapes expliquées ci-dessus.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal

 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 Y
 Do you want to modify entries applicable to any app in environment default-local (Y/N) 
 Y
 Environment 1 default-local : 
 Default Settings for Any App not setup for environment default-local enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /root/gg
 Enter user ?
 root
 Enter password ?
 123
 Add Another Server? (Y/N)
 n
 Do you want to modify entries applicable to any app in environment default-local-8080 (Y/N) 
 n
 Settings for dapper not setup for environment default-local-8080 enter them manually.
 Environment 2 default-local-8080 : 
 Value for: Project Container directory, (inc slash)
 /root/vv
 Value for: Git Repo URL
 
 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch
 
 Value for: Apache VHost URL (Don't Include http://)
 
 Value for: Apache VHost Hostname/IP
 
 Value for: How many revisions to keep
 
 Value for: DB IP Address
 
 Value for: DB App User Name (Will be created if not existing)
 
 Value for: DB App User Pass
 
 Value for: DB Name (Will be created if not existing)
 
 Value for: DB Admin User Name
 
 Value for: DB Admin User Pass
 
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************
 
 
 Success
 In Dapperfy
 ******************************
 
 

La troisième forme d'exécution se explique par les étapes à venir. La commande est la même que

.. code-block:: bash

	ptdeploy dapperfy drupal


After entering the command given above, the following details are enquired during execution as depicted from the table,



.. cssclass:: table-bordered

 +--------------------------+-------------------------------------------+-------------+----------------------------------------------------+
 | paramètre                | Autres paramètres                         | Option      | commentaires                                       |
 +==========================+===========================================+=============+====================================================+
 |Dapperfy This for         | au lieu de Drupalnous pouvons utiliser,   | Y(Yes)      | Si l'utilisateur doit dapperfy l'drupal            |  
 |Drupal? (Y/N)	            | drupal aussi                              |             | qu'ils peuvent entrée comme Y.                     |
 +--------------------------+-------------------------------------------+-------------+----------------------------------------------------+
 |Dapperfy This for         | au lieu de Drupalnous pouvons utiliser,   | N(No)       | Si l'utilisateur ne est pas dans le besoin à       | 
 |Drupal? (Y/N)	            | drupal aussi                              |             | l'dapperfy drupal qu'ils peuvent entrée comme N.   | 
 +--------------------------+-------------------------------------------+-------------+----------------------------------------------------+ 
 |Use existing environment  | au lieu de Drupalnous pouvons utiliser,   | Y(Yes)      | Si l'utilisateur souhaite procéder avec les        |
 |settings? (Y/N)           | drupal aussi                              |             | paramètres d'environnement existantes qu'ils       |
 |                          |                                           |             | entrée comme Y.                                    |
 +--------------------------+-------------------------------------------+-------------+----------------------------------------------------+
 |Use existing environment  | au lieu de Drupalnous pouvons utiliser,   | N(No)       | Si l'utilisateur souhaite continuer avec les       |
 |settings? (Y/N)           | drupal aussi                              |             | nouveaux paramètres de l'environnement qu'ils      |
 |                          |                                           |             | peuvent entrée comme N.|                           |
 +--------------------------+-------------------------------------------+-------------+----------------------------------------------------+



Après l'achèvement des enquêtes indiquées ci-dessus, les étapes suivantes comme décrit exécuteront,

Etape 1:

Voulez-vous ajouter un autre environnement paramètres? (Y / N)

L'utilisateur dispose à l'entrée Y ou N.

Étape 2:

Environnement 3 défaut local:

Dans cette étape, la valeur de l'environnement et répertoire temp sont enquis et l'utilisateur ont pour les saisir.

Les paramètres de l'environnement peuvent être définies manuellement si nécessaire à des valeurs non-entrée par défaut.

Les données de ont demandé pendant l'exécution de l'application des paramètres sont définis comme ci-dessous,

Rapport Directory Project Container.

Rapport Git repo URL

Rapport option clé SSH privée pour Git Repo.

Rapport Direction générale des douanes Git

Valeur pour Apache VHost URL

Valeur pour Apache VHost Nom d'hôte / IP

Valeur pour combien de révisions pour garder

Rapport Adresse IP DB

Rapport DB App Nom d'utilisateur

Rapport DB App User Pass

Donnera la capture d'écran ci-dessous une représentation picturale pour les étapes expliquées ci-dessus.


.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 y
 Environment 3  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Value for: Project Container directory, (inc slash)

 Value for: Git Repo URL

 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch

 Value for: Apache VHost URL (Don't Include http://)

 Value for: Apache VHost Hostname/IP

 Value for: How many revisions to keep

 Value for: DB IP Address

 Value for: DB App User Name (Will be created if not existing)

 Value for: DB App User Pass

 Value for: DB Name (Will be created if not existing)

 Value for: DB Admin User Name

 Value for: DB Admin User Pass

 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************



Le quatrième type de dapperfying Drupal est expliqué ci-dessous, et la commande utilisée est la même que

.. code-block:: bash

	ptdeploy dapperfy drupal

Après être entré dans l'ordre donné ci-dessus, les détails suivants sont enquis lors de l'exécution comme illustré dans le tableau,

.. cssclass:: table-bordered

 +-------------------------+---------------------------------------+-------------+----------------------------------------------------+
 | paramètre               | Autres paramètres                     | Option      | commentaires                                       |
 +=========================+=======================================+=============+====================================================+
 |Dapperfy This for        | au lieu de Drupalnous pouvons         | Y(Yes)      | Si l'utilisateur doit dapperfy l'drupal qu'ils     | 
 |Drupal? (Y/N)	           | utiliser, drupal aussi                |             | peuvent entrée comme Y.                            |
 +-------------------------+---------------------------------------+-------------+----------------------------------------------------+
 |Dapperfy This for        | au lieu de Drupalnous pouvons         | N(No)       | Si l'utilisateur ne est pas dans le besoin à       |
 |Drupal? (Y/N)	           | utiliser, drupal aussi                |             | l'dapperfy drupal qu'ils peuvent entrée comme N.   |
 +-------------------------+---------------------------------------+-------------+----------------------------------------------------+
 |Use existing environment | au lieu de Drupalnous pouvons         | Y(Yes)      | Si l'utilisateur souhaite procéder avec les        |
 |settings? (Y/N)          | utiliser, drupal aussi                |             | paramètres d'environnement existantes qu'ils       |
 |                         |                                       |             | peuvent entrée comme Y.                            |
 +-------------------------+---------------------------------------+-------------+----------------------------------------------------+
 |Use existing environment | au lieu de Drupalnous pouvons         | N(No)       | Si l'utilisateur souhaite procéder avec les        |
 |settings? (Y/N)          | utiliser, drupal aussi                |             | nouveaux paramètres de l'environnement qu'ils      |
 |                         |                                       |             | peuvent entrée comme N.|                           |
 +-------------------------+---------------------------------------+-------------+----------------------------------------------------+

 

Si l'utilisateur procède dapperfying l'drupal en inscrivant, Y, les étapes suivantes sont impliqués lors de l'exécution,

Etape 1:

Voulez-vous ajouter un autre environnement? (Y / N)

L'utilisateur dispose à l'entrée O ou N, en fonction de leur besoin d'ajouter un autre environnement.

Représentant de manière visuelle sur ce processus de dapperfying l'drupal La capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************



avantages
-----------

* Il est bien de choses à faire dans les deux Ubuntu et ainsi que dans cent OS.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse.
* Les paramètres de l'environnement peuvent être définies lors de l'exécution de la dapperfying.
