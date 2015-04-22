==========
Joomla
==========

Synopsis
----------------

Joomla fournit site d'intégration. De nombreux services d'hébergement Web offrent un simple clic installer, obtenir l'utilisateur nouveau site opérationnel en quelques minutes.

Y compris sa facilité d'utilisation et l'extensibilité, ont fait de Joomla logiciel le plus populaire du site Web. Le meilleur de tous, Pilote automatique, builderfy et dapperfy sont disponibles dans ptdeploy et fait une meilleure solution. Ce est à l'aise avec Ubuntu et Cent OS.

Commande Aide
------------------------

Cette commande help guide l'utilisateur pour fournir une intégration pour Joomla. Il a personnalisé Pilote automatique, builderfy et dapperfy sont disponibles dans ptdeploy Propecia peut aussi fournit une configuration de base de données pour le module de configuration db.

La commande d'aide pour Oracle est indiqué ci-dessous.

.. code-block:: bash

		ptdeploy joomla help

Après les entrées de commande ci-dessus, il commence à fonctionner à intégrer site joomla. Il catéchèse les fonctions de joomla dans les captures d'écran.

.. code-block:: bash

 kevell@corp:/# ptdeploy Joomla help
 ******************************


  This module is a Default one, and provides integration for Joomla websites. It has tailored Builderfy and Dapperfy
  Autopilots and also provides Joomla Database Configuration for the DBConfigure Module.

  Joomla, joomla

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Joomla.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy joomla --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************



Dapperfy
---------------

Ce dapperfy utilisé pour créer l'utilisateur Auto Deploy fichiers. Dapperfy peut travailler pour un grand nombre de projets sans configurations complexes avec quelques minutes d'une valeur de mise en place. Utilisation Dapperfy est très rapide, et ce est probablement le meilleur point de départ, même pour les configurations complexes que l'utilisateur peut toujours juste modifier les fichiers après avec leurs propres personnalisations. La commande suivante utilisée pour dapperfy.

.. code-block:: bash

		ptdeploy dapperfy joomla


Après entrée comme ci-dessus ladite commande il demande dapperfy exécution il montre la capture d'écran.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy joomla
 Dapperfy This for Joomla? (Y/N) 
 Y
 Do you want to add another environment? (Y/N) 
 n
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 

 Success
 In Dapperfy
 ******************************

Builderfy
--------------

Il crée des modèles à installer construction. L'utilisateur peut ajouter d'autres modèles. Lorsque nous apportons des changements à l'utilisateur référentiel, le déploiement d'une nouvelle version à la Production d'utilisateur cible. La commande utilisée pour builderfy est la suivante,

.. code-block:: bash

		ptdeploy builderfy continuous-joomla

La capture d'écran ci-dessous explique sa fonction.

.. code-block:: bash


 kevell@corp:/# ptdeploy builderfy continuous-joomla
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this?

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the Continuous Delivery build for My Project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot test environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Success
 In Builderfy
 ******************************



exécuter
------------

Ce processus exécuter le pilote automatique créateur de construction. Accès rapide est possible. La commande pour l'exécution comme suit,

.. code-block:: bash

		ptdeploy autopilot execute

La capture d'écran suivante expliquer ses fonctions.

.. code-block:: bash



Option
------------

.. cssclass:: table-bordered

 +-------------------------+---------------------+-----------+---------------------------------------------------------+
 | paramètre               | Autres paramètres   | Option    | commentaires                                            |
 +=========================+=====================+===========+=========================================================+
 |Dapperfy this for        | Joomla, joomla      | Y(Yes)    | Si l'utilisateur souhaite continuer dapperfying qu'ils  |           
 |joomla? (Y/N)            |                     |           | peuvent entrée comme Y.                                 |
 +-------------------------+---------------------+-----------+---------------------------------------------------------+
 |Dapperfy this for        | Joomla, joomla      | N(No)     | Si l'utilisateur souhait de quitter dapperfying         |
 |joomla? (Y/N)            |                     |           | qu'ils peuvent entrée comme N                           |
 +-------------------------+---------------------+-----------+---------------------------------------------------------+
 |Do you want to add       | Joomla, joomla      | Y(Yes)    | Si l'utilisateur souhaitez ajouter nouvel environnement |
 |another environment?     |                     |           | qu'ils peuvent entrée comme Y                           |
 |(Y/N)                    |                     |           |                                                         |
 +-------------------------+---------------------+-----------+---------------------------------------------------------+
 |Do you want to add       | Joomla, joomla      | N(No)     | Si l'utilisateur n'a pas besoin d'ajouter un nouvel     |
 |another environment?     |                     |           | environnement qu'ils peuvent entrée comme N             |
 |(Y/N)|                   |                     |           |                                                         |
 +-------------------------+---------------------+-----------+---------------------------------------------------------+


avantages
------------

* Soutien Eh bien pour les professionnels
* Processus multilingue
* Mise à niveau facile
* Le dispositif de système Speedy
* Non sensible à la casse
* Convient pour Ubuntu et Cent OS.


Le Joomla se ouvre un tout nouveau monde d'expression car elle vous la liberté d'utiliser font que la conception rêve devenu réalité utilisateur permet!
