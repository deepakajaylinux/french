=============
Host Editor
=============

synopsis
--------------

Ce module prend en charge de gérer Apache éditeur Virtual Host sous ptdeploy. Il peut fonctionner de deux manières. Ils sont ajouter et de supprimer. Vhost Editor est un outil PHP écrite pour faire ajouter des hôtes virtuels à apache une brise. Vhost Editor permettra à l'utilisateur d'ajouter, modifier ou supprimer des informations d'hôte virtuel sur le serveur Web de l'utilisateur. Il est commode de travailler avec Ubuntu et cent OS. Voyons comment l'apache Vhost Editor peut fonctionner sous dapperstarano.

Aide command
----------------------

Cette commande help guide l'utilisateur pour créer un hôte virtuel. Cette affiche également d'ajouter un hôte virtuel, supprimer un hôte virtuel, Activer un hôte virtuel, et désactiver un hôte virtuel.

La commande d'aide pour Apachevhosteditor est illustré ci-dessous.

.. code-block:: bash

          ptdeploy Apachevhosteditor help

After inputs the above command, it starts functioning to add a virtual host editor. It catechesis the functions in the screenshots.


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



d'autres paramètres
---------------------------------

Voici les autres paramètres qui peuvent être définis dans les déclarations:

ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted.

Ajouter
-------------

Cela facilite à l'utilisateur de créer un hôte virtuel. Tout en ajoutant hôte virtuel il peut demande vhe-docroot, vhe-file-ext, vhe-apache-command, vhe-ip port,vhe-host-dir, vhe-templates,vhe-default-template-name. L'utilisateur peut entrer dans le selon leur souhait.

.. code-block:: bash

        sudo ptdeploy vhe add

Après l'entrée que la commande ci-dessus, l'utilisateur peut remplir le processus suivant

.. cssclass:: table-bordered

 +---------------------------------+--------------+---------------------------------+-------------------------------------------------------+
 | paramètres                      | annuaire     | option                          | commentaires                                          |
 +=================================+==============+=================================+=======================================================+
 |ptdeploy vhe add (Default)       |  Yes         | Il peut demander à              | Hôte virtuel ajouté dans le document racine spécifié  |
 |                                 |              | l'utilisateur root du document  | dans ptdeploy                                         |
 +---------------------------------+--------------+---------------------------------+-------------------------------------------------------+
 |What’s the server name           | -            | Il peut demander à              | Nom du serveur ajouté sous ptdeploy                   |
 |                                 |              | l'utilisateur le nom du serveur |                                                       |
 +---------------------------------+--------------+---------------------------------+-------------------------------------------------------+
 |What IP:Port (default)           | 127.0.0.1:80 | Il peut demander à              | Lorsque l'entrée de l'utilisateur comme entrer la     |
 |                                 |              | l'utilisateur IP port           | valeur par défaut ajoutée pour IP : Port              |
 +---------------------------------+--------------+---------------------------------+-------------------------------------------------------+
 |What file extension should be    | None         | Il peut demander à              | L'utilisateur donne entrée comme extension de         |
 |used? (Default)                  |              | l'utilisateur d'extension       | fichier                                               |
 +---------------------------------+--------------+---------------------------------+-------------------------------------------------------+
 |ptdeploy vhe add                 | No           | Il peut demander à              | Il peut se termine le processus                       |
 |                                 |              | l'utilisateur pour l'entrée|    |                                                       |
 +---------------------------------+--------------+---------------------------------+-------------------------------------------------------+




Enfin, le système peut demande pour le répertoire des modèles de vhost. Il ya cinq options sont disponibles dans les modèles. Ils sont comme suit.

0 pour doc root-no-suffixe

1 pour suffixe de doc utilisé pour le document suffixe écran

2 pour doc -web suffixe utilisé pour suffixe web de documents

3 pour suffixe de doc utilisé pour suffixe world wide web

4 pour docroot-suffixe utilisé pour le document suffixe racine


L'utilisateur souhaite sélectionner les valeurs en fonction de leurs besoins. Ensuite, le système peut demander le nom de serveur virtuel, l'adresse et l'utilisateur root IP etc est juste ou fausse. Si l'utilisateur dit oui, alors il affiche le répertoire de serveur virtuel et activer cette vhost?

L'utilisateur répond oui il peut permettre à l'hôte virtuel bien il peut sortir.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe add
 Do you want to add a VHost? (Y/N)
 Y
 What's the document root? Enter nothing for /
 root
 What URL do you want to add as server name?
 www.vh.com
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
       ServerName www.vh.com
       DocumentRoot root
       <Directory root>
               Options Indexes FollowSymLinks MultiViews
               AllowOverride All
               Order allow,deny
               allow from all
       </Directory>
 </VirtualHost>

 Is this Okay? (Y/N)

 ******************************


 Apache VHost Editor Finished
 ******************************


