=============
Skipfish
=============


synopsis
------------

Module skipfish utilisé pour installer skipfish. Skipfish est un outil de reconnaissance de la sécurité des applications Web active. Il prépare un plan du site interactif pour le site visé par la réalisation d'une analyse récursive et sondes basées sur les dictionnaires. La carte résultante est ensuite annotée avec la sortie d'un certain nombre de contrôles de sécurité actifs. Le rapport final généré par l'outil est destiné à servir de base à des évaluations professionnelles de sécurité des applications Web. Ce module renforcer avec Ubuntu et cent OS.

Commande Aide
----------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module skipfish. Il énumère les alternatives aux paramètres du module skipfish. Il décrit également la syntaxe pour l'installation du module skipfish. La commande d'aide pour le module skipfish est représentée ci-dessous.

.. code-block:: bash	

		ptconfigure Skipfish help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu skipfish.

.. code-block:: bash

 kevell@corp:/# ptconfigure Skipfish help

 ******************************


  This command allows you to install Skipfish.
  Skipfish, skipfish

        - install
        Installs Skipfish. 
        example: ptconfigure skipfish install

 ------------------------------
 End Help
 ******************************



 
installation
-----------------

Cette commande autorise à installer skipfish carte de site interactif. Lorsque l'utilisateur veut installer skipfish la commande suivante guide l'utilisateur à installer.

.. code-block:: bash

                ptconfigure skipfish install

après avoir tapé cette commande, le système demande à l'utilisateur le souhaite. L'autre processus explique l'installation grâce à la capture d'écran.

.. code-block:: bash


 kevell@corp:/# ptconfigure Skipfish install
 Install  Skipfish? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          Skipfish !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  skipfish
 0 upgraded, 1 newly installed, 0 to remove and 15 not upgraded.
 Need to get 233 kB of archives.
 After this operation, 574 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ trusty/universe skipfish amd64 2.10b-1 [233 kB]
 Fetched 233 kB in 29s (7,910 B/s)
 Selecting previously unselected package skipfish.
 (Reading database ... 199429 files and directories currently installed.)
 Preparing to unpack .../skipfish_2.10b-1_amd64.deb ...
 Unpacking skipfish (2.10b-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up skipfish (2.10b-1) ...
 [Pharaoh Logging] Adding Package skipfish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Skipfish: Success
 ------------------------------
 Installer Finished

 ******************************



Option
-----------

.. cssclass:: table-bordered

 
 +------------------------+-----------------------------------------+-------------+----------------------------------------------------+
 | paramètre              | Autres paramètres                       | Option      | commentaires                                       |
 +========================+=========================================+=============+====================================================+
 |Install Skipfish? (Y/N) | au lieu de skipfish nous pouvons        | Y(Yes)      | Si l'utilisateur veut le processus d'installation, |
 |                        | utiliser, skipfish                      |             | vous pouvez aller en entrée Y.                     |
 +------------------------+-----------------------------------------+-------------+----------------------------------------------------+
 |Install Skipfish? (Y/N) | au lieu de skipfish nous pouvons        | N(No)       | Si les utilisateurs veulent, ils peuvent           |
 |                        | utiliser, skipfish                      |             | terminer l'entrée de processus d'installation N.|  |
 +------------------------+-----------------------------------------+-------------+----------------------------------------------------+

avantages
--------------

* Skipfish est hautement adaptative et fiable.
* Eh bien conçu des contrôles de sécurité.
* Manutention Graceful des sites multi-cadres
* Installation de version mise à jour automatique
* Haut débit accessible.
* Sensibilité non de cas.
* Ainsi à faire dans Ubuntu et Cent OS.
