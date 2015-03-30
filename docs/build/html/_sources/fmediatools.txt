============
Media Tools
============


synopsis
------------

Ce module vise à installer GC recommandée Media Tool que VLC Media Player qui améliore la productivité du système de l'utilisateur. VLC media player supporte de nombreuses méthodes de compression audio et vidéo et les formats de fichiers, y compris les DVD-Vidéo, CD et protocoles de streaming vidéo. VLC media player (communément appelé VLC) est un appareil portable, libre et open-source, un lecteur multimédia multi-plateforme et serveur de streaming des médias écrits par le projet VideoLAN. Voyons comment ce module aide les installer VLC.

Commande Aide
--------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module d'outils médiatiques. Les listes de commandes de l'aide sur les autres paramètres d'outils de médias. Il décrit également la syntaxe pour installer VLC. La commande d'aide pour le module d'outils de médias est représentée ci-dessous.

.. code-block:: bash
  
 ptconfigure mediatools help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu outils de médias.

.. code-block:: bash


	Kevell@corp:/# ptconfigure MediaTools help
	******************************


	This command allows you to install a few GC recommended Media Tools
        for productivity in your system. Currently, we're only including
        VLC Media Player

         MediaTools, media-tools, mediatools, mediatools, media-tools

        - install
        Installs some media tools
        example: ptconfigure mediatools install

	------------------------------
	End Help


installation
---------------


La commande suivante permet d'installer les outils de médias.

.. code-block:: bash

	ptconfigure mediatools install


Visualiser sa fonction La capture d'écran.

.. code-block:: bash


        - install
        Installs some media tools
        example: ptconfigure mediatools install

        ------------------------------
        End Help

Si l'utilisateur procède le processus d'installation, le processus suivant se produit lors de l'installation.

* Extrait des modèles de colis
* Lit listes de paquets.
* Construit arbre de dépendance.
* Lit les informations d'état.
* Répertorie les paquets qui sont automatiquement installés.
* Répertorie les paquets supplémentaires qui sont installés.
* Répertorie les paquets suggérés.
* Répertorie les nouveaux paquets qui sont installés.
* Enfin, les rapports sont clairement affichées avec l'état et les résultats.
* La capture d'écran ci-dessous explique le processus mentionné ci-dessus imagée.

.. code-block:: bash


 kevell@corp:/# ptconfigure mediatools install 
 Install Media Tools? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Media Tools!        * 
 ******************************* 
 [Pharaoh Logging] Packages vlc, libdvdread4 from the Packager Apt are already installed, so not installing 
 Creating /tmp/ptconfigure-temp-script-57996813529.sh 
 chmod 755 /tmp/ptconfigure-temp-script-57996813529.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-57996813529.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-57996813529.sh 
 --2015-03-27 13:21:10--  http://download.videolan.org/pub/debian/stable//Packages 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 3520 (3.4K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ 

 100%[=======================================================================================================>] 3,520       --.-K/s   in 0s      

 2015-03-27 13:21:11 (77.0 MB/s) - â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ saved [3520/3520] 

 --2015-03-27 13:21:12--  http://download.videolan.org/pub/debian/stable/stable/libdvdcss2_1.2.13-0_amd64.deb 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 44462 (43K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ 

 100%[=======================================================================================================>] 44,462      65.6KB/s   in 0.7s   

 2015-03-27 13:21:13 (65.6 KB/s) - â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ saved [44462/44462] 

 Selecting previously unselected package libdvdcss2. 
 (Reading database ... 362949 files and directories currently installed.) 
 Preparing to unpack .../dvdcss-2TJ4IX/libdvdcss.deb ... 
 Unpacking libdvdcss2 (1.2.13-0) ... 
 Setting up libdvdcss2 (1.2.13-0) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 Temp File /tmp/ptconfigure-temp-script-57996813529.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 
 Single App Installer: 
 -------------------------------------------- 
 MediaTools: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 




Options
----------


.. cssclass:: table-bordered

 +----------------------+-----------------------------------------------+-------------+--------------------------------------------+
 | paramètres           | paramètre alternatif                          | option      | commentaires                               |
 +======================+===============================================+=============+============================================+
 |Install Media Tools?  | au lieu de Media Tools, , les solutions       | Y(Yes)      | Si l'utilisateur souhaite procéder le      |
 |(Y/N)                 | suivantes peuvent également être utilisés     |             | processus d'installation qu'ils peuvent    |
 |                      | MediaTools, media-tools, mediatools.          |             | entrée comme Y                             |
 +----------------------+-----------------------------------------------+-------------+--------------------------------------------+
 |Install Media Tools?  | au lieu de Media Tools, , les solutions       | N(No)       | Si l'utilisateur souhaite quitter le       |
 |(Y/N)                 | suivantes peuvent également être utilisés     |             | processus d'installation qu'ils peuvent    |
 |                      | MediaTools, media-tools, mediatools.          |             | entrée comme N.|                           |
 +----------------------+-----------------------------------------------+-------------+--------------------------------------------+
 
   
avantages
------------


* Les paramètres utilisés dans les opérations d'aide et d'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Utilisation de ce module de la productivité du système peut être améliorée.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce module facilite l'installation GC recommandée outils médiatiques.
