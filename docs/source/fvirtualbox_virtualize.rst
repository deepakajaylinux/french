=============
Virtualbox
=============

synopsis
-------------

Ce module d'encourager l'installation de la voix. En cas de ptvirtualize module entièrement géré par virtual box.  Il est facile à utiliser avec Ubuntu et cent OS.  Le package de Virtual Box installe sur un système d'exploitation hôte existant sous forme d'application. Les utilisateurs de Virtual Box peuvent charger plusieurs OS invités sous un système de d'exploitation hôte unique. Virtual Box a pris en charge Open Virtualization Format (OVF).C'est à l'aise avec Ubuntu et Cent OS.

Commande Aide
-----------------------

Le guide de commande aide l'utilisateur à installer virtual box dans ptvirtualize. Cette commande help guide l'utilisateur pour créer un hôte virtuel. Cela affiche aussi pour ajouter un hôte virtuel, supprimer un hôte virtuel, permettent à un hôte virtuel et désactiver un hôte virtuel.


La commande help pour la machine virtuelle est illustrée ci-dessous.


.. code-block:: bash

	ptvirtualize virtualbox help

Après les entrées la commande ci-dessus, il commence de fonctionnement pour ajouter un éditeur de l'hôte virtuel. Il catéchèse les fonctions dans les captures d'écran.


La capture d'écran suivante montre sur l'installation de la machine virtuelle.



.. code-block:: bash


Installation
---------------------

Ce module d'initiation de l'utilisateur à installer. Pour activer la machine virtuelle suivez la commande comme suit,

.. code-block:: bash


	ptvirtualize virtual box install

Ensuite, le système peut vous renseigner


ptvirtualize virtual box install? (Y/N) 

Si l'utilisateur entre Y, puis il sera installé, sinon il va quitter l'écran.


.. code-block:: bash

 kevell@corp:/# ptconfigure Virtualbox install
 Install Virtualbox? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Virtualbox !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-27415379023.sh
 chmod 755 /tmp/ptconfigure-temp-script-27415379023.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-27415379023.sh Permissions
 Executing /tmp/ptconfigure-temp-script-27415379023.sh
 invoke-rc.d: initscript virtualbox, action "restart" failed.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  dkms libgsoap4 virtualbox-dkms virtualbox-qt
 Suggested packages:
  debhelper virtualbox-guest-additions-iso vde2
 The following NEW packages will be installed:
   dkms libgsoap4 virtualbox virtualbox-dkms virtualbox-qt
 0 upgraded, 5 newly installed, 0 to remove and 6 not upgraded.
 Need to get 21.2 MB of archives.
 After this operation, 85.7 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libgsoap4 amd64 2.8.16-2 [525 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/multiverse virtualbox amd64 4.3.10-dfsg-1 [15.5 MB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main dkms all 2.2.0.3-1.1ubuntu5.14.04 [64.6 kB]
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/multiverse virtualbox-dkms all 4.3.10-dfsg-1 [538 kB]
 Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/multiverse virtualbox-qt amd64 4.3.10-dfsg-1 [4,592 kB]
 Fetched 21.2 MB in 54s (389 kB/s)
 Selecting previously unselected package libgsoap4:amd64.
 (Reading database ... 203014 files and directories currently installed.)
 Preparing to unpack .../libgsoap4_2.8.16-2_amd64.deb ...
 Unpacking libgsoap4:amd64 (2.8.16-2) ...
 Selecting previously unselected package virtualbox.
 Preparing to unpack .../virtualbox_4.3.10-dfsg-1_amd64.deb ...
 Unpacking virtualbox (4.3.10-dfsg-1) ...
 Selecting previously unselected package dkms.
 Preparing to unpack .../dkms_2.2.0.3-1.1ubuntu5.14.04_all.deb ...
 Unpacking dkms (2.2.0.3-1.1ubuntu5.14.04) ...
 Selecting previously unselected package virtualbox-dkms.
 Preparing to unpack .../virtualbox-dkms_4.3.10-dfsg-1_all.deb ...
 Unpacking virtualbox-dkms (4.3.10-dfsg-1) ...
 Selecting previously unselected package virtualbox-qt.
 Preparing to unpack .../virtualbox-qt_4.3.10-dfsg-1_amd64.deb ...
 Unpacking virtualbox-qt (4.3.10-dfsg-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for shared-mime-info (1.2-0ubuntu3) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Setting up libgsoap4:amd64 (2.8.16-2) ...
 Setting up virtualbox (4.3.10-dfsg-1) ...
 * Stopping VirtualBox kernel modules
   ...done.
 * Starting VirtualBox kernel modules
 * No suitable module for running kernel found
   ...fail!
 Setting up dkms (2.2.0.3-1.1ubuntu5.14.04) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up virtualbox-dkms (4.3.10-dfsg-1) ...
 Loading new virtualbox-4.3.10 DKMS files...
 First Installation: checking all kernels...
 Building for 3.13.0-32-generic and 3.13.0-43-generic
 Building initial module for 3.13.0-32-generic
 Done.

 vboxdrv:
 Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-32-generic/updates/dkms/

 vboxnetadp.ko:
 Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-32-generic/updates/dkms/

 vboxnetflt.ko:
 Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-32-generic/updates/dkms/

 vboxpci.ko:
 Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-32-generic/updates/dkms/

 depmod.......

 DKMS: install completed.
 Building initial module for 3.13.0-43-generic
 Done.
 vboxdrv:
 Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-43-generic/updates/dkms/

 vboxnetadp.ko:
  Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-43-generic/updates/dkms/

 vboxnetflt.ko:
 Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-43-generic/updates/dkms/

 vboxpci.ko:
 Running module version sanity check.
 - Original module
   - No original module exists within this kernel
 - Installation
   - Installing to /lib/modules/3.13.0-43-generic/updates/dkms/

 depmod.........

 DKMS: install completed.
 * Stopping VirtualBox kernel modules
   ...done.
 * Starting VirtualBox kernel modules
   ...done.
 Setting up virtualbox-qt (4.3.10-dfsg-1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 Temp File /tmp/ptconfigure-temp-script-27415379023.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Virtualbox: Success
 ------------------------------
 Installer Finished
 ******************************


options
--------------


.. cssclass:: table-bordered

 +-------------------------------+---------------+---------------------------------------+----------------------------------+
 | paramètres			 | options	 | paramètres alternatifs		 | commentaires			    |
 +===============================+===============+=======================================+==================================+
 |Install virtual box?(Y/N)	 | Yes		 | Au lieu d'utiliser VirtualBox ,       | Installé avec succès sous        |
 |				 |		 | l'utilisateur peut utiliser la boîte	 | module de ptvirtualize	    |
 |                               |               | virtuelle                             |                                  |
 +-------------------------------+---------------+---------------------------------------+----------------------------------+
 |Install virtual box?(Y/N)	 | No		 | Au lieu d'utiliser VirtualBox ,       | Quittez l'écran                  |
 |				 |		 | l'utilisateur peut utiliser la boîte  |				    |
 |                               |               | virtuelle|                            |                                  |
 +-------------------------------+---------------+---------------------------------------+----------------------------------+




Avantages
---------------

* Voix peut être installé via ce module. 
* Les images ISO et les périphériques physiques connectés hôte peuvent
  être montés en tant que lecteurs de CD/DVD. 
* L'image du DVD d'une distribution Linux peut être téléchargé et utilize
  directement par VirtualBox.
 