supprimer
-----------

La commande de terminal pour la suppression hôte (s) virtuelle est rm. Le format général de cette commande est rm. rm supprime un hôte virtuel si vous spécifiez un chemin d'accès correct pour elle et si vous ne le faites pas, il affiche un message d'erreur et de passer à l'hôte suivant. Parfois, vous ne pouvez pas avoir les permissions d'écriture pour un hôte virtuel, dans ce cas il vous demande confirmation. Tapez oui si vous souhaitez supprimer.

Si le nom supprimé était le dernier lien à un hôte virtuel et aucun processus n'a ouvert l'hôte virtuel, l'hôte virtuel est supprimé et l'espace qu'il utilisait est rendu disponible pour une réutilisation.

Si le nom était le dernier lien à un hôte virtuel, mais qu'un processus conserve encore l'hôte virtuel ouvert, l'hôte virtuel restera en existence jusqu'à ce que le dernier descripteur d'hôte virtuel se référant à elle est fermée.

Si le nom correspond à un lien symbolique, le lien est supprimé. La commande suivante permet de supprimer l'hôte virtuel.

.. code-block:: bash

           sudo ptdeploy vhe rm –yes –guess –vhe-deletion-vhost=www.kevell.com

La capture d'écran suivante peut expliquer ses fonctions.

.. code-block:: bash

 - rm
         example: ptdeploy vhe rm
         example: ptdeploy vhe rm --yes --
         example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
         example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm
 Do you want to delete VHost/s? (Y/N) 
 y
 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf

 0
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 yes
 Site 000-default disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite 000-default.conf done
 VHost 000-default.conf Deleted  if existed
 ******************************


 1Apache VHost Editor Finished
 ******************************




liste
-------

Liste des informations sur l'hôte virtuel (le répertoire courant par défaut). Trier les entrées par ordre alphabétique. Les arguments obligatoires a des options longues ainsi que les options courtes. Une liste appelée avec une URL spécifiant à la fois le nom de la liste et également le point de vue sous-jacente qui fournira et organiser les données. La commande suivante permet de lister l'hôte virtuel.

.. code-block:: bash

	    ptdeploy vhe list

Notez que si une liste peut être utilisé avec une variété de points de vue, ou pourrait être adaptée pour produire une page élaborée à partir d'un point de vue spécifiquement conçu pour organiser les données pour cela. Listes stockées dans le champ d'un document de conception des listes. Il peut être visualisé par les captures d'écran.

.. code-block:: bash

 - list
         List current Virtual Hosts
         example: ptdeploy vhe list


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe list
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 You have a sites available dir, so also listing available sites.
 Current Installed VHosts:
 --- Enabled Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf
 --- All Available Virtual Hosts: ---
 (2) 000-default.conf
 (3) default-ssl.conf
 ******************************


 1Apache VHost Editor Finished
 ******************************





permettre
------------

Boot sécurisé est une fonction conçue pour empêcher les logiciels malveillants et les médias non autorisée de chargement pendant le processus de démarrage. Cette option permettra activé le bloc de serveur. Dans hôte virtuel lorsque l'occasion tapé la commande suivante,

.. code-block:: bash

	ptdeploy vhe enable

Cette option est activée par défaut. Cette option permet au serveur d'hôte virtuel permet.

Module Aider à développer un grand nombre de capacités habilitantes nécessaires à l'entretien des environnements haute performance grâce à notre compréhension des interdépendances entre les personnes, les processus et la technologie. La capture d'écran ci-dessous explique la même chose..

.. code-block:: bash


 - enable

         enable a Server Block
         example: ptdeploy vhe enable


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe enable
 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf
 
 0
 ERROR: Site default-ssl.conf does not exist!
 a2ensite default-ssl.conf.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************





désactiver
---------------

Cette désactivation utilisée pour désactiver le serveur. Les connexions inactives ou ralenti éditeur hôte virtuel sont normalement déconnectés par le serveur après une certaine période de temps. La commande suivante permet de désactiver l'éditeur d'hôte virtuel

.. code-block:: bash
	
	ptdeploy vhe disable

Après avoir tapé cette commande, il peut demander à l'utilisateur de désactiver le serveur. Si les entrées de l'utilisateur que oui il désactiver le serveur est à dire qu'il ne permettra à aucun corps à travailler dans ce serveur.

La capture d'écran suivante visualiser évidemment.

.. code-block:: bash

 - disable
 
        disable a Server Block
         example: ptdeploy vhe disable

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe disable
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf

 0
 Site default-ssl already disabled
 a2dissite default-ssl.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************



Avantages
----------------
* multi utilisateur peut accéder à la fois.
* L'utilisateur peut ajouter ou supprimer des hôtes virtuels.
* L'éditeur d'hôte virtuel peut activer ou désactiver l'hôte virtuel selon le souhait de l'utilisateur.
* Sensibilité non de cas.

