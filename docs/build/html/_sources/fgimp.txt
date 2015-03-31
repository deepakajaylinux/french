=======
GIMP
=======


Synopsis
-----------

Ce module permet aux utilisateurs d'installer GIMP qui est un éditeur d'image populaire.

GIMP un acronyme pour Programme GNU Image Manipulation) est utilisé pour la retouche d'image et l'édition, de forme libre dessin, redimensionnement, recadrage, photo-montages, la conversion entre les différents formats d'image, et les tâches plus spécialisées.

GIMP est distribué gratuitement (et par) ne importe qui, et ne importe qui peut regarder son contenu et son code source et peut ajouter des fonctionnalités ou corriger les problèmes. Il est distribué sous licence GPLv3 LGPLv3 et +. GIMP a commencé en 1995 comme le projet d'école de deux étudiants universitaires; maintenant GIMP est une application à part entière, disponible sur toutes les distributions de GNU / Linux et les versions récentes de Microsoft Windows et Mac OS X.

Voyons comment ce module facilite l'installation de GIMP parmi les sujets à venir.


Commande Aide
-------------------

La commande d'aide est un manuel d'utilisation brève qui représente les utilisateurs concernant l'objectif de ce module, ses listes aboutissants ses paramètres alternatifs qui peuvent être utilisés dans les déclarations, avec la syntaxe pour l'installation de GIMP grâce à apt-get. La syntaxe d'utilisation de l'aide option dans ce module est illustré ci-dessous,

.. code-block:: bash

	ptconfigure GIMP help


La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de GIMP.


.. code-block:: bash

 kevell@corp:/# ptconfigure GIMP help 
 ******************************** 

  This command allows you to install GIMP, the popular Image Editor 
  GIMP, gimp 

        - install 
        Installs GIMP through apt-get 
        example: ptconfigure gimp install 

 ------------------------------ 
 End Help 
 ****************************** 



installation
--------------

La commande utilisée pour l'installation de GIMP grâce à apt-get en utilisant ce module est simple en utilisant simplement la commande ci-dessous,
.. code-block:: bash

	ptconfigure GIMP install

Après avoir saisi la commande ci-dessus, les étapes suivantes sont effectuées comme décrit dans le tableau,

.. cssclass:: table-bordered


 +-----------------------+---------------------------------+------------+------------------------------------------------------+
 | Paramètres            | Alternative paramètres          | Option     | Commentaires                                         |
 +=======================+=================================+============+======================================================+
 |GIMP Install? (Y/N)    | Au lieu de GIMP nous pouvons    | Y(Yes)     | Si l'utilisateur souhaite continuer l'installation,  |
 |                       | utiliser gimp également.        |            | ils peuvent entrée comme Y.                          |
 +-----------------------+---------------------------------+------------+------------------------------------------------------+
 |GIMP Install? (Y/N)    | Au lieu de GIMP nous pouvons    | N(No)      | Si l'utilisateur souhait de quitter l'installation,  |
 |                       | utiliser gimp également.        |            | ils peuvent entrée comme N.|                         |
 +-----------------------+---------------------------------+------------+------------------------------------------------------+


La capture d'écran ci-dessous illustre visuellement sur le processus d'installation.

