================
Ubuntu Compiler
================

synopsis
----------

Ce module revitaliser programme de c. Ubuntu et autres distributions Linux disposent de vastes dépôts de paquets pour sauver l'utilisateur de la peine de compilation. Avec une seule commande, vous pouvez construire à partir des sources comme un pro. Ce est le confort avec Ubuntu et CentOS.

Commande Aide
--------------

Cette commande d'aide à guider l'utilisateur sur compilateur Ubuntu. Ce est moins de temps, car il peut automatiquement installé. Convient pour le programme de C.

.. code-block:: bash

		ptconfigure Ubuntucompiler help

La commande d'aide suivante aidera l'utilisateur pour l'installation.

.. code-block:: bash

	kevell@corp:/# ptconfigure UbuntuCompiler help
	******************************


         This allows you to Complie programs written in C Source

          UbuntuCompiler, ubuntu-compiler, ubuntucompiler

        - install
        Installs Ubuntu Compiling tools through apt-get.
        example: ptconfigure ubuntu-compiler install

	------------------------------
	End Help
	******************************

installation
--------------

Ce est un processus sensible à installer Ubuntu module de compilateur sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

  		ptconfigure Ubuntu-compiler install

Après avoir donné la commande, le compilateur Ubuntu sera installé avec de nouvelles mises à jour.

Si l'entrée de l'utilisateur comme N l'écran suivant viendra.

.. code-block:: bash

	Kevell@corp:/# ptconfigure UbuntuCompiler install
	Install Ubuntu Compiler? (Y/N) 
	n
	******************************


	Single App Installer:
	--------------------------------------------
	UbuntuCompiler: Failure
	------------------------------
	Installer Finished
	******************************



option
-----------

.. cssclass:: table-bordered


 +--------------------------------+----------------------------------+--------------+-------------------------------------+
 | Paramètres                     | alternative Paramètres           | option       | Commentaire                         |
 +================================+==================================+==============+=====================================+
 |Install Ubuntu compiler? Y/N    | UbuntuCompiler, ubuntu-compiler, | Yes          | Installed successfully              | 
 |                                | ubuntucompiler                   |              |                                     |
 +--------------------------------+----------------------------------+--------------+-------------------------------------+
 |Install Ubuntu compiler? Y/N    | UbuntuCompiler, ubuntu-compiler, | No           | Exit the screen                     |
 |                                | ubuntucompiler|                  |              |                                     |
 +--------------------------------+----------------------------------+--------------+-------------------------------------+

avantages
-----------

* Démarrage plus rapide
* Une meilleure sécurité
* Modification du noyau pour anticiper tout compilation
* Convient pour le programme de C

