===================
PharaohTools
===================

synopsis
------------

Les passes de modules de l'outil Pharaon dans l'installation Ptdeploy, Pttest, Jrush, la génération de rapports de ptconfigure. Il facilite les utilisateurs pour assurer la disponibilité avant installations. Seulement modules manquants peuvent être installés spécifiquement.

Commande Aide
---------------

La commande help guide les utilisateurs sur la façon de faire usage de ce module particulier sous ptconfigure.

Il fait également prendre conscience des options qui peuvent être effectuées sur ce module spécifique.

La capture d'écran comme ci-dessous vous donne une représentation graphique concernant l'utilisation de la commande d'aide.

.. code-block:: bash

 kevell@corp:/# ptconfigure PharaohTools help
 ******************************


  This command allows you to install the Pharaoh Tools which are ready. These include
  ptconfigure - this Configuration Management tool, Ptdeploy - the Automated Deployment tool,
  and Pttest, the test configuration and automation tool.

  PharaohTools, pharaohtools, pharaoh-tools

        - install
        Installs the latest version of all of the Pharaoh Tools
        example: ptconfigure pharaoh-tools install

 ------------------------------
 End Help
 ******************************

installation
-------------

Le module d'outil de pharaon agit comme une route plus courte qui enveloppe installation de Ptdeploy, Pttest, Jrush. Si l'un module particulier est manquant parmi les trois, le seul module spécifique sera installé qui est un avantage supplémentaire. Le processus d'assurer joue un rôle important dans l'accaparement de données concernant la disponibilité des modules.

La commande utilisée pour le processus d'installation sous Pharaon outil est donnée ci-dessous,

.. code-block:: bash

		ptconfigure pharaoh-tools install


.. cssclass:: table-bordered

 +-----------------------+----------------------------+-------------------+------------------------------------------------------------+
 | paramètres            | Alternative paramètre      | Disponible entrée | commentaires                                               |
 +=======================+============================+===================+============================================================+
 |Install Pharaoh Tools? | PharaohTools,              | Y(Yes)            | Si l'utilisateur souhaite continuer avec le processus      |        
 |(Y/N)                  | pharaohtools,              |                   | d'installation, ils peuvent entrée comme Y                 |
 |                       | pharaoh-tools              |                   |                                                            |
 +-----------------------+----------------------------+-------------------+------------------------------------------------------------+
 |Install Pharaoh Tools? | PharaohTools,              | N(No)             | Si l'utilisateur souhaite quitter le processus             | 
 |(Y/N)                  | pharaohtools,              |                   | d'installation, ils peuvent cesser de fumer en             |
 |                       | pharaoh-tools              |                   | utilisant simplement N|                                    |
 +-----------------------+----------------------------+-------------------+------------------------------------------------------------+


Lors de l'installation de l'outil Pharaon les étapes suivantes ont lieu:


Assurer
---------

* L'outil pharaon assure les modules disponibles.
* Tout en assurant, Il ne vérifie pas sur les versions.

Ptdeploy
-------------

* Le module ptdeploy se rapporte tel qu'il est installé, en cas d'existence.
* Il vérifie également la version du module de ptdeploy.
* Si le module de ptdeploy est pas disponible dans la machine, puis automatiquement ptdeploy progressera à installer.


Pttest
---------------

* Après l'achèvement de l'installation ptdeploy, il assurera le module Pttest.
* Le module Pttest se rapporte tel qu'il est installé, en cas d'existence.
* Si le module Pttest ne est pas disponible dans la machine, ensuite automatiquement Pttest progressera à installer.


Jrush
---------

* Après l'achèvement de l'installation Pttest, il assurera le module Jrush.
* Le module Jrush se rapporte tel qu'il est installé, en cas d'existence.
* Si le module Jrush ne est pas disponible dans la machine, ensuite automatiquement Jrush progressera à installer.


Si tous les trois modules existent déjà, alors il affichera un message d'exception comme indiqué dans la capture d'écran ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install
 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************



options supplémentaires
-------------------------

Lors de l'installation Ptdeploy, Pttest, Jrush les options suivantes sont requises comme entrée de l'utilisateur. Voyons à propos, les options supplémentaires qui peuvent être spécifiées par les utilisateurs se ils le souhaitent, est représenté sous forme de tableau, comme indiqué ci-dessous.


.. cssclass:: table-bordered

 +------------------------+-------------------------+----------+-----------------------------------------------------------------------+
 | paramètre              | chemin                  | option   | commentaire                                                           |
 +========================+=========================+==========+=======================================================================+
 |Program data directory  | “/opt/pttest “(module   | Yes      | Si l'utilisateur de procéder installation avec le répertoire de       |
 |(Default)               | correspondant)          |          | données par défaut du programme qu'ils peuvent entrée comme Oui       |
 +------------------------+-------------------------+----------+-----------------------------------------------------------------------+
 |Program data directory  | Spécifique de           | No(Slash | Si l'utilisateur souhaite procéder à leur propre répertoire de        |
 |                        | l'utilisateur           | de fin)  | données de programme, ils peuvent entrée comme N, et dans la main     |
 |                        |                         |          | indiquer qu'ils possèdent emplacement.                                |
 +------------------------+-------------------------+----------+-----------------------------------------------------------------------+
 |Program executor        | “/usr/bin”              | Yes      | Si l'utilisateur de procéder installation avec le répertoire          |
 |directory (Default)     |                         |          | programme d'exécuteur défaut qu'ils peuvent entrée comme Oui          |
 +------------------------+-------------------------+----------+-----------------------------------------------------------------------+
 |Program executor        | Spécifique de           | No(Slash | Si l'utilisateur souhaite procéder à leur propre répertoire           |
 |directory               | l'utilisateur           | de fin)  | programme d'exécuteur testamentaire, ils peuvent entrée comme N,      |
 |                        |                         |          | et dans la main indiquer qu'ils possèdent emplacement.|               |
 +------------------------+-------------------------+----------+-----------------------------------------------------------------------+


Lors de l'installation, il précisera l'emplacement de git clone, affiche le nombre d'objets, recevant des objets, résoudre des deltas, la connectivité.

La capture d'écran suivante vous explique graphiquement sur le processus impliqué dans l'installation de l'outil Pharaon.

.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install
 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************

avantages
------------

* Il facilite les utilisateurs de se assurer avant l'installation.
* En cas de module particulier est manquant, l'utilisateur peut procéder à l'installation de ce module particulier seul.
* L'utilisateur peut spécifier leur propre chemin ou l'emplacement pour le répertoire des données du programme et le répertoire de l'exécuteur.
* Si un module particulier existe déjà dans la machine, puis l'outil d'installation jeter un message d'exception comme ce est déjà
  installé.
* Il évite l'écrasement indésirable de modules, il est donc gain de temps.
