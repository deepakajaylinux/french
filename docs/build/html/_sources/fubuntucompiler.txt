================
Ubuntu Compiler
================

synopsis
----------

Ce module revitaliser programme de c. Ubuntu et autres distributions Linux disposent de vastes dépôts de paquets pour sauver l'utilisateur de la peine de compilation. Avec une seule commande, vous pouvez construire à partir des sources comme un pro. Ce est le confort avec Ubuntu et CentOS.

Commande Aide
--------------

Cette commande d'aide à guider l'utilisateur sur compilateur Ubuntu. Ce est moins de temps, car il peut automatiquement installé. Convient pour le programme de C.

.. code-block:: bash

		ptconfigure Ubuntucompiler help

La commande d'aide suivante aidera l'utilisateur pour l'installation.

.. code-block:: bash

	kevell@corp:/# ptconfigure UbuntuCompiler help
	******************************


         This allows you to Complie programs written in C Source

          UbuntuCompiler, ubuntu-compiler, ubuntucompiler

        - install
        Installs Ubuntu Compiling tools through apt-get.
        example: ptconfigure ubuntu-compiler install

	------------------------------
	End Help
	******************************

installation
--------------

Ce est un processus sensible à installer Ubuntu module de compilateur sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

  		ptconfigure Ubuntu-compiler install

Après avoir donné la commande, le compilateur Ubuntu sera installé avec de nouvelles mises à jour.

Si l'entrée de l'utilisateur comme N l'écran suivant viendra.

.. code-block:: bash



 kevell@corp:/# ptconfigure ubuntu-compiler install 
 Install Ubuntu Compiler? (Y/N) 
 y
 ******************************* 
 *        Pharaoh Tools        * 
 *         Ubuntu Comp!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  dh-apparmor libalgorithm-diff-perl libalgorithm-diff-xs-perl 
  libalgorithm-merge-perl libmail-sendmail-perl libsys-hostname-long-perl 
  po-debconf 
 Use 'apt-get autoremove' to remove them. 
 Suggested packages: 
  g++-multilib 
 The following NEW packages will be installed: 
  g++ 
 0 upgraded, 1 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 1,490 B of archives. 
 After this operation, 34.8 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main g++ amd64 4:4.8.2-1ubuntu6 [1,490 B] 
 Fetched 1,490 B in 1s (1,438 B/s) 
 Selecting previously unselected package g++. 
 (Reading database ... 393110 files and directories currently installed.) 
 Preparing to unpack .../g++_4%3a4.8.2-1ubuntu6_amd64.deb ... 
 Unpacking g++ (4:4.8.2-1ubuntu6) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up g++ (4:4.8.2-1ubuntu6) ... 
 update-alternatives: using /usr/bin/g++ to provide /usr/bin/c++ (c++) in auto mode 
 [Pharaoh Logging] Adding Package g++ from the Packager Apt executed correctly  

 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  dh-apparmor libmail-sendmail-perl libsys-hostname-long-perl po-debconf  
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
  dpkg-dev make 
 Suggested packages: 
  debian-keyring make-doc 
 The following NEW packages will be installed: 
  build-essential dpkg-dev make 
 0 upgraded, 3 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 850 kB of archives. 
 After this operation, 2,039 kB of additional disk space will be used. 
 Get:1 http://security.ubuntu.com/ubuntu/ trusty-security/main dpkg-dev all 1.17.5ubuntu5.3 [726 kB] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main make amd64 3.81-8.2ubuntu3 [119 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main build-essential amd64 11.6ubuntu6 [4,838 B] 
 Fetched 850 kB in 37s (22.5 kB/s) 
 Selecting previously unselected package make. 
 (Reading database ... 393115 files and directories currently installed.) 
 Preparing to unpack .../make_3.81-8.2ubuntu3_amd64.deb ... 
 Unpacking make (3.81-8.2ubuntu3) ... 
 Selecting previously unselected package dpkg-dev. 
 Preparing to unpack .../dpkg-dev_1.17.5ubuntu5.3_all.deb ... 
 Unpacking dpkg-dev (1.17.5ubuntu5.3) ... 
 Selecting previously unselected package build-essential. 
 Preparing to unpack .../build-essential_11.6ubuntu6_amd64.deb ... 
 Unpacking build-essential (11.6ubuntu6) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up make (3.81-8.2ubuntu3) ... 
 Setting up dpkg-dev (1.17.5ubuntu5.3) ... 
 Setting up build-essential (11.6ubuntu6) ... 
 [Pharaoh Logging] Adding Package build-essential from the Packager Apt executed correctly 
 [Pharaoh Logging] Package make from the Packager Apt is already installed, so not installing 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 UbuntuCompiler: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 



option
-----------

.. cssclass:: table-bordered


 +--------------------------------+----------------------------------+--------------+---------------------------------------------+
 | Paramètres                     | alternative Paramètres           | option       | Commentaire                                 |
 +================================+==================================+==============+=============================================+
 |Install Ubuntu compiler? Y/N    | UbuntuCompiler, ubuntu-compiler, | Yes          | System starts installation procesLe         |
 |                                | ubuntucompiler                   |              | système démarre processus d'installations   | 
 +--------------------------------+----------------------------------+--------------+---------------------------------------------+
 |Install Ubuntu compiler? Y/N    | UbuntuCompiler, ubuntu-compiler, | No           | Il arrête le processus d'installation       |
 |                                | ubuntucompiler|                  |              |                                             |
 +--------------------------------+----------------------------------+--------------+---------------------------------------------+

avantages
-----------

* Démarrage plus rapide
* Une meilleure sécurité
* Modification du noyau pour anticiper tout compilation
* Convient pour le programme de C

