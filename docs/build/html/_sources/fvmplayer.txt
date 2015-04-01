===============
VMWarePlayer
===============

synopsis
----------------

VMPlayer peut fonctionner appliances virtuelles existantes et de créer ses propres machines virtuelles (qui nécessitent un système d'exploitation doit être installé pour être fonctionnel). Il utilise le même noyau de virtualisation comme VMware Workstation, un programme similaire avec plus de fonctionnalités, mais pas gratuitement. VMware Player est disponible en ptconfigure. Il est adapté avec Ubuntu et CentOS.

Commande Aide
-----------------------

Cette commande help guide l'utilisateur pour créer joueur de machine virtuelle. Spécialisée dans ptconfigure. Fournit également des fonctionnalités pour la machine virtuelle
joueur.

La commande d'aide pour VMplayer est illustré ci-dessous.

.. code-block:: bash
		
	ptconfigure VMWarePlayer help

Après les entrées de commande ci-dessus, il commence à fonctionner pour créer le cadre de joueur. Il catéchèse les fonctions de vmplayer dans les captures d'écran.

installation
-----------------

 L'installation de vmplayer nécessaire pour rendre l'installation dans une version mise à jour. Ce est un processus manifeste pour installer le module de vmplayer sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

	ptconfigure VMWarePlayer install


Après dynamiser la commande il catéchiser entrée.

Lorsque l'entrée de l'utilisateur que oui il va installer automatiquement vmplayer avec la vérification du système. Si pas quitter l'installation. La capture d'écran suivante démontre vmplayer et ses fonctions.

option
------------

.. cssclass:: table-bordered

 +---------------------------+---------------------------------------------+-------------+----------------------------------------------+
 | paramètres                | Autres  Paramètres                          | options     | Commentaires                                 |
 +===========================+=============================================+=============+==============================================+
 |Install vmplayer?(Y/N)     | Au lieu d'utiliser vmplayer nous pouvons    | Y           | Il va installer vmplayer sous ptconfigure    |
 |                           | utiliser VMPlayer, VM-player                |             | dans Pharaoh tools                           |
 +---------------------------+---------------------------------------------+-------------+----------------------------------------------+
 |Install vmplayer?(Y/N)     | Au lieu d'utiliser vmplayer nous pouvons    | N           | La sortie du système d'installation          |
 |                           | utiliser VMPlayer, VM-player|               |             |                                              |
 +---------------------------+---------------------------------------------+-------------+----------------------------------------------+

.. code-block:: bash

 kevell@corp:/# ptconfigure VMWarePlayer install
 Install VMWarePlayer? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! VMWare Player !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-7944529549.sh
 chmod 755 /tmp/ptconfigure-temp-script-7944529549.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-7944529549.sh Permissions
 Executing /tmp/ptconfigure-temp-script-7944529549.sh
 --2015-03-26 10:24:11--  https://download3.vmware.com/software/player/file/VMware-Player-7.0.0-2305329.x86_64.bundle
 Resolving download3.vmware.com (download3.vmware.com)... 23.65.99.51, 2600:1411:0:193::2ef, 2600:1411:0:1a0::2ef, ...
 Connecting to download3.vmware.com (download3.vmware.com)|23.65.99.51|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 210911382 (201M) [application/x-octet-stream]
 Saving to: â€˜VMware-Player-7.0.0-2305329.x86_64.bundleâ€™ 

 100%[======================================================================================================>] 21,09,11,382 44.1KB/s   in 2h
 36m 

 2015-03-26 13:01:08 (21.9 KB/s) - â€˜VMware-Player-7.0.0-2305329.x86_64.bundleâ€™ saved [210911382/210911382]


 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine", 

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",
 Gtk-Message: Failed to load module "canberra-gtk-module": libcanberra-gtk-module.so: cannot open shared object file: No such file or directory
 Extracting VMware Installer...done.
 Temp File /tmp/ptconfigure-temp-script-7944529549.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VMWarePlayer: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
----------------

* Exécutez les appliences virtuels existants et de créer la machine virtuelle
* Non sensible à la casse
* Convient pour Ubuntu et Cent OS
* Utilisé pour tous les types de professionnels
