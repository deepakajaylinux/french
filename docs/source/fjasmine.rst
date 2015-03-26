===============
Jasmine
===============

synopsis
---------

Jasmine est un cadre de développement piloté par comportement pour tester le code JavaScript.  Jasmine est une source européenne, framework JavaScript de tests.  Il ne s'appuie pas sur les navigateurs, DOM ou n'importe quel framework JavaScript. Ainsi, il est adapté pour les sites Web, projets de Node.js, ou n'importe où ce JavaScript peut fonctionner.

Commande Aide
--------------

Cette commande permet de déterminer l'utilisation du module de jasmin. Il énumère les paramètres alternatifs de jasmin. Il décrit également la syntaxe pour le fonctionnement du module de jasmin. La commande help pour Jasmin s'affiche comme ci-dessous.

.. code-block:: bash

        ptconfigure Jasmine  help

La représentation picturale de la commande ci-dessus est listée ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure Jasmine help
 ******************************


  This command allows you to install Jasmine from a GC Repo.

  Jasmine

        - install
        Installs the latest GC Repo version of Jasmine.
        example: ptconfigure Jasmine install

 ------------------------------
 End Help
 ******************************


installation
---------------

La commande utilisée pour l'installation du module jasmin sur le terminal est répertoriée ci-dessous,


.. code-block:: bash

        ptconfigure Jasmine install

La commande ci-dessus a pour but d'installer la dernière version de jasmin et de ses dépendances...

La représentation picturale de la commande ci-dessus est listée ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure jasmine install
 Install Jasmine? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Jasmine        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79546324044.sh
 chmod 755 /tmp/ptconfigure-temp-script-79546324044.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79546324044.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79546324044.sh
 Cloning into 'jasmine'...
 remote: Counting objects: 12178, done.
 remote: Total 12178 (delta 0), reused 0 (delta 0), pack-reused 12178
 Receiving objects: 100% (12178/12178), 6.60 MiB | 8.00 KiB/s, done.
 Resolving deltas: 100% (7866/7866), done.
 Checking connectivity... done.
 Archive:  jasmine-standalone-2.0.0.zip
  inflating: MIT.LICENSE             
  inflating: lib/jasmine-2.0.0/jasmine_favicon.png  
  inflating: lib/jasmine-2.0.0/jasmine.js  
  inflating: lib/jasmine-2.0.0/jasmine-html.js  
  inflating: lib/jasmine-2.0.0/jasmine.css  
  inflating: lib/jasmine-2.0.0/console.js  
  inflating: lib/jasmine-2.0.0/boot.js  
  inflating: SpecRunner.html         
  inflating: src/Player.js           
  inflating: src/Song.js             
  inflating: spec/PlayerSpec.js      
  inflating: spec/SpecHelper.js      
 Temp File /tmp/ptconfigure-temp-script-79546324044.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jasmine: Success
 ------------------------------
 Installer Finished
 ******************************


objectifs
-----------

* Elle doit encourager les bonnes pratiques d'essais 
* il doit être simple à démarrer avec 
* il devrait s'intégrer facilement aux systèmes de build continu




