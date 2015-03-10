===========================
ApacheVHostEditor
===========================

synopsis
------------------

Apache hôtes virtuels sont utilisés pour exécuter plus d'un domaine hors d'une adresse IP unique. Ceci est particulièrement utile pour les personnes qui ont besoin de gérer les fonctions de vhost apache. Les sites présentent des informations différentes aux visiteurs, selon qui les utilisateurs ont accédé au site. Il n'y a pas de limite au nombre d'hôtes virtuels qui peuvent être ajoutés à un Virtual Private Server (VPS) .Cet peut être adapté pour Ubuntu et CentOS.

Commande Aide
-----------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules Apache virtualhost de l'éditeur. Les listes de commandes de l'aide sur les autres paramètres d'Apache éditeur de virtualhost
le cadre du module ptdeploy. Il décrit également la syntaxe pour l'installation du usera de updation. La commande d'aide pour apache éditeur de virtualhost est illustré ci-dessous.

.. code-block:: bash

		ptdeploy Apache virtualhost editor help

La capture d'écran ci-dessous montre l'effort complète d'Apache éditeur de virtualhost.

.. code-block:: bash


 kevell@corp:/# ptdeploy ApacheVHostEditor help
 ******************************


  This command is part of Default Modules and handles Apache VHosts Functions.

  ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted

          - add
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - add-balancer
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com

          - list
          List current Virtual Hosts
          example: ptdeploy vhe list

          - enable
          enable a Server Block
          example: ptdeploy vhe enable

          - disable
          disable a Server Block
          example: ptdeploy vhe disable

 ------------------------------
 End Help
 ******************************

paramètres alternatifs
-----------------------------------

Voici les autres paramètres qui peuvent être définis dans les déclarations:

ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted.

ajouter
----------

Cette commande permet de créer un hôte virtuel. Primordial est possible. La commande suivante peut être adoptée pour la création d'un éditeur d'hôte virtuel.

.. code-block:: bash

		sudo ptdeploy vhe add

après la saisie de la commande ci-dessus, il peut poser la question suivante,

Le document Vhe racine, extension de fichier Vhe, commande apache Vhe, Port IP Vhe, Vhe Annuaire Vhost, Vhe modèle, Vhe défaut nom du modèle.

L'utilisateur doit saisir tous les détails, un par un ENTRER contraire dans la ligne de commande lui-même. La capture d'écran ci-dessous explique à ce sujet

.. code-block:: bash


 - add
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates



Add Balancer
---------------------

Cette commande permet de créer un hôte virtuel. Primordial est possible. Il ya deux façons d'entrer dans l'entrée. De manière simple l'utilisateur peut donner VHE add. La seconde manière avec le nom de chemin commande hôte peut être mentionné. La commande suivante peut être adoptée pour la création d'un éditeur d'hôte virtuel.

.. code-block:: bash

		sudo ptdeploy vhe add

après la saisie de la commande ci-dessus, il peut poser la question suivante,

Le document Vhe racine, extension de fichier Vhe, commande apache Vhe, Port IP Vhe, Vhe Annuaire Vhost, Vhe modèle, Vhe défaut nom du modèle.

L'utilisateur doit saisir tous les détails, un par un autre ENTRER tout dans la ligne de commande lui-même. La capture d'écran ci-dessous 
explique à ce sujet

.. code-block:: bash

 - add-balancer
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates


supprimer
-------------

Cette commande permet de supprimer un serveur virtuel particulier. Il ya deux façons d'entrer dans l'entrée. De manière simple l'utilisateur peut donner VHE remove (rm). La seconde manière avec le nom de chemin commande hôte peut être mentionné. La commande suivante est utilisée pour supprimer le nom d'hôte.

.. code-block:: bash

	        ptdeploy vhe rm

La capture d'écran suivante montre la fonction de rm.

.. code-block:: bash

 - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com

liste
--------

Cette commande permet de lister les hôtes virtuels actuels. La commande suivante permet de lister les hôtes virtuels.

.. code-block:: bash

		ptdeploy vhe list

La capture d'écran montre la fonction de liste.

.. code-block:: bash

 - list
          List current Virtual Hosts
          example: ptdeploy vhe list


permettre
-----------

Boot sécurisé est une fonction conçue pour empêcher les logiciels malveillants et les médias non autorisée de chargement pendant le processus de démarrage. Cette option permettra activé le bloc de serveur. Dans hôte virtuel lorsque l'occasion tapé la commande suivante,

.. code-block:: bash
   
                ptdeploy vhe enable

Cette option est activée par défaut. Cette option permet au serveur d'hôte virtuel permet.

Module Aider à développer un grand nombre de capacités habilitantes nécessaires à l'entretien des environnements haute performance grâce à notre compréhension des interdépendances entre les personnes, les processus et la technologie. La capture d'écran ci-dessous explique la même chose.

.. code-block:: bash

 - enable
          enable a Server Block
          example: ptdeploy vhe enable



désactiver
-------------

Cette désactivation utilisée pour désactiver le serveur. Les connexions inactives ou ralenti éditeur hôte virtuel sont normalement déconnectés par le serveur après une certaine période de temps. La commande suivante permet de désactiver l'éditeur d'hôte virtuel.

.. code-block:: bash
   
                ptdeploy vhe disable

Après avoir tapé cette commande, il peut demander à l'utilisateur de désactiver le serveur. Si les entrées de l'utilisateur que oui il désactiver le serveur est à dire qu'il Wona € ™ t permettent tout organisme de travailler dans ce serveur.

La capture d'écran suivante visualiser évidemment.

.. code-block:: bash

 - disable
          disable a Server Block
          example: ptdeploy vhe disable



avantages
---------------

* Multi utilisateur peut accéder à la fois.
* L'utilisateur peut ajouter ou supprimer des hôtes virtuels.
* L'éditeur de l'hôte virtuel peut activer ou désactiver l'hôte virtuel selon le souhait de l'usera € ™.
* Sensibilité non de cas.
* Eh bien-to-do dans Ubuntu et CentOS.


