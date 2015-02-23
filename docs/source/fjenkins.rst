==============
Jenkins
==============

synopsis
-------------

Jenkins est populaire pour construire serveur. Jenkins est un outil d'intégration continue open source écrit en Java. Jenkins fournit des services d'intégration continue pour le développement logiciel. Il se agit d'un système en fonctionnement sur serveur dans un conteneur de servlet comme Apache Tomcat.

La fonctionnalité et la flexibilité de base de Jenkins lui permettent de se intégrer dans une variété d'environnements et peut aider à rationaliser le processus de développement pour tous les acteurs impliqués

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module Jenkins. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande.

.. code-block:: bash
             
		ptconfigure jenkins help

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash



 
 kevell@corp:/# ptconfigure jenkins help
 ******************************


 This command allows you to install Jenkins, the popular Build Server.

 Jenkins, jenkins

 - install
 Installs Jenkins through apt-get
 example: ptconfigure jenkins install

 ------------------------------
 End Help
 ******************************



installation
----------------

Si l'utilisateur doit installer le module Jenkins dans la machine, la commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
              
	        ptconfigure jenkins install


Est listé ci-dessous la capture d'écran de la commande ci-dessus,

.. code-block:: bash


 kevell@corp:/# ptconfigure jenkins install
 Install Jenkins? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Jenkins !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-14615194352.sh
 chmod 755 /tmp/ptconfigure-temp-script-14615194352.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-14615194352.sh Permissions
 Executing /tmp/ptconfigure-temp-script-14615194352.sh
 E: Could not get lock /var/lib/apt/lists/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/lib/apt/lists/
 OK
 Temp File /tmp/ptconfigure-temp-script-14615194352.sh Removed
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:
 
 The following packages have unmet dependencies:
 jenkins : Depends: daemon but it is not installable
           Depends: default-jre-headless but it is not installable or
                    java-runtime-headless
 [Pharaoh Logging] Adding Package jenkins from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jenkins: Success
 ------------------------------
 Installer Finished
 ******************************


options
-----------

.. cssclass:: table-bordered

 +----------------------------+--------------------------------------+------------+-------------------------------------------------+
 | Paramètres                 | alternative paramètres               | Option     | Commentaires                                    |
 +============================+======================================+============+=================================================+
 |ptconfigure Jenkins Install | Au lieu d'utiliser Jenkins,          | Y(Yes)     | Une fois que l'utilisateur fournit l'option,    |
 |                            | l'utilisateur peut ajouter jenkins   |            | système démarre processus d'installation        |
 +----------------------------+--------------------------------------+------------+-------------------------------------------------+
 |ptconfigure Jenkins Install | Au lieu d'utiliser Jenkins,          | N(No)      | Une fois que l'utilisateur fournit l'option,    |
 |                            | l'utilisateur peut ajouter jenkins   |            | le système se arrête processus d'installation|  |
 +----------------------------+--------------------------------------+------------+-------------------------------------------------+


avantages
--------------

* Détection de bug immédiate
* Aucune étape d'intégration dans le cycle de vie
* Un système déployable à un moment donné
* Enregistrement de l'évolution du projet
