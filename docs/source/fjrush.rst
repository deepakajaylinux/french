======
Jrush
======

synopsis
------------

Ce module aide à l'installation du jrush à votre machine. Il facilite également la mise à jour avec une nouvelle version. Voyons comment ces modules aide à l'installation d'un jrush.

Commande Aide
--------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module Jrush. Il énumère les alternatives aux paramètres du module Jrush. Il décrit également la syntaxe pour l'installation du module Jrush. La commande d'aide pour le module Jrush est représentée ci-dessous.

.. code-block:: bash

		ptconfigure JRush help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu JRush.

.. code-block:: bash

 kevell@corp:/# ptconfigure JRush help
 ******************************


  This command allows you to install or Update JRush.

  JRush, jrush, Jrush, jRush

        - install
        Installs the latest version of jRush
        example: ptconfigure jRush install

 ------------------------------
 End Help
 ******************************




installation
----------------

La commande utilisée pour installer le JRush à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash

		ptconfigure JRush install


options
---------

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +--------------------------------+----------------------------------------------+---------------+------------------------------------------+
 | paramètres                     | Alternative Paramètre                        | options       | commentaires                             |
 +================================+==============================================+===============+==========================================+
 |Install JRush - Joomla Command  | Au lieu de JRush nous pouvons utiliser:      | Y(Yes)        | Si l'utilisateur souhaite procéder le    |
 |Line ? (Y/N)                    | jrush, Jrush, jRush.                         |               | processus d'installation qu'ils peuvent  |
 |                                |                                              |               | entrée comme Y.                          |
 +--------------------------------+----------------------------------------------+---------------+------------------------------------------+
 |Install JRush - Joomla Command  | Au lieu de JRush nous pouvons utiliser:      | N(No)         | Si l'utilisateur souhaite quitter le     |
 |Line ? (Y/N)                    | jrush, Jrush, jRush.                         |               | processus d'installation qu'ils peuvent  |
 |                                |                                              |               | entrée comme N.|                         |
 +--------------------------------+----------------------------------------------+---------------+------------------------------------------+



Si l'utilisateur exécute le processus d'installation et de désinstallation du suivant se produit comme le montre sous forme de tableau .

.. cssclass:: table-bordered

 +--------------------------+--------------------------+----------------+-------------------------------------------------------------------+
 | paramètres               | chemin                   | option         | commentaires                                                      |
 +==========================+==========================+================+===================================================================+
 |Program data directory    | “/opt/jrush (module      | Yes            | Si l'utilisateur de procéder installation avec le répertoire de   |
 |(Par défaut)              | correspondant)           |                | données par défaut du programme qu'ils peuvent entrée comme Oui   |
 +--------------------------+--------------------------+----------------+-------------------------------------------------------------------+
 |Program data directory    | Spécifique de            | No(Slash de    | Si l'utilisateur souhaite procéder à leur propre répertoire de    |
 |                          | l'utilisateur            | fin)           | données de programme, ils peuvent entrée comme N, et dans la      |
 |                          |                          |                | main préciser leur propre emplacement                             |
 +--------------------------+--------------------------+----------------+-------------------------------------------------------------------+
 |Program executor          | “/usr/bin”               | Yes            | Si l'utilisateur de procéder installation avec le répertoire      |
 |directory (Par défaut)    |                          |                | programme d'exécuteur défaut qu'ils peuvent entrée comme Oui      |
 +--------------------------+--------------------------+----------------+-------------------------------------------------------------------+
 |Program executor          | Spécifique de            | No(Slash de    | Si l'utilisateur souhaite procéder à leur propre répertoire       |
 |directory                 | l'utilisateur            | fin)           | programme d'exécuteur testamentaire, ils peuvent entrée comme N,  |
 |                          |                          |                | et dans la main indiquer qu'ils possèdent emplacement.|           |
 +--------------------------+--------------------------+----------------+-------------------------------------------------------------------+


Lors de l'installation, le processus suivant se produit:

* Indique l'état de recevoir des objets.
* Indique l'état de résoudre les deltas.
* Vérifie la connectivité.
* Affiche comme dossier de données du programme peuplées.
* Supprime l'exécuteur de programme si existait déjà.

Enfin, l'installation de Jrush est terminée. La capture d'écran ci-dessous illustre le processus d'installation du JRush à votre machine:

.. code-block:: bash

 kevell@corp:/# ptconfigure JRush install
 Install JRush - Joomla Command Line ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         JRush CLI !!        *
 *******************************
 What is the program data directory? Found "/opt/jrush" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/jrush.git'  /tmp/jrush/jrushCloning into '/tmp/jrush/jrush'...
 remote: Counting objects: 3452, done.
 remote: Total 3452 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (3452/3452), 2.04 MiB | 50.00 KiB/s, done.
 Resolving deltas: 100% (2097/2097), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JRush: Success
 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure jRush uninstall
 Un Install JRush - Joomla Command Line ? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         JRush CLI !!        *
 *******************************
 What is the program data directory? Found "/opt/jrush" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)
 
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 JRush: Success
 ------------------------------
 Installer Finished
 ******************************



avantages
------------

* Ce module facilite l'utilisateur dans l'installation JRush avec la dernière version.
* L'utilisateur peut choisir leur propre chemin pour le répertoire des données du programme et le répertoire de l'exécuteur.
* Les paramètres utilisés pour déclarer l'aide et les installations ne sont pas sensibles à la casse, qui est ajouté tout avantage par rapport 
  aux autres.
* Il est bien de choses à faire dans les deux cent OS et ainsi que dans ubuntu.
* Le statut requis sont clairement surveillée lors de l'installation.
