===============
NginxSBEditor
===============

synopsis
----------

Ce module est une partie amende de modules par défaut et gère les fonctions de Nginx. Voyons sur les méthodes d'utilisation de ce ainsi que sur les fonctions en vertu de cet éditeur de nginx dans les prochains sujets.

Commande Aide
---------------------

La commande help enveloppe toutes les informations nécessaires concernant NginxSBEditor tels que ses principales utilisations, la liste des paramètres de remplacement qui peut être utilisé dans la déclaration, ce sont fonction principale de NginxSBEditor (Ex: ajouter, supprimer, liste, activer, désactiver), et également la syntaxe utilisée pour déclarer ces fonctions intéressantes. La commande suivante est utilisée pour déclarer option d'aide en vertu NginxSBEditor,

.. code-block:: bash

		ptdeploy NginxSBEditor help


La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptdeploy NginxSBEditor help
 ******************************


  This command is part of Default Modules and handles Nginx ServerBlocks Functions.

  NginxSBEditor, nginx-sb-editor, nginxsbe

          - add
          create a Server Block
          example: ptdeploy nginxsbe add
          sb-docroot
          sb-url
          sb-ip-port

          - rm
          remove a Server Block
          example: ptdeploy nginxsbe rm

          - list
          List current Server Blocks
          example: ptdeploy nginxsbe list

          - enable
          enable a Server Block
          example: ptdeploy nginxsbe enable

          - disable
          disable a Server Block
          example: ptdeploy nginxsbe disable

 ------------------------------
 End Help
 ******************************

Comment utiliser
--------------------

Comme illustré et expliqué dans la commande d'aide ci-dessus, le NginxSBEditor, a les fonctions suivantes,

* Ajouter
* Retirer
* Liste
* Activer
* Désactiver


Voyons comment utiliser ces fonctions intéressantes dans NginxSBEditor.

ajouter
---------

Le rôle de cette fonction est de créer / ajouter un nouveau bloc de serveur. La commande et le travail d'ajouter des fonctions est représenté ci-dessous,

.. code-block:: bash

		ptdeploy NginxSBEditor add

Après être entré dans l'ordre donné ci-dessus, le fonctionnement de cette fonction d'ajout est indiqué ci-dessous,

.. cssclass:: table-bordered

 +-----------------------+--------------------------------------------+----------+--------------------------------------------------------+
 | Parameters		 | Alternative Parameters		      | Options  | Comments			                          |
 +=======================+============================================+==========+========================================================+
 |Do you want to add a   | au lieu de NginxSBEditor, nous pouvons     | Y(Yes)   | Si l'utilisateur a besoin d'ajouter un nouveau         |
 |ServerBlock? (Y/N)     | utiliser nginx-sb-editor, nginxsbe aussi.  |          | serveur bloc qu'ils peuvent entrée comme Y.            |
 +-----------------------+--------------------------------------------+----------+--------------------------------------------------------+
 |Do you want to add a 	 | au lieu de NginxSBEditor, nous pouvons     | N(No)	 | Si l'utilisateur n'a pas besoin d'ajouter un nouveau   |
 |ServerBlock? (Y/N)	 | utiliser nginx-sb-editor, nginxsbe aussi.  |          | bloc de serveur qu'ils peuvent d'entrée comme N|       |
 +-----------------------+--------------------------------------------+----------+--------------------------------------------------------+


Si l'utilisateur procède ajoutant les blocs de serveur pendant le processus d'ajouter les étapes suivantes sont impliqués.

Etape 1:

Quelle est la racine des documents?

L'utilisateur dispose de spécifier la racine, se ils le souhaitent ne pas procéder à la valeur par défaut.

Étape 2:

Que URL voulez-vous ajouter au nom du serveur?

L'utilisateur doit indiquer l'url qui est censé ajouter.

Etape 3:

Que IP? Port doit être réglé?

L'utilisateur dispose spécifier l'adresse IP, se ils le souhaitent ne pas procéder à la valeur par défaut.

Etape 4:

Quelle est votre répertoire ServerBlock modèle?

L'utilisateur dispose spécifier le répertoire, se ils le souhaitent ne pas procéder à la valeur par défaut.

Etape 5:

Se il vous plaît vérifier la ServerBlock

L'utilisateur dispose vérifier l'affichage de sortie du bloc de serveur qui est ajouté et assurer.

Etape 6:

Est-ce d'accord? (Y / N)

Si l'utilisateur sont heureux avec le résultat généré, ils peuvent entrée comme Y autre N.

Etape 7:

Quelle est votre répertoire de ServerBlock?

L'utilisateur dispose spécifier le répertoire.

Etape 8:

Voulez-vous permettre à un bloc de serveur? (Y / N)

L'utilisateur dispose à l'entrée que Y ou N en fonction de leurs besoins.

Etape 9:

Quelle est votre répertoire Symlink ServerBlock Enabled.

Si un bloc de serveur est activé, l'utilisateur doit indiquer son répertoire.

Représentant de manière visuelle la capture d'écran ci-dessous le processus expliqué ci-dessus.

