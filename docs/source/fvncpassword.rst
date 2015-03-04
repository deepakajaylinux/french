============
VNCPasswd
============

synopsis
----------------

L'utilitaire vncpasswd devrait être utilisé pour créer et modifier les mots de passe pour l'authentification du serveur VNC. Il utilise ces mots de passe lors du démarrage avec le gestionnaire de bureau local lors du démarrage à partir du script de serveur VNC. vncpasswd permet d'entrer un ou deux mots de passe. L'utilitaire vncpasswd demande interactive si elle doit régler le deuxième mot de passe. Ce est plus à l'aise ubunt et CentOS.

Commande Aide
----------------------

Aide commande comprend un vaste système d'aide basée sur la console, qui rappelle de pages de manuel dans Ubuntu. Les rubriques d'aide comprennent l'aide pour l'installation du passward pour la zone locale ou distante. Simple d'écrire les commandes sans arguments.

.. code-block:: bash

                ptconfigure  VNC-passwd help

La capture d'écran suivante peut visualiser.

.. code-block:: bash

 kevell@corp:/# ptconfigure VNCPasswd help

 ******************************


  This command allows you to install VNCPasswd, the popular Remote/Local Desktop Manager Solution.

  VNCPasswd, vncpasswd, vnc-passwd

        - install
        Installs VNCPasswd through a package manager
        example: ptconfigure vnc install

 ------------------------------
 End Help
 ******************************


installation
-----------------

Installation permet à l'utilisateur d'installer vncpassward. Il est très populaire dans Remote Desktop ou local. Ce installer le passwd vnc travers package manager.The premier mot de passe est une primaire, le second mot de passe peut être utilisé pour une vue seule authentication.It est à l'aise avec Ubuntu et CentOS.
 
.. code-block:: bash

                ptconfigure  VNC-passwd install

Après clé dans la commande du système peut demander à l'utilisateur pour l'entrée. Si l'entrée de l'utilisateur que Y, il peut installer le VNCpassward bien il peut sortir. capture d'écran suivante peut visualiser.

.. code-block:: bash

 kevell@corp:/# ptconfigure VNC-passwd install

 Install VNCPasswd? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNCPasswd !        *
 *******************************
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 The following NEW packages will be installed:
  expect
 0 upgraded, 1 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package expect from the Packager Apt did not execute correctly
 Enter VNC User:

 Enter VNC Pass:

 Creating /tmp/ptconfigure-temp-script-40114506906.sh
 chmod 755 /tmp/ptconfigure-temp-script-40114506906.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-40114506906.sh Permissions
 Executing /tmp/ptconfigure-temp-script-40114506906.sh
 sudo: unknown user: /usr/bin/expect
 sudo: unable to initialize policy plugin
 Temp File /tmp/ptconfigure-temp-script-40114506906.sh Removed
 [Pharaoh Logging] Removing Package expect
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Package 'expect' is not installed, so not removed
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 0 upgraded, 0 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Package expect from the Packager Apt is not installed, so not removed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNCPasswd: Success
 ------------------------------
 Installer Finished
 ******************************

Options
---------------

.. cssclass:: table-bordered

 +---------------------------+--------------------------------------------+--------------+--------------------------------------------+
 | paramètre                 | Alternative Paramètre                      | Option       | Kommentare                                 |
 +===========================+============================================+==============+============================================+
 |Install VNCpasswd? (Y/N)   | Au lieu d'utiliser vncpasswd nous pouvons  | Y            | il va installer VNCPassward sous           |
 |                           | utiliser VNCPasswd,vncpasswd,vnc-passward  |              | ptconfigure                                |
 +---------------------------+--------------------------------------------+--------------+--------------------------------------------+
 |Install VNCpasswd? (Y/N)   | Au lieu d'utiliser vncpasswd nous pouvons  | N            | La sortie du système d'installation        |
 |                           | utiliser VNCPasswd,vncpasswd,vnc-passward| |              |                                            |
 +---------------------------+--------------------------------------------+--------------+--------------------------------------------+



avantages
-----------------

* Support multi-langue
* Authentification VNC
* Performances optimisées
* Le transfert de fichiers est possible
* Stratégies de déploiement puissantes
