============
GitKeySafe
============

synopsis
------------------

Git coffre à clés qui vous aide à installe clé Git sécurité. Cela permet la permission de manière sécurisée. Ces systèmes ont la capacité des utilisateurs de visualiser l'autorisation du système de fichiers. L'autorisation de lecture accorde la capacité de lire un fichier. L'autorisation d'écriture accorde la possibilité de modifier un fichier. L'autorisation d'exécution accorde la capacité d'exécuter un fichier. Il réconforte avec Ubuntu et cent OS.

Commande Aide
----------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules Gitkeysafe. La commande help répertorie les autres paramètres de Gitkeysafe sous module de Cléopâtre. Il décrit également la syntaxe pour l'installation de la keysafe de l'utilisateur. La commande d'aide pour Gitkeysafe est illustré ci-dessous.

.. code-block:: bash

		ptconfigure GitkeySafe help

La syntaxe de la non cas de commande d'aide sensible qui ajoute un avantage pour ce module. Visualisez la capture d'écran suivante l'utilisateur sur la commande d'aide en vertu de la syntaxe de la non cas de commande d'aide sensible qui ajoute un avantage pour ce module. Visualiser l'utilisateur sur la commande d'aide en vertu gitkeysafe La capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptconfigure GitKeySafe help

 ******************************


  This module installs Git Key-Safe Server to the program git-key-safe

  GitKeySafe, git-key-safe, gitkeysafe

        - install
        Installs Git Key-Safe Server
        example: ptconfigure gitkeysafe install

        script example: git-safe-key -i /path/to/key clone http://git.com/repo.git

 ------------------------------
 End Help
 ******************************

installation
-----------------

Installation implique typiquement code étant copié / générée à partir des fichiers d'installation de nouveaux fichiers sur l'ordinateur local pour faciliter l'accès par le système d'exploitation .. Leur utilisation, l'utilisateur doit se assurer et avoir une sauvegarde, de sorte que les données de l'utilisateur peut toujours être restauré . La commande suivante permet d'installer clé de git sécurité.

.. code-block:: bash

		ptconfigure gitkeysafe install

Lors de l'installation de ce module la capture d'écran suivante sera apparu.

.. code-block:: bash

 kevell@corp:/# ptconfigure gitkeysafe install

 Install Git Key-Safe Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Git Key-Safe Server!        *
 *******************************
 Git Key-Safe script /usr/bin/git-key-safe added
 Git Key-Safe script /usr/bin/git-key-safe permissions changed to 775
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitKeySafe: Success
 ------------------------------
 Installer Finished
 ******************************

option
----------

.. cssclass:: table-bordered

 +------------------------+-----------------------------------------------+--------------+-----------------------------------------+
 | paramètres             | Autres Paramètres                             | options      | commentaires                            |
 +========================+===============================================+==============+=========================================+
 |Install gitkeysafe      | Au lieu d'utiliser gitkeysafe nous pouvons    | Y            | Il se installe sous gitkeysafe          |
 |                        | utiliser GitKeySafe,git-key-safe              |              | ptconfigure                             |
 +------------------------+-----------------------------------------------+--------------+-----------------------------------------+
 |Install gitkeysafe      | Au lieu d'utiliser gitkeysafe nous pouvons    | N            | La sortie du système d'installation     |
 |                        | utiliser GitKeySafe,git-key-safe|             |              |                                         |
 +------------------------+-----------------------------------------------+--------------+-----------------------------------------+



avantages
--------------

* Sensibilité non de cas
* Utilise pour installer la clé Git sécurité
* Voir la permission de l'utilisateur
* Travailler avec Ubuntu et cent OS
* La sécurité est possible
