===========
VNC
===========

synopsis
-------------

Ce module fournit une assistance pour l'installation vnc4server via apt get. Il permet de se connecter pour la machine virtuelle. Il facilite assurer avant l'installation.

Commande Aide
-----------------------

La commande d'aide fournit une prise de conscience en ce qui concerne le module VNC. Il décrit également sur les options qui peuvent être effectuées en vertu de ce module VNC.

La commande d'aide pour ce module VNC est donnée ci-dessous,

.. code-block:: bash

	ptconfigure vnc help

La capture d'écran ci-dessous vous montre une représentation picturale concernant l'utilisation de la commande d'aide pour le module VNC.

.. code-block:: bash

 Kevell@corp:/# ptconfigure vnc help
 ******************************
        This command allows you to install VNC, the popular Virtual Machine Solution.
	 VNC, vnc

        - install
        Installs VNC through apt-get
        example: ptconfigure vnc install

	------------------------------
	End Help
	******************************


Installation
------------------

.. code-block:: bash
	
		ptconfigure vnc install

After inputting the command as given above, the following operations takes places.



.. cssclass:: table-bordered


 +--------------------------+----------------------+---------------+----------------------------------------------------------+
 | paramètres               | Autres paramètres    | Options       | Commentaires                                             |
 +==========================+======================+===============+==========================================================+
 |Install VNC? (Y/N)        | VNC, vnc             | Y(Yes)        | Si l'utilisateur souhaite continuer avec le processus    |
 |                          |                      |               | d'installation, ils peuvent entrée comme Y.              |
 +--------------------------+----------------------+---------------+----------------------------------------------------------+
 |Install VNC? (Y/N)        | VNC, vnc             | N(No)         | Si l'utilisateur souhaite quitter le processus           |
 |                          |                      |               | d'installation, ils peuvent cesser de fumer en utilisant |
 |                          |                      |               | simplement N.|                                           |
 +--------------------------+----------------------+---------------+----------------------------------------------------------+



Lors de l'installation du serveur VNC, il effectue les opérations suivantes comme indiqué ci-dessous:

* Lit la liste des paquets, des informations d'état,
* Construit l'arbre des dépendances.
* Installe les xbase-clients que des forfaits supplémentaires, vnc-java que des forfaits proposés.
* Installe vnc4server xbase-clients que les nouveaux paquets.
* Il affiche également le nombre de fichiers mis à niveau, nouvellement installé, enlevé, pas mis à niveau.

La capture d'écran comme ci-dessous, explique les utilisateurs graphique concernant le processus d'installation.

.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  xbase-clients
 Suggested packages:
  vnc-java
 The following NEW packages will be installed:
  vnc4server xbase-clients
 0 upgraded, 2 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,579 kB of archives.
 After this operation, 5,418 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe xbase-clients all 1:7.7+1ubuntu8 [2,752 B]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vnc4server amd64 4.1.1+xorg4.3.0-37ubuntu5.0.1 [1,577 kB]
 Fetched 1,579 kB in 33s (46.6 kB/s)
 Selecting previously unselected package xbase-clients.
 (Reading database ... 211210 files and directories currently installed.)
 Preparing to unpack .../xbase-clients_1%3a7.7+1ubuntu8_all.deb ...
 Unpacking xbase-clients (1:7.7+1ubuntu8) ...
 Selecting previously unselected package vnc4server.
 Preparing to unpack .../vnc4server_4.1.1+xorg4.3.0-37ubuntu5.0.1_amd64.deb ...
 Unpacking vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xbase-clients (1:7.7+1ubuntu8) ...
 Setting up vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 update-alternatives: using /usr/bin/vnc4server to provide /usr/bin/vncserver (vncserver) in auto mode
 update-alternatives: using /usr/bin/Xvnc4 to provide /usr/bin/Xvnc (Xvnc) in auto mode
 update-alternatives: using /usr/bin/x0vnc4server to provide /usr/bin/x0vncserver (x0vncserver) in auto mode
 update-alternatives: using /usr/bin/vnc4passwd to provide /usr/bin/vncpasswd (vncpasswd) in auto mode
 update-alternatives: using /usr/bin/vnc4config to provide /usr/bin/vncconfig (vncconfig) in auto mode
 [Pharaoh Logging] Adding Package vnc4server from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************




Si le serveur vnc existe déjà dans la machine de l'utilisateur, il sera jette un message d'exception que le serveur vnc est déjà installé. La capture d'écran ci-dessous donne une représentation picturale qui concerne le message d'exception.

.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 [Pharaoh Logging] Package vnc4server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
---------------

* Il permet d'assurer le processus avant l'installation.
* Il facilite l'installation via apt get.
* Il permet la connectivité de la machine virtuelle.
* En cas de serveur VNC est déjà exister, il jette un message exceptionnel pendant le processus d'assurer.
