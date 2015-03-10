==================
RubySystem
==================

synopsis
------------

Ruby est un système, de réflexion, de haut niveau langage dynamique de script. Ruby système ne est pas seulement pour le développement d'applications Web en collaboration avec le Ruby RVM. Il peut également être utilisé comme un puissant comme un langage de script et une très bonne alternative à l'écriture de scripts shell habituelle, couramment utilisé pour atteindre les besoins de script dans les systèmes adminstration.Set de modules intégrés et quelques bibliothèques externes, le système peut faire Ruby systèmes adminstration plus efficient.Ruby système est un outil très utile et puissant qui est un must have dans toolbox.It de chaque administrateur système est à l'aise avec Ubuntu et Cent OS.

Commande Aide
--------------------

Cette commande peut fonctionner sur les objectifs et les commandes disponibles dans le module de système Ruby. Il explique également la commande pour installer le système Ruby. Avant l'installation, l'utilisateur peut lire cette commande d'aide explique sa fonction.

.. code-block:: bash
        
		ptconfigure RubySystem help


L'image suivante vous aide également à comprendre clairement ce module.

.. code-block:: bash

 kevell@corp:/# ptconfigure RubySystem help
 ******************************


  This command allows you to install Ruby RVM, the system wide version.

  RubySystem, rubysystem, ruby-system, rubysys

        - install
        Installs Ruby a System Wide version of Ruby for you
        example: ptconfigure ruby-rvm install

  Ruby is installed the recommended per-user way. To use ruby after the install
  first run "source ~/.rvm/scripts/rvm" to get access to the Ruby install for
  your user, then "rvm install 1.9.3" (to install, specify version as needed)
  then "rvm use 1.9.3" (to select your default version for the session)

 ------------------------------
 End Help
 ******************************


installation
-------------------

Ce est un processus flagrante à installer le module de système Ruby sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash
        
                ptconfigure rubysystem install

Après clé dans la commande, il peut demande

Installer Ruby, l'ensemble du système? (Y / N)

Dans le cas où l'entrée d'utilisateur en tant que Y, on peut installer Rubysystem de l'emballage. Sinon, il peut quitter l'écran. Les captures d'écran suivantes peuvent expliquer il.

.. code-block:: bash


 kevell@corp:/# ptconfigure RubySystem install
 
 Install Ruby, System Wide? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Ruby System!        *
 *******************************

 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  ruby1.9.1-examples ri1.9.1 graphviz ruby1.9.1-dev
 The following NEW packages will be installed:
  ruby1.9.1
 0 upgraded, 1 newly installed, 0 to remove and 12 not upgraded.
 1 not fully installed or removed.
 Need to get 37.5 kB of archives.
 After this operation, 240 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main ruby1.9.1 amd64 1.9.3.0-1ubuntu1 [37.5 kB]
 Fetched 37.5 kB in 7s (5232 B/s)
 Selecting previously unselected package ruby1.9.1.
 (Reading database ... 282890 files and directories currently installed.)
 Preparing to unpack .../ruby1.9.1_1.9.3.0-1ubuntu1_amd64.deb ...
 Unpacking ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up zend-server-php-5.3 (6.1.0+b1177) ...
 Module php5 already enabled
 Module rewrite already enabled
 Site zendserver_gui already enabled
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0
 Content-type: text/html

 Setting up ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 update-alternatives: using /usr/bin/gem1.9.1 to provide /usr/bin/gem (gem) in auto mode
 [Pharaoh Logging] Adding Package ruby1.9.1 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 RubySystem: Success
 ------------------------------
 Installer Finished
 ******************************




Options
--------------


.. cssclass:: table-bordered

 +-----------------------+--------------------------------------------+--------------+--------------------------------------+
 | paramètres            | Autres paramètres                          | Option       | commentaires                         |
 +=======================+============================================+==============+======================================+
 |ptconfigure Rubysystem | Au lieu d'utiliser RubySystem, rubysystem, | Y            | Le système démarre l'installation    |
 |Install?(Y/N)          | ruby-system, rubysys.                      |              |                                      |
 +-----------------------+--------------------------------------------+--------------+--------------------------------------+
 |ptconfigure Rubysystem | Au lieu d'utiliser RubySystem, rubysystem, | N            | Le système se arrête le processus    |
 |Install?(Y/N)          | ruby-system, rubysys.                      |              | d'installation|                      |
 +-----------------------+--------------------------------------------+--------------+--------------------------------------+

benifits
---------

* Système Ruby est un, de réflexion, de haut niveau langage de script dynamique pour la programmation orientée objet rapide et facile.
* Dans le système Ruby, est un outil pratique et agréable. Y compris les outils qui sont utilisés dans le processus de déploiement.
* Le système Ruby est déjà un professionnel ayant les connaissances extrême expérimenté à la fois dans le développement web et du génie logiciel  générale compétences.
* Le principal avantage du langage de programmation Ruby Ruby et le système est considéré comme étant la vitesse de développement.
