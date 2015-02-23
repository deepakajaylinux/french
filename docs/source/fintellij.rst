==========
IntelliJ
==========


Synopsis
------------

Ce module d'accélérer l'installation d'IntelliJ qui est un Brains Jet IDE avec une dernière version. La plateforme IntelliJ est une plate-forme pour la construction, les IDE intelligents linguistiques-courant avec un ensemble complet de composants, qui comprend système virtuel de fichiers, le cadre de l'assurance-chômage, éditeur de texte, lexing, analyse, arbres de syntaxe abstraite et d'autres infrastructures spécifique à la langue, les cadres de mise en œuvre navigation, la complétion de code, les inspections, les intentions, refactoring, l'intégration de contrôle de version, cadre de débogueur, graphique coureur de test unitaire.

Le code source plateforme IntelliJ est couvert par la licence Apache 2.0. Cela signifie que vous pouvez construire à la fois open source et des produits commerciaux au-dessus de la plate-forme sans payer de redevances à JetBrains. Voyons sur les fonctionnalités de ce module sous IntelliJ.

Commande Aide
-----------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module IntelliJ. Il énumère les alternatives aux paramètres du module IntelliJ. Il décrit également la syntaxe pour l'installation du module IntelliJ. La commande d'aide pour le module IntelliJ est représentée ci-dessous.

.. code-block:: bash

 		ptconfigure IntelliJ help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu IntelliJ.

.. code-block:: bash

 kevell@corp:/# ptconfigure IntelliJ help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  IntelliJ, intellij

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************


installation
---------------

La commande utilisée pour installer le JRush à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash

		ptconfigure IntelliJ install

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit:

* Il demande à l'utilisateur d'entrer la version d'IntelliJ.
* Assurer la disponibilité des modules et non vérifie la version.
* Si le module ne existe pas dans la machine de l'utilisateur, il commence l'installation.
* Lors de l'installation il sera demande à l'utilisateur d'entrer dans le répertoire d'installation de Java.

Enfin, l'installation d'IntelliJ se rempli. Représente le processus d'installation IntelliJ La capture d'écran comme indiqué ci-dessous.

.. code-block:: bash

 kevell@corp:/# ptconfigure IntelliJ install
 Install IntelliJ IDE? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         IntelliJ IDE        *
 *******************************
 Enter IntelliJ Version
 PHP Notice:  Undefined offset: 0 in /opt/ptconfigure/ptconfigure/src/Core/Base/Model/Base.php on line 187
 (0)  
 PHP Notice:  Undefined offset: 1 in /opt/ptconfigure/ptconfigure/src/Core/Base/Model/Base.php on line 187
 (1)  

 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-98824051629.sh
 chmod 755 /tmp/ptconfigure-temp-script-98824051629.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-98824051629.sh Permissions
 Executing /tmp/ptconfigure-temp-script-98824051629.sh
 Cloning into 'intellij'...
 remote: Counting objects: 1026, done.
 remote: Total 1026 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (1026/1026), 205.06 MiB | 410.00 KiB/s, done.
 Resolving deltas: 100% (60/60), done.
 Checking connectivity... done.
 Checking out files: 100% (744/744), done.
 Temp File /tmp/ptconfigure-temp-script-98824051629.sh Removed
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 IntelliJ: Success
 ------------------------------
 Installer Finished
 ******************************

paramètres
----------------------------

Au lieu d' IntelliJ nous pouvons utiliser, intellij

avantages
------------


* Ce module facilite l'utilisateur dans l'installation IntelliJ avec la dernière version.
* Les paramètres utilisés pour déclarer l'aide et les installations ne sont pas sensibles à la casse, qui est ajouté tout avantage par rapport 
  aux autres.
* Il est bien de choses à faire dans les deux cent OS et ainsi que dans ubuntu.
* Le statut requis sont clairement surveillée lors de l'installation.
* Lors de l'installation, l'utilisateur peut saisir la version requise et ainsi que Java Installez Directory.
