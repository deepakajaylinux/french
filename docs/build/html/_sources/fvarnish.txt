===========
Varnish
===========

synopsis
--------------

Ce module aide à l'installation du vernis à la machine de l'utilisateur. Vernis est un programme qui peut grandement accélérer un site Web tout en réduisant la charge sur le serveur Web. Selon le site officiel de vernis, vernis est un «accélérateur d'applications Web aussi connu comme un proxy inverse mise en cache HTTP". Voyons ici, à propos de comment ce module effectue l'installation de vernis de apt-get.

Commande Aide
------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de vernis. La commande help répertorie les autres paramètres de vernis. Il décrit également la syntaxe pour l'installation de vernis. La commande d'aide dans le cadre du module de vernis est donnée ci-dessous:

.. code-block:: bash

		ptconfigure varnish help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous montre sur la commande d'aide en vertu module de vernis.


.. code-block:: bash

	kevell@corp:/# ptconfigure Varnish help
	******************************


        This command allows you to install Varnish, the popular HTTP Cache

        Varnish, varnish

        - install
        Installs Varnish through apt-get
        example: ptconfigure varnish install

	------------------------------
	End Help
	******************************

installation
---------------

La commande utilisée pour installer le vernis à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash

		ptconfigure varnish install

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +--------------------------+--------------------------------------------------+--------------+-------------------------------------------+
 | paramètres               | Autres paramètres                                | Options      | commentaire                               |
 +==========================+==================================================+==============+===========================================+
 |Install Varnish? (Y/N)    | au lieu deVarnish, varnish peuvent également     | Y(Yes)       | Si l'utilisateur souhaite procéder le     |
 |                          | être utilisés.                                   |              | d'installation qu'ils peuvent entrée      |
 |                          |                                                  |              | comme Y.                                  |
 +--------------------------+--------------------------------------------------+--------------+-------------------------------------------+
 |Install Varnish? (Y/N)    | au lieu deVarnish, varnish peuvent également     | N(No)        | Si l'utilisateur souhaite quitter le      |
 |                          | être utilisés.                                   |              | processus d'installation qu'ils peuvent   |
 |                          |                                                  |              | entrée comme N.|                          |
 +--------------------------+--------------------------------------------------+--------------+-------------------------------------------+


Si l'utilisateur procède le processus d'installation, pendant l'exécution de l'installation, le processus suivant se produit:

* Lit listes de paquets.
* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste des paquets installés.
* Liste des packages supplémentaires installés.
* Liste des nouveaux paquets installés.
* Nombre de fichiers mis à niveau, nouvellement installés, retirés, pas mis à niveau.
* Enfin, à partir accélérateur HTTP verni.
* La capture d'écran ci-dessous illustre le processus mentionné ci-dessus:

.. code-block:: bash
   
	Kevell@corp:/# ptconfigure varnish install
	Install Varnish? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Varnish !        *
	*******************************
	Creating /tmp/ptconfigure-temp-script-95745650915.sh
	chmod 755 /tmp/ptconfigure-temp-script-95745650915.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-95745650915.sh Permissions
	Executing /tmp/ptconfigure-temp-script-95745650915.sh
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
        libjemalloc1 libvarnishapi1
	Suggested packages:
	varnish-doc
	The following NEW packages will be installed:
	libjemalloc1 libvarnishapi1 varnish
	0 upgraded, 3 newly installed, 0 to remove and 6 not upgraded.
	Need to get 518 kB of archives.
	After this operation, 1,653 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libvarnishapi1 amd64 3.0.5-2 [29.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjemalloc1 amd64 3.5.1-2 [76.8 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe varnish amd64 3.0.5-2 [411 kB]
	Fetched 518 kB in 3s (152 kB/s)
	Selecting previously unselected package libvarnishapi1.
	(Reading database ... 201582 files and directories currently installed.)
	Preparing to unpack .../libvarnishapi1_3.0.5-2_amd64.deb ...
	Unpacking libvarnishapi1 (3.0.5-2) ...
	Selecting previously unselected package libjemalloc1.
	Preparing to unpack .../libjemalloc1_3.5.1-2_amd64.deb ...
	Unpacking libjemalloc1 (3.5.1-2) ...
	Selecting previously unselected package varnish.
	Preparing to unpack .../varnish_3.0.5-2_amd64.deb ...
	Unpacking varnish (3.0.5-2) ...
	Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Setting up libvarnishapi1 (3.0.5-2) ...
	Setting up libjemalloc1 (3.5.1-2) ...
	Setting up varnish (3.0.5-2) ...
	 * Starting HTTP accelerator varnishd
	   ...done.
	Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Temp File /tmp/ptconfigure-temp-script-95745650915.sh Removed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	Varnish: Success
	------------------------------
	Installer Finished
	******************************





avantages
------------

* Vernis est un moderne et performante, la mise en œuvre open source mise en cache proxy inverse HTTP.
* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