.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe add
 Do you want to add a ServerBlock? (Y/N) 
 Y
 What's the document root? Enter nothing for /
 /root/Nginx
 What URL do you want to add as server name?
 www.ngx.com
 What IP:Port should be set? Enter nothing for 127.0.0.1:80

 What is your ServerBlock Template directory? Enter nothing for default templates
 /root/Nginxdir
 Please Choose ServerBlock Template: 
 --- Default Server Block Templates: ---
 (0) docroot-no-suffix
 (1) docroot-src-sfx
 (2) docroot-web-suffix
 (3) docroot-www-suffix
 (4) docroot-docroot-suffix

 3
 Please check ServerBlock: server {
        listen   127.0.0.1:80 ; ## listen for ipv4; this line is default and implied
        #listen   [::]:80 default ipv6only=on; ## listen for ipv6

        root /root/Nginx/www ;
        index index.html index.htm index.php;

        # Make site accessible from http://localhost/
        server_name www.ngx.com ;

        # pass the PHP scripts to FastCGI server listening on 127.0.0.1:9000
        #
        location ~ \.php$ {
                try_files $uri =404;
                fastcgi_split_path_info ^(.+\.php)(/.+)$;
                fastcgi_pass 127.0.0.1:9000;
                fastcgi_index index.php;
                include fastcgi_params;
        }

 }

 Is this Okay? (Y/N) 
 Y
 What is your ServerBlock directory?
 /root/Nginxdir
 Do you want to enable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /home/Nginxsymlink
 Server Block Enabled Symlink Created
 ******************************
 

 1ServerBlock Creator Finished
 ******************************




supprimer
----------

La fonction de suppression est utilisée pour enlever les blocs de serveurs indésirables. Cela peut être fait en utilisant la commande donnée ci-dessous,

.. code-block:: bash

	ptdeploy NginxSBEditor rm

Après avoir saisi la commande ci-dessus, le processus suivant impliqué dans la suppression comme indiqué dans le tableau

.. cssclass:: table-bordered



 +-----------------------+--------------------------------------------+----------+--------------------------------------------------------+
 | Parameters            | Alternative Parameters                     | Options  | Comments                                               |
 +=======================+============================================+==========+========================================================+
 |Do you want to delete  | au lieu de NginxSBEditor, nous pouvons     | Y(Yes)   | Si l'utilisateur doit supprimer le bloc de             |
 |a ServerBlock? (Y/N)   | utiliser nginx-sb-editor, nginxsbe aussi.  |          | serveur qu'ils peuvent entrée comme Y.                 |
 +-----------------------+--------------------------------------------+----------+--------------------------------------------------------+
 |Do you want to delete  | au lieu de NginxSBEditor, nous pouvons     | N(No)    | Si l'utilisateur n'a pas besoin de supprimer le        |
 |a ServerBlock? (Y/N)   | utiliser nginx-sb-editor, nginxsbe aussi.  |          | bloc de serveur qu'ils peuvent entrée comme N|         |
 +-----------------------+--------------------------------------------+----------+--------------------------------------------------------+


Si l'utilisateur procède de supprimer les blocs de serveur lors de ce processus, les étapes suivantes sont impliqués.

Etape 1:

ServerBlock suppression

Quelle est votre répertoire de ServerBlock?

L'utilisateur doit indiquer le répertoire.

Étape 2:

Se il vous plaît Choisissez ServerBlock

Blocs --all serveur: ---

(0) www.ngn.com

(1) www.ngx.com

(2) www.nx.com

L'utilisateur doit indiquer les valeurs 0-2 en fonction de leurs besoins.

Etape 3:

!! Sure? Certainement supprimer ServerBlock? (Y / N) !!

L'utilisateur doit indiquer Y ou N en fonction de leurs besoins.

Etape 4:

Voulez-vous désactiver un ServerBlock? (Y / N)

L'utilisateur doit indiquer Y ou N en fonction de leurs besoins.

Etape 5:

Quelle est votre répertoire Symlink ServerBlock Enabled?

L'utilisateur doit indiquer le répertoire.

Représentant de manière visuelle sur le processus de suppression de la capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe rm
 Do you want to delete ServerBlock/s? (Y/N) 
 Y
 Deleting ServerBlock
 What is your ServerBlock directory?
 /root/Nginxdir
 Please Choose ServerBlock:
 ---All Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 (2) www.nx.com

 2
 !! Sure? Definitely delete ServerBlock? (Y/N) !!
 Y
 Do you want to disable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /root/home/Nginxsymlink
 Server Block www.nx.com Disabled if existed
 Server Block www.nx.com Deleted if existed
 *******************************


 1ServerBlock Creator Finished
 ******************************


liste
-------

La fonction de l'option de la liste est de lister les blocs de serveur installés actuelles. La commande utilisée pour la liste est donnée ci-dessous,

.. code-block:: bash

		ptdeploy NginxSBEditor list

Après avoir saisi la commande ci-dessus, le processus suivant impliqué dans l'option de la liste.

Etape 1:

Quelle est votre répertoire de ServerBlock?

L'utilisateur doit indiquer le répertoire.

Étape 2:

Quelle est votre répertoire Symlink ServerBlock Enabled?

L'utilisateur doit indiquer le répertoire.

Après ces étapes, il liste des ServerBlocks actuellement installés sont affichés.

La capture d'écran ci-dessous illustre le fonctionnement de l'option de liste visuellement.

.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe list
 What is your ServerBlock directory?
 /root/Nginxdir
 What is your Enabled Symlink ServerBlock directory?

 Current Installed ServerBlocks:
 --- Enabled Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 --- All Available Server Blocks: ---
 (2) www.ngn.com
 (3) www.ngx.com
 ******************************


 1ServerBlock Creator Finished
 ******************************

avantages
----------

* Il est bien de choses à faire dans les deux Ubuntu et ainsi que dans cent OS.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse.
* Les utilisateurs peuvent afficher la liste des blocs de serveurs disponibles et actuellement installés, même avant d'ajouter ou de supprimer 
  un bloc de serveur.
