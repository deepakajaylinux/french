=================
PackageManager
=================

synopsis
----------------

Cette commande utilisé pour envelopper la gestion des paquets. Ce est d'avoir trois options. Ils sont PKG-installer, pkg-assurer, pkg-remove. Cela permet à l'utilisateur d'installer dans ne importe quel système. Il gérer les fonctions package Manager. Il convient de travailler avec Ubuntu et CentOS.

Commande Aide
--------------

Cette commande help guide l'utilisateur à installer, assurer, retirez gestion des paquets. Cela permet l'installation, assurez, retirez. La commande d'aide pour le gestionnaire de paquets est illustré ci-dessous.

.. code-block:: bash

		ptconfigure packagemanager help

Après les entrées de commande ci-dessus, il commence à fonctionner pour envelopper. Il catéchèse les fonctions dans les captures d'écran.

.. code-block:: bash

 kevell@corp:/# ptconfigure packagemanager help
 ******************************


  This command allows you to use a Package Management wrapper.

  PackageManager, package-manager, packagemanager, package-mgr, pkgmgr

        - pkg-install
        Installs a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

        - pkg-ensure
        Installs a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

        - pkg-remove
        Removes a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

  A package manager wrapper that will allow you to install packages on any system

 ------------------------------
 End Help
 ******************************



paramètres alternatifs
--------------------------------

Voici les autres paramètres qui peuvent être définis dans les déclarations:

PackageManager, package-manager, packagemanager, pkgmgr, package-mgr.

Pkg-installer
---------------

L'installation comprend l'installation de PackageManager nécessaire pour faire l'installation dans une version mise à jour. Ce est un processus manifeste pour installer le module PackageManager sous ptconfigure. PackageManager en utilisant simplement la commande ci-dessous,

.. Code-block:: bash

	ptconfigure PackageManager Install

Après dynamiser la commande il catéchiser entrée.

Lorsque l'entrée d'utilisateur comme il sera automatiquement oui installer PackageManager avec vérification du système. Si pas quitter l'installation. La capture d'écran suivante démontre PackageManager et ses fonctions.

.. code-block:: bash


Pkg-assurer
-----------------

Pkg assurer un système service se exécute. En cas de non exécution démarrer d'autre ne essayez pas. Grâce à cette commande, l'utilisateur peut déterminer si le système fonctionne ou ralenti. Des commandes simples sont faciles à manipuler. La commande suivante permet d'assurer, par le gestionnaire de paquets.

.. code-block:: bash
    
	ptconfigure PackageManager ensure


Pkg-remove
-----------------

Pkg retirer commande utilisée pour supprimer un paquet de gestionnaire de paquets. Le gestionnaire de paquets vérifie d'abord le paquet à supprimer du gestionnaire de paquets. Ensuite, il demande confirmation. Ensuite, utilisez l'option de suppression.

.. code-block:: bash

 		ptconfigure PackageManager remove

avantages
-------------

* Sensibilité non de cas.
* Eh bien-to-do dans Ubuntu et CentOS.
* Supprimer le paquet est possible.
* Enroulez le gestionnaire de paquets.
* Les commandes sont simples à utilizer.

