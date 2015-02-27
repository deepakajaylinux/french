=======
PHPAPC
=======

synopsis
-------------

Ce module vise à installer le PHP APC à la machine des utilisateurs de toutes les manières possibles.

APC est l'un des mécanisme de cache le plus populaire pour les op-code de la mise en cache de PHP. Une fois activé, il commence la mise en cache codes PHP automatiquement. Il travaille aussi bien avec le plugin W3 Total Cache pour stocker l'objet et MySQL caches.

Les thèmes à venir seront guide votre entièrement dans tous les aspects impliqués dans l'installation du PHP APC.



Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module PHP APC. Il énumère les alternatives aux paramètres du module Php APC. Il décrit également la syntaxe pour l'installation du module Php APC. La commande d'aide pour le module PHP APC est représentée ci-dessous.

.. code-block:: bash
	
		ptconfigure PHPAPC help


La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide sous PHP APC.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPAPC help

 ******************************


  This command allows you to install some common and helpful PHP APC.

  PHPAPC, php-apc, phpapc, phpapc

        - install
        Install PHP APC.
        example: ptconfigure phpapc install

 ------------------------------
 End Help
 ******************************



installation
----------------

La commande utilisée pour installer le Php APC dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash
	
		ptconfigure phpapc install


Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +----------------------------+------------------------------------+--------------+--------------------------------------------+
 | paramètres		      | Alternative Paramètre		   | options	  | commentaires                               |
 +============================+====================================+==============+============================================+
 |Install PHP APC? (Y/N)      | Au lieu de phpapc , nous pouvons   | Y(Yes)       | Si l'utilisateur souhaite procéder de la   |
 |			      | utiliser PHPAPC, php-apc.          |		  | processus d'installation qu'ils peuvent    |
 |                            |                                    |              | entrée comme Y                             |
 +----------------------------+------------------------------------+--------------+--------------------------------------------+
 |Install PHP APC? (Y/N)      | Au lieu de phpapc , nous pouvons   | N(No)        | Si l'utilisateur souhaite quitter le       |
 |                            | utiliser PHPAPC, php-apc.          |              | processus d'installation qu'ils peuvent    |
 |                            |                                    |              | entrée comme N|                            |
 +----------------------------+------------------------------------+--------------+--------------------------------------------+



Si l'utilisateur procède à l'installation, au cours du processus d'installation est décrite dans les listes ci-dessous:


* Lit listes de paquets.
* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les paquets qui sont automatiquement installés.
* Liste aboutissants de l'emballage supplémentaire que installez.
* Liste outs les forfaits proposés.
* Liste outs les nouveaux paquets qui installent.
* Les détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.


Enfin, le processus d'installation se rempli. Représenter visuellement la capture d'écran qui suit le processus d'installation du PHP APC.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpapc install

 Install PHP APC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP APC!        *
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
 The following extra packages will be installed:
  php5-apcu
 The following packages will be REMOVED:
  php5-xcache
 The following NEW packages will be installed:
  php-apc php5-apcu
 0 upgraded, 2 newly installed, 1 to remove and 78 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPAPC: Success
 ------------------------------
 Installer Finished
 ******************************


Fonctions APC
------------------


Cette sous-thèmes offres avec les fonctions les plus fréquemment utilisées sous APC. Tout en travaillant avec PHP APC l'utilisateur peut se référer à ces fonctions de APC.

* Apc_add - cache une nouvelle variable dans le magasin de données
* Apc_bin_dump - Obtenez un vidage binaire des fichiers donnés et variables utilisateur
* Apc_bin_dumpfile - Sortie d'un vidage binaire des fichiers mis en cache et variables utilisateur dans un fichier
* Apc_bin_load - Charger un vidage binaire dans le cache de fichiers APC / utilisateur
* Apc_bin_loadfile - Charger un vidage binaire d'un fichier dans le cache de fichiers de APC / utilisateur
* Apc_cache_info - Récupère les informations du cache du magasin de données d'APC
* Apc_cas - met à jour une ancienne valeur avec une nouvelle valeur
* Apc_clear_cache - Efface le cache APC
* Apc_compile_file - Stocke un fichier dans le cache de bytecode, évitant tous les filtres.
* Apc_dec - Diminuer un numéro enregistré
* Apc_define_constants - Définit un ensemble de constantes pour la récupération et la définition de masse
* Apc_delete_file - Supprime les fichiers du cache opcode
* Apc_delete - Efface une variable stockée dans le cache
* apc_exists - Vérifie si la clé existe APC
* Apc_fetch - Récupère une variable stockée dans le cache
* Apc_inc - Augmenter un numéro enregistré
* apc_load_constants - Charge un jeu de constantes depuis le cache
* Apc_sma_info - Récupère les informations d'allocation mémoire partagée d'APC
* Apc_store - cache une variable dans le magasin de données



Avantages
-----------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce module de volonté installe le apc php dans la version mise à jour.
* Si le module existe déjà dans la machine de l'utilisateur, il affiche un message comme il est déjà existant.
* APC est livré avec fichier nommé apc.php, qui fournit une interface Web simple.