.. code-block:: bash

 kevell@corp:/# ptconfigure gimp install 
 Install GIMP? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *          ! GIMP !        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-67656420389.sh 
 chmod 755 /tmp/ptconfigure-temp-script-67656420389.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-67656420389.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-67656420389.sh 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following package was automatically installed and is no longer required: 
  libjemalloc1 
 Use 'apt-get autoremove' to remove it. 
 The following extra packages will be installed: 
  gimp-data libamd2.3.1 libbabl-0.1-0 libblas3 libcamd2.3.1 libccolamd2.8.0 
  libcholmod2.1.2 libgegl-0.2-0 libgfortran3 libgimp2.0 libilmbase6 
  libjavascriptcoregtk-1.0-0 liblapack3 libmng2 libopenexr6 libumfpack5.6.2 
  libwebkitgtk-1.0-0 libwebkitgtk-1.0-common 
 Suggested packages: 
  gimp-help-en gimp-help gimp-data-extras 
 The following NEW packages will be installed: 
  gimp gimp-data libamd2.3.1 libbabl-0.1-0 libblas3 libcamd2.3.1 
  libccolamd2.8.0 libcholmod2.1.2 libgegl-0.2-0 libgfortran3 libgimp2.0 
  libilmbase6 libjavascriptcoregtk-1.0-0 liblapack3 libmng2 libopenexr6 
  libumfpack5.6.2 libwebkitgtk-1.0-0 libwebkitgtk-1.0-common 
 0 upgraded, 19 newly installed, 0 to remove and 6 not upgraded. 
 Need to get 14.2 MB/19.7 MB of archives. 
 After this operation, 87.2 MB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty-proposed/main libwebkitgtk-1.0-0 amd64 2.4.8-1ubuntu1/ubuntu14.04.1 [7,224 kB] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty-proposed/main libwebkitgtk-1.0-0 amd64 2.4.8-1ubuntu1/ubuntu14.04.1 [7,224 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main libgimp2.0 amd64 2.8.10-0ubuntu1 [484 kB] 
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main gimp-data all 2.8.10-0ubuntu1 [3,068 kB] 
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main gimp amd64 2.8.10-0ubuntu1 [3,411 kB] 
 Fetched 9,355 kB in 18min 31s (8,412 B/s) 
 Selecting previously unselected package libamd2.3.1:amd64. 
 (Reading database ... 381874 files and directories currently installed.) 
 Preparing to unpack .../libamd2.3.1_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libbabl-0.1-0:amd64. 
 Preparing to unpack .../libbabl-0.1-0_0.1.10-1ubuntu2_amd64.deb ... 
 Unpacking libbabl-0.1-0:amd64 (0.1.10-1ubuntu2) ... 
 Selecting previously unselected package libcamd2.3.1:amd64. 
 Preparing to unpack .../libcamd2.3.1_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libcamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libccolamd2.8.0:amd64. 
 Preparing to unpack .../libccolamd2.8.0_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libccolamd2.8.0:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libblas3. 
 Preparing to unpack .../libblas3_1.2.20110419-7_amd64.deb ... 
 Unpacking libblas3 (1.2.20110419-7) ... 
 Selecting previously unselected package libgfortran3:amd64. 
 Preparing to unpack .../libgfortran3_4.8.2-19ubuntu1_amd64.deb ... 
 Unpacking libgfortran3:amd64 (4.8.2-19ubuntu1) ... 
 Selecting previously unselected package liblapack3. 
 Preparing to unpack .../liblapack3_3.5.0-2ubuntu1_amd64.deb ... 
 Unpacking liblapack3 (3.5.0-2ubuntu1) ... 
 Selecting previously unselected package libcholmod2.1.2:amd64. 
 Preparing to unpack .../libcholmod2.1.2_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libcholmod2.1.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libilmbase6:amd64. 
 Preparing to unpack .../libilmbase6_1.0.1-6ubuntu1_amd64.deb ... 
 Unpacking libilmbase6:amd64 (1.0.1-6ubuntu1) ... 
 Selecting previously unselected package libopenexr6:amd64. 
 Preparing to unpack .../libopenexr6_1.6.1-7ubuntu1_amd64.deb ... 
 Unpacking libopenexr6:amd64 (1.6.1-7ubuntu1) ... 
 Selecting previously unselected package libumfpack5.6.2:amd64. 
 Preparing to unpack .../libumfpack5.6.2_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libumfpack5.6.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libgegl-0.2-0:amd64. 
 Preparing to unpack .../libgegl-0.2-0_0.2.0-4ubuntu1_amd64.deb ... 
 Unpacking libgegl-0.2-0:amd64 (0.2.0-4ubuntu1) ... 
 Selecting previously unselected package libjavascriptcoregtk-1.0-0:amd64. 
 Preparing to unpack .../libjavascriptcoregtk-1.0-0_2.4.8-1ubuntu1/ubuntu14.04.1_amd64.deb ... 
 Unpacking libjavascriptcoregtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libmng2:amd64. 
 Preparing to unpack .../libmng2_2.0.2-0ubuntu3_amd64.deb ... 
 Unpacking libmng2:amd64 (2.0.2-0ubuntu3) ... 
 Selecting previously unselected package libwebkitgtk-1.0-common. 
 Preparing to unpack .../libwebkitgtk-1.0-common_2.4.8-1ubuntu1/ubuntu14.04.1_all.deb ... 
 Unpacking libwebkitgtk-1.0-common (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libwebkitgtk-1.0-0:amd64. 
 Preparing to unpack .../libwebkitgtk-1.0-0_2.4.8-1ubuntu1/ubuntu14.04.1_amd64.deb ... 
 Unpacking libwebkitgtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libgimp2.0. 
 Preparing to unpack .../libgimp2.0_2.8.10-0ubuntu1_amd64.deb ... 
 Unpacking libgimp2.0 (2.8.10-0ubuntu1) ... 
 Selecting previously unselected package gimp-data. 
 Preparing to unpack .../gimp-data_2.8.10-0ubuntu1_all.deb ... 
 Unpacking gimp-data (2.8.10-0ubuntu1) ... 
 Selecting previously unselected package gimp. 
 Preparing to unpack .../gimp_2.8.10-0ubuntu1_amd64.deb ... 
 Unpacking gimp (2.8.10-0ubuntu1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Processing triggers for hicolor-icon-theme (0.13-1) ... 
 Processing triggers for mime-support (3.54ubuntu1.1) ... 
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ... 
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ... 
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ... 
 Rebuilding /usr/share/applications/bamf-2.index... 
 Setting up libamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libbabl-0.1-0:amd64 (0.1.10-1ubuntu2) ... 
 Setting up libcamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libccolamd2.8.0:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libblas3 (1.2.20110419-7) ... 
 update-alternatives: using /usr/lib/libblas/libblas.so.3 to provide /usr/lib/libblas.so.3 (libblas.so.3) in auto mode 
 Setting up libgfortran3:amd64 (4.8.2-19ubuntu1) ... 
 Setting up liblapack3 (3.5.0-2ubuntu1) ... 
 update-alternatives: using /usr/lib/lapack/liblapack.so.3 to provide /usr/lib/liblapack.so.3 (liblapack.so.3) in auto mode 
 Setting up libcholmod2.1.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libilmbase6:amd64 (1.0.1-6ubuntu1) ... 
 Setting up libopenexr6:amd64 (1.6.1-7ubuntu1) ... 
 Setting up libumfpack5.6.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libgegl-0.2-0:amd64 (0.2.0-4ubuntu1) ... 
 Setting up libjavascriptcoregtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libmng2:amd64 (2.0.2-0ubuntu3) ... 
 Setting up libwebkitgtk-1.0-common (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libwebkitgtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libgimp2.0 (2.8.10-0ubuntu1) ... 
 Setting up gimp-data (2.8.10-0ubuntu1) ... 
 Setting up gimp (2.8.10-0ubuntu1) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 Temp File /tmp/ptconfigure-temp-script-67656420389.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 
 GIMP: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  




avantages
----------

* Les paramètres utilisés déclarant aide et d'autres caractéristiques différentes de apt ne sont pas sensibles à la casse.
* Il est bien de choses à faire dans les deux cents os et ainsi que dans Ubuntu.


GIMP fournit également des outils «intelligents» qui utilisent un algorithme plus complexe de faire des choses qui seraient autrement de temps, voire impossible. Il se agit notamment d'un:

* Outil Clone, qui copie pixels en utilisant une brosse
* Healing Brush, qui copie les pixels d'une zone et corrige ton et la couleur
* Outil Perspective de clone, qui fonctionne comme l'outil clone, mais corrige des changements de distance
* Blur et aiguiser les flous d'outils et aiguise aide d'un pinceau
* Dodge et un outil de gravure est une brosse qui rend cibles pixels plus clairs (esquives) ou plus sombre (brûlures)


GIMP transformer outils comprennent:

* Aligner
* Déplacer
* cultures
* Rotation
* échelle
* Shear
* perspective
* flip
