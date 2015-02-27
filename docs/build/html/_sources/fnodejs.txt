=========
Node-JS
=========

synopsis
-------------

Ce module aide les utilisateurs à installer Node JS qui est un côté serveur JS Langue. Node.js est un open source, environnement d'exécution multi-plateforme pour les applications côté serveur et réseau. Applications Node.js sont écrits en JavaScript, et peuvent être exécutés dans l'exécution Node.js sur OS X, Microsoft Windows, Linux et FreeBSD. Ici, nous allons voir comment ce module facilite l'installation et l'aide de la Node-JS.

Commande Aide
---------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module Node-JS. Les listes de commande d'aide sur les alternatives aux paramètres du module Node-JS. Il décrit également la syntaxe pour installer le module Node-JS. La commande d'aide pour le module Node-JS est représentée ci-dessous.

.. code-block:: bash

		ptconfigure NodeJS help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu Node JS.

.. code-block:: bash
		


 kevell@corp:/# ptconfigure NodeJS help
 ******************************


  This command allows you to install Node JS, The Server Side JS Language

  NodeJS, node-js, nodejs

        - install
        Installs NodeJS through apt-get.
        example: ptconfigure node-js install

 ------------------------------
 End Help
 ******************************




installation
----------------

Installation du Node-JS à votre machine, qui peut être fait simplement en utilisant la commande suivante comme indiqué:

.. code-block:: bash

		ptconfigure node-js install

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +------------------------+------------------------------------------+-------------+-------------------------------------------------+
 | paramaters             | Alternative Paramètre                    | options     | commentaires                                    |
 +========================+==========================================+=============+=================================================+
 |Install Node JS? (Y/N)  | Aulieude Node JS, NodeJS, noeud-js,      | Y(Yes)      | Si l'utilisateur souhaite procéder le processus |
 |                        | nodejs peuvent également être utilisés.  |             | d'installation qu'ils peuvent entrée comme Y.   |
 +------------------------+------------------------------------------+-------------+-------------------------------------------------+
 |Install Node JS? (Y/N)  | Aulieude Node JS, NodeJS, noeud-js,      | N(No)       | Si l'utilisateur souhaite procéder le processus |
 |                        | nodejs peuvent également être utilisés.  |             | d'installation qu'ils peuvent entrée comme N.|  |
 +------------------------+------------------------------------------+-------------+-------------------------------------------------+


Si l'utilisateur procède le processus d'installation, pendant l'exécution de l'installation, le processus suivant se produit:

* Lit listes de paquets.
* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste des paquets qui sont automatiquement installés.
* Liste des nouveaux paquets installés.
* Énumère le nombre de fichiers qui sont mis à niveau, nouvellement installés, retirés, non reclassés.

Enfin, les rapports et le statut sont clairement signalés. Et aussi, en ajoutant package nodejs du Packager Apt exécutés correctement. La capture d'écran ci-dessous illustre l'ensemble du processus d'installation comme décrit.

Si le nœud-js module est déjà en place dans la machine de l'utilisateur, il affichera un message que le paquet noeud-js de l'emballeur Apt est déjà installé. La capture d'écran qui suit est un bon exemple pour ceux type de messages.

.. code-block:: bash

 kevell@corp:/# ptconfigure node-js install
 Install Node JS? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Node JS!        *
 *******************************
	Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  ax25-node libax25 openbsd-inetd
 The following NEW packages will be installed:
  ax25-node libax25 node openbsd-inetd
 0 upgraded, 4 newly installed, 0 to remove and 17 not upgraded.
 Need to get 110 kB of archives.
 After this operation, 465 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libax25 amd64 0.0.12-rc2+cvs20120204-2ubuntu2 [22.7 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main openbsd-inetd amd64 0.20091229-2ubuntu3 [30.8 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/universe ax25-node amd64 0.3.2-7.4 [54.8 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/universe node all 0.3.2-7.4 [1,284 B]
 Fetched 110 kB in 2s (39.1 kB/s)
 Selecting previously unselected package libax25.
 (Reading database ... 237551 files and directories currently installed.)
 Preparing to unpack .../libax25_0.0.12-rc2+cvs20120204-2ubuntu2_amd64.deb ...
 Unpacking libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Selecting previously unselected package openbsd-inetd.
 Preparing to unpack .../openbsd-inetd_0.20091229-2ubuntu3_amd64.deb ...
 Unpacking openbsd-inetd (0.20091229-2ubuntu3) ...
 Selecting previously unselected package ax25-node.
 Preparing to unpack .../ax25-node_0.3.2-7.4_amd64.deb ...
 Unpacking ax25-node (0.3.2-7.4) ...
 Selecting previously unselected package node.
 Preparing to unpack .../node_0.3.2-7.4_all.deb ...
 Unpacking node (0.3.2-7.4) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Setting up openbsd-inetd (0.20091229-2ubuntu3) ...
 * Stopping internet superserver inetd
   ...done.
 * Not starting internet superserver: no services enabled
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up ax25-node (0.3.2-7.4) ...
 Setting up node (0.3.2-7.4) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package node from the Packager Apt executed correctly
            
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libv8-3.14.5
 The following NEW packages will be installed:
  libv8-3.14.5 nodejs
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 1,873 kB of archives.
 After this operation, 7,429 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libv8-3.14.5 amd64 3.14.5.8-5ubuntu2 [1,189 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/universe nodejs amd64 0.10.25~dfsg2-2ubuntu1 [684 kB]
 Fetched 1,873 kB in 14s (126 kB/s)
 Selecting previously unselected package libv8-3.14.5.
 (Reading database ... 237621 files and directories currently installed.)
 Preparing to unpack .../libv8-3.14.5_3.14.5.8-5ubuntu2_amd64.deb ...
 Unpacking libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Selecting previously unselected package nodejs.
 Preparing to unpack .../nodejs_0.10.25~dfsg2-2ubuntu1_amd64.deb ...
 Unpacking nodejs (0.10.25~dfsg2-2ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Setting up nodejs (0.10.25~dfsg2-2ubuntu1) ...
 update-alternatives: using /usr/bin/nodejs to provide /usr/bin/js (js) in auto mode
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package nodejs from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NodeJS: Success
 ------------------------------
 Installer Finished


avantages
------------

* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
* Si le paquet noeud-js existe déjà dans la machine de l'utilisateur, il ne sera pas écrasements, au lieu de cela, il affiche un message comme 
  déjà exister.
* Node.js utilise le moteur Google V8 JavaScript pour exécuter du code, et un grand pourcentage des modules de base sont écrits en JavaScript.
* Node.js contient une bibliothèque intégrée pour permettre aux applications d'agir comme un serveur Web sans logiciel comme Apache HTTP 
  Server ou IIS.
