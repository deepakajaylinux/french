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


 kevell@corp:/# ptdeploy vhe add 
 
 Do you want to add a VHost? (Y/N) 
 y 
 What's the document root? Enter nothing for /home/karunakaran 

 What URL do you want to add as server name? 
 kumar 
 What IP:Port should be set? Enter nothing for 127.0.0.1:80 

 What File Extension should be used? Enter nothing for None (probably .conf on this system) 

 What is your VHost Template directory? Enter nothing for default templates 

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: --- 
 (0) docroot-no-suffix 
 (1) docroot-src-suffix 
 (2) docroot-web-suffix 
 (3) docroot-www-suffix 
 (4) docroot-docroot-suffix 

 0 
 Please check VHost: NameVirtualHost 127.0.0.1:80 
 <VirtualHost 127.0.0.1:80> 
	ServerAdmin webmaster@localhost 
	ServerName kumar 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Is this Okay? (Y/N) 
 y 
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Enabling site kumar. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite kumar.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************


.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.murali.com --vhe-file-ext=".conf" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*" 

 *template data* 

 Assuming Okay due to yes parameter 
 Enabling site www.murali.com. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite www.murali.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add --yes --guess --vhe-url=www.kkkkkkkkk.com 

 What is your VHost Template directory? Enter nothing for default templates 

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: --- 
 (0) docroot-no-suffix 
 (1) docroot-src-suffix 
 (2) docroot-web-suffix 
 (3) docroot-www-suffix 
 (4) docroot-docroot-suffix 

 0 
 NameVirtualHost 127.0.0.1:80 
 <VirtualHost 127.0.0.1:80> 
 	ServerAdmin webmaster@localhost 
	ServerName www.kkkkkkkkk.com 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Assuming Okay due to yes parameter 
 Enabling site www.kkkkkkkkk.com. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite www.kkkkkkkkk.com done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************



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


 kevell@corp:/# ptdeploy vhe rm 

 Do you want to delete VHost/s? (Y/N) 
 y 
 Deleting vhost 
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 
 
 14 
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Site www.siva.com disabled. 
 To activate the new configuration, you need to run: 
   service apache2 reload 
 a2dissite www.siva.com.conf done 
 VHost www.siva.com.conf Deleted  if existed 
 ****************************** 
 
 1Apache VHost Editor Finished 
 ****************************** 
 
.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm --yes --

 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) ddddddd.conf
 (2) default-ssl.conf
 (3) default-ssl.dpkg-remove
 (4) default.dpkg-remove
 (5) karuna
 (6) kumar.conf
 (7) llllllllllllll.conf
 (8) mmmmmm.conf
 (9) ptbuild.conf
 (10) testrepo.conf
 (11) www.dae.com.conf
 (12) www.dave.com
 (13) www.google.com
 (14) www.kkkkkkkkk.com.conf
 (15) www.murali.com.conf
 
 14
 Site www.kkkkkkkkk.com already disabled
 a2dissite www.kkkkkkkkk.com.conf done
 VHost www.kkkkkkkkk.com.conf Deleted  if existed
 ******************************
 
 1Apache VHost Editor Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.da.com.conf

 Deleting vhost
 Site www.da.com disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite www.da.com.conf done
 VHost www.da.com.conf Deleted  if existed
 ******************************


 1Apache VHost Editor Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.dae.com.conf

 Deleting vhost
 Site www.dae.com disabled.
 To activate the new configuration, you need to run:
   service apache2 reload
 a2dissite www.dae.com.conf done
 VHost www.dae.com.conf Deleted  if existed
 ******************************
 
 1Apache VHost Editor Finished
 ******************************





liste
--------

Cette commande permet de lister les hôtes virtuels actuels. La commande suivante permet de lister les hôtes virtuels.

.. code-block:: bash

		ptdeploy vhe list

La capture d'écran montre la fonction de liste.

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe list 

 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 You have a sites available dir, so also listing available sites. 
 Current Installed VHosts: 
 --- Enabled Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 
 --- All Available Virtual Hosts: --- 
 (16) 000-default.conf 
 (17) ddddddd.conf 
 (18) default-ssl.conf 
 (19) default-ssl.dpkg-remove 
 (20) default.dpkg-remove 
 (21) karuna 
 (22) kumar.conf 
 (23) llllllllllllll.conf 
 (24) mmmmmm.conf 
 (25) ptbuild.conf 
 (26) www.dave.com 
 (27) www.google.com 
 (28) www.kkkkkkkkk.com.conf 
 (29) www.murali.com.conf 
 (30) www.siva.com.conf 
 (31) www.siva1.com 
 ****************************** 
 
 1Apache VHost Editor Finished 
 ****************************** 
 




permettre
-----------

Boot sécurisé est une fonction conçue pour empêcher les logiciels malveillants et les médias non autorisée de chargement pendant le processus de démarrage. Cette option permettra activé le bloc de serveur. Dans hôte virtuel lorsque l'occasion tapé la commande suivante,

.. code-block:: bash
   
                ptdeploy vhe enable

Cette option est activée par défaut. Cette option permet au serveur d'hôte virtuel permet.

Module Aider à développer un grand nombre de capacités habilitantes nécessaires à l'entretien des environnements haute performance grâce à notre compréhension des interdépendances entre les personnes, les processus et la technologie. La capture d'écran ci-dessous explique la même chose.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe enable 

 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 

 7 
 Enabling site llllllllllllll. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite llllllllllllll.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 



désactiver
-------------

Cette désactivation utilisée pour désactiver le serveur. Les connexions inactives ou ralenti éditeur hôte virtuel sont normalement déconnectés par le serveur après une certaine période de temps. La commande suivante permet de désactiver l'éditeur d'hôte virtuel.

.. code-block:: bash
   
                ptdeploy vhe disable

Après avoir tapé cette commande, il peut demander à l'utilisateur de désactiver le serveur. Si les entrées de l'utilisateur que oui il désactiver le serveur est à dire qu'il Wona € ™ t permettent tout organisme de travailler dans ce serveur.

La capture d'écran suivante visualiser évidemment.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe disable 

 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) default-ssl.conf 
 (2) default-ssl.dpkg-remove 
 (3) default.dpkg-remove 
 (4) karuna 
 (5) kumar.conf 
 (6) ptbuild.conf 
 (7) www.dave.com 
 (8) www.google.com 
 (9) www.kkkkkkkkk.com.conf 
 (10) www.murali.com.conf 
 (11) www.siva.com.conf 
 (12) www.siva1.com 

 9 
 Site www.kkkkkkkkk.com disabled. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2dissite www.kkkkkkkkk.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 



avantages
---------------

* Multi utilisateur peut accéder à la fois.
* L'utilisateur peut ajouter ou supprimer des hôtes virtuels.
* L'éditeur de l'hôte virtuel peut activer ou désactiver l'hôte virtuel selon le souhait de l'usera € ™.
* Sensibilité non de cas.
* Eh bien-to-do dans Ubuntu et CentOS.


