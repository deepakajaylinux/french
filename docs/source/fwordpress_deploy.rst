============
Wordpress
============

Synopsis
-----------

Ce module est une partie fine de la une par défaut, ce qui facilite les utilisateurs à intégrer les sites de presse de mots. Ses fonctions comprennent dapperfy, builderfy, et fournit également la configuration de base de données de presse de mot pour le module DBConfigure.

Word Press est un outil de blogging gratuit et open-source et un système de gestion de contenu (CMS) basé sur PHP et MySQL. Les caractéristiques comprennent une architecture de plug-in et un système de template. Word Press a été utilisé par plus de 23,3% des 10 millions de sites top à partir de Janvier 2015. Word Press est le système de blogs la plus populaire dans l'utilisation sur le Web, à plus de 60 millions de sites Web.

Commande Aide
-------------------

La commande d'aide explique les utilisateurs concernant la fonction principale de ce module, ses paramètres alternatifs qui peuvent être utilisés dans les déclarations, ses trois grandes fonctions (ex: dapperfy, builderfy, exécution), et aussi sur la syntaxe pour déclarer ses trois fonctions principales. La commande utilisée pour déclarer l'option d'aide est illustré ci-dessous,

.. code-block:: bash

		ptdeploy Wordpress help


La capture d'écran ci-dessous illustre visuellement ce qui concerne la commande d'aide en vertu de ce module. La syntaxe utilisée dans la déclaration ne est pas sensible à la casse.

.. code-block:: bash

 kevell@corp:/# ptdeploy Wordpress help
 ******************************


  This module is a Default one, and provides integration for Wordpress websites. It has tailored Builderfy and Dapperfy
  Autopilots and also provides Wordpress Database Configuration for the DBConfigure Module.

  Wordpress, wordpress

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Wordpress.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy wordpress --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************



Comment utiliser dapperfy wordpress
--------------------------------------

La commande utilisée pour dapperfy l'wordpress est donnée ci-dessous,

.. code-block:: bash

		ptdeploy dapperfy wordpress


Après être entré dans l'ordre donné ci-dessus, le processus de dapperfying commence comme illustré dans le tableau ci-dessous,

.. cssclass:: table-bordered


 +---------------------------+-----------------------------------------+----------+---------------------------------------------+
 | Paramètres                | Autres paramètres                       | options  | Commentaires                                |
 +===========================+=========================================+==========+=============================================+
 |Dapperfy This for          | Au lieu de wordpress, nous pouvons      | Y(Yes)   | Si l'utilisateur doit dapperfy l'wordpress  |
 |Wordpress? (Y/N)           | utiliser Wordpress aussi.               |          | ils peuvent entrée comme Y.                 |
 +---------------------------+-----------------------------------------+----------+---------------------------------------------+
 |Dapperfy This for          | Au lieu de wordpress, nous pouvons      | N(No)    | Si l'utilisateur ne est pas dans le besoin  |
 |Wordpress? (Y/N)           | utiliser Wordpress aussi.               |          | à l'dapperfy wordpress ils peuvent entrée   |
 |                           |                                         |          | comme N.|                                   |
 +---------------------------+-----------------------------------------+----------+---------------------------------------------+
 

Si l'utilisateur procède le processus de dapperfying l'wordpress, pendant l'exécution de dapperfying les étapes suivantes se produit,

Etape 1:

Utilisez les paramètres d'environnement existantes? (Y / N)

L'utilisateur doit indiquer Y ou N, selon leur souhait pour l'utilisation de paramètres d'environnement existants.

Étape 2:

Voulez-vous ajouter un autre environnement? (Y / N)

L'utilisateur doit indiquer Y ou N, selon leur souhait pour ajouter un autre environnement.

Après l'achèvement de ces étapes, le processus de l'dapperfying wordpress se rempli. Il est représenté visuellement à partir de la capture d'écran ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy wordpress
 Dapperfy This for Wordpress? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 
 
 Success
 In Dapperfy
 ******************************
 

Travailler de WordPress Auto déployer les fichiers
-------------------------------------------------------

Afin de générer l'auto déployer fichiers dans wordpress, l'utilisateur doit entrer la commande ci-dessous,

.. code-block:: bash

		ptdeploy dapperfy wordpress --yes --guess

Après être entré dans l'ordre donné ci-dessus, l'Auto Deploy fichiers seront générés, comme représenté imagée de la capture d'écran ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy wordpress --yes --guess
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 

 Success
 In Dapperfy
 ******************************


avantages
----------

* Il est bien de choses à faire dans les deux Ubuntu et ainsi que dans cent OS.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse.
* Word Press propose également la gestion de la liaison intégrée; , structure de permalien propre un moteur de recherche convivial
* Il a la capacité d'affecter plusieurs catégories aux articles; et de soutenir pour le marquage des postes et des articles.
* Dans wordpress filtres automatiques sont également inclus, fournissant un formatage standard et le style de texte dans des articles

