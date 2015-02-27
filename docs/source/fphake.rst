==============
Phake
==============

synopsis
-------------

Phake est un cadre moqueur pour PHP. Il permet la création d'objets qui imitent un objet réel d'une manière prévisible et contrôlée. Cela vous permet de traiter les appels de méthode externes faites par votre système sous test (SUT) comme une autre forme d'entrée à votre SUT et la sortie de votre SUT. Cela se fait en écrasant méthodes qui fournissent entrée indirecte dans votre test et en vérifiant les paramètres des méthodes qui reçoivent sortie indirecte de votre test.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module Phake. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure Phake help


 kevell@corp:/# ptconfigure Phake help
 ******************************


  This command allows you to install or update Phake.

  Phake, phake

        - install
        Installs the latest version of phake
        example: ptconfigure phake install

        - ensure
        Installs the latest version of phake, only if a version is not installed
        example: ptconfigure phake ensure

 ------------------------------
 End Help
 ******************************


installation
----------------

Lorsque l'utilisateur doit installer Phake dans la machine, la commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
         
   	        ptconfigure Phake install
 


Le système demande le nom du répertoire, si vous veut mettre en place votre PATH, vous pouvez définir votre chemin. Définissez votre chemin suivi par le symbole «/». Appuyez sur Entrée se il n'y a aucun changement à faire.

"What is the program data directory? Found "/opt/phake" - use this?

Ensuite, le système demande pour exécuter nom de répertoire, si vous veut mettre en place votre PATH, vous pouvez définir votre chemin. Définissez votre chemin suivi par le symbole «/». Appuyez sur Entrée se il n'y a aucun changement à faire

"What is the program executer directory? Found "/usr/bin" - Use this? "

Montre le même écran ci-dessous.

.. code-block:: bash

 kevell@corp:/# ptconfigure Phake install
 Install Phake ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          Phake         *
 *******************************
 What is the program data directory? Found "/opt/phake" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'http://github.com/jaz303/phake.git'  /tmp/phake/phakeCloning into '/tmp/phake/phake'...
 remote: Counting objects: 552, done.
 remote: Total 552 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (552/552), 91.36 KiB | 76.00 KiB/s, done.
 Resolving deltas: 100% (314/314), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Phake: Success
 ------------------------------
 Installer Finished
 ******************************


Options
-----------                               

.. cssclass:: table-bordered


 +---------------------+---------------------------------------------+---------------+----------------------------------------------+
 | paramaters          | Alternative Paramètre                       | options       | commentaires                                 |
 +=====================+=============================================+===============+==============================================+
 |ptconfigure Phake    | Chacun des deux paramètre alternatif peut   | Y             | Une fois que l'utilisateur fournit l'option, |
 |Install              | être utilisé dans commandement Phake, phake |               | système démarre processus d'installation     |
 |                     | par exemple: ptconfigure phake Install      |               |                                              |
 +---------------------+---------------------------------------------+---------------+----------------------------------------------+
 |ptconfigure Phake    | Chacun des deux paramètre alternatif peut   | N             | Une fois que l'utilisateur fournit l'option, |
 |Install              | être utilisé dans commandement Phake, phake |               | le système se arrête processus               |
 |                     | par exemple: ptconfigure phake Install      |               | d'installation|                              |
 +---------------------+---------------------------------------------+---------------+----------------------------------------------+

avantages
----------

* Phake est une grande bibliothèque moqueur et peut être facilement intégré dans PHPUnit.
* Sa nouvelle approche de simulacres et les talons prototypes et la séparation entre Stubbing et de vérification phases est très 
  rafraîchissant et facile à utiliser.
