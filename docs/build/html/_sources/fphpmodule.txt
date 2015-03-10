===========
PHPModules
===========

synopsis
-------------

Ce Modules vise à installer et enveloppant certains des modules PHP communs et utiles, soutenir. Quelques exemples sont: php5-gd l'libs d'image, php5-libs imagick l'image, php5-curl la manipulation libs, php5-mysql les libs pour la gestion des connexions mysql fichier distant. Voyons comment utiliser ce module, le processus d'installation dans les prochains sujets.

Commande Aide
----------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module PHP. Il énumère les alternatives aux paramètres du module PHP. Il décrit également la syntaxe pour installer le module PHP. La commande d'aide pour le module PHP est représentée ci-dessous.

.. code-block:: bash
	
		ptconfigure PHPModules help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide pour le module PHP.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPModules help

 ******************************


  This command allows you to install some common and helpful PHP Modules.

  PHPModules, php-mods, phpmods, php-modules, phpmodules

        - install
        Installs some common PHP Modules. These include php5-gd the image libs,
        php5-imagick the image libs, php5-curl the remote file handling libs,
        php5-mysql the libs for handling mysql connections.
        example: ptconfigure phpmods install

 ------------------------------
 End Help
 ******************************


installation
--------------

La commande utilisée pour installer les modules php dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash

		ptconfigure phpmods install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +---------------------------+----------------------------------------------+-----------+--------------------------------------------+
 | paramètres                | paramètre alternatif                         | option    | commentaires                               |
 +===========================+==============================================+===========+============================================+
 |Install PHP Modules?(Y/N)  | au lieu de phpmods nous pouvons utiliser     | Yes       | Si l'utilisateur souhaite procéder à       |
 |                           | PHPModules, php-mods, php-modules,           |           | l'installation processus, ils peuvent      |
 |                           | phpmodules aussi                             |           | entrée comme Y                             |
 +---------------------------+----------------------------------------------+-----------+--------------------------------------------+
 |Data directory             | au lieu de phpmods nous pouvons utiliser     | No        | Si l'utilisateur souhaite quitter le       |
 |                           | PHPModules, php-mods, php-modules,           |           | d'installation qu'ils peuvent entrée comme |
 |                           | phpmodules aussi.                            |           | N.|                                        |
 +---------------------------+----------------------------------------------+-----------+--------------------------------------------+

	

Si l'utilisateur procède à l'installation, au cours du processus d'installation est décrite dans les listes ci-dessous:


* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les paquets qui sont automatiquement installés.
* Liste outs les nouveaux paquets qui installent.
* Détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.


La capture d'écran ci-dessous représente graphiquement le processus décrit ci-dessus de l'installation.
.. code-block:: bash


 kevell@corp:/# ptconfigure phpmods install
 
 Install PHP Modules? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mods!        *
 *******************************
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-gd from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-imagick from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-curl from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mysql from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcache from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mongo from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPModules: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
------------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Tout l'installation fréquemment utilisé des modules php se enveloppait dans un processus unique.

