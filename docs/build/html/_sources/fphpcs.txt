==========
PHPCS
==========

synopsis
----------

Ce module aide à l'installation de PHP cs de GC Repo. Lors de l'installation, ce module récupère la dernière version. L'utilisateur peut spécifier l'emplacement pour le répertoire des données du programme et le répertoire de l'exécuteur. Enfin les résultats sont clairement signalés.

Commande Aide
-------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module PHP cs. Il décrit également la syntaxe pour installer php cs. La commande d'aide pour php cs est donnée ci-dessous.

.. code-block:: bash

	ptconfigure PHPCS help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu PHPCS.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCS help
 ******************************


 This command allows you to install PHPCS from a GC Repo.

 PHPCS
 - install
 Installs the latest version of PHPCS
 example: ptconfigure phpcs install

 ------------------------------
 End Help
 ******************************

installation
-------------

Installation du PHP CS est plus simple en utilisant la commande suivante comme indiqué:

.. code-block:: bash
	
	ptconfigure PHPCS install

Après avoir saisi la commande ci-dessus les opérations suivantes comme indiqué dans le format tabulaire se produit.

.. cssclass:: table-bordered

 +------------------------------------+-------------+----------------------------------------------------------------------+
 | paramaters                         | Options     | commentaires                                                         |
 +====================================+=============+======================================================================+
 |Install PHP Code Sniffer ? (Y/N)    | Y(Yes)      | Si l'utilisateur souhaite procéder le processus d'installation       |
 |                                    |             | qu'ils peuvent entrée comme Y.                                       |
 +------------------------------------+-------------+----------------------------------------------------------------------+
 |Install PHP Code Sniffer ? (Y/N)    | N(No)       | Si l'utilisateur souhaite quitter le processus d'installation qu'ils |
 |                                    |             | peuvent entrée comme N.|                                             |
 +------------------------------------+-------------+----------------------------------------------------------------------+




Si l'utilisateur procède le processus d'installation les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered


 +----------------------+-------------------------+------------------+------------------------------------------------------------------+
 | paramaters           | Chemin                  | Option           | Commentaire                                                      |
 +======================+=========================+==================+==================================================================+
 |Program data          | opt/phpcs (module       | Yes              | Si l'utilisateur de procéder Installation avec le répertoire de  |
 |directory(Par défaut) | correspondant)          |                  | données par défaut du programme qu'ils peuvent entrée comme Oui  |
 +----------------------+-------------------------+------------------+------------------------------------------------------------------+
 |Program data          | Spécifique de           | No(Slash de fin) | Si l'utilisateur souhaite procéder à leur propre répertoire de   |
 |directory             | l'utilisateur           |                  | données de programme, ils peuvent entrée comme N, et dans la     |
 |                      |                         |                  | main indiquer qu'ils possèdent emplacement.                      |
 +----------------------+-------------------------+------------------+------------------------------------------------------------------+
 |Program executor      | “/usr/bin”              | Yes              | Si l'utilisateur de procéder installation avec le répertoire     |
 |directory             |                         |                  | programme d'exécuteur défaut qu'ils peuvent entrée comme Oui     |
 |(Par défaut)          |                         |                  |                                                                  |
 +----------------------+-------------------------+------------------+------------------------------------------------------------------+
 |Program executor      | Spécifique de           | No(Slash de fin) | Si l'utilisateur souhaite procéder à leur propre répertoire      |
 |directory             | l'utilisateur           |                  | programme d'exécuteur testamentaire, ils peuvent entrée comme N, |
 |                      |                         |                  | et dans la main indiquer qu'ils possèdent emplacement.|          |
 +----------------------+-------------------------+------------------+------------------------------------------------------------------+


Après ces processus comme indiqué dans le format tabulaire, les résultats sont clairement signalées le long avec le statut. La capture d'écran suivante vous explique graphiquement sur le processus impliqué dans l'installation de PHPCS.

.. code-block:: bash

 Kevell@corp:/# ptconfigure PHPCS install
 Install PHP Code Sniffer ? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP CSniffer        *
 *******************************
 What is the program data directory? Found "/opt/phpcs" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/ptconfigure-phpcs.git'  /tmp/phpcs/phpcsCloning into '/tmp/phpcs/phpcs'...
 remote: Counting objects: 862, done.
 remote: Total 862 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (862/862), 491.23 KiB | 64.00 KiB/s, done.
 Resolving deltas: 100% (378/378), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCS: Success
 ------------------------------
 Installer Finished
 ****************************



avantages
-----------

* Ce module facilite l'utilisateur dans l'installation de PHP CS avec la version mise à jour.
* L'utilisateur peut choisir leur propre chemin pour le répertoire des données du programme et l'exécuteur
* Les paramètres utilisés pour déclarer l'aide et les installations ne sont pas sensibles à la casse, qui est ajouté tout avantage par rapport 
  aux autres.
