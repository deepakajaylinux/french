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

        - uninstall 
        Uninstalls the latest version of PHPCS 
        example: ptconfigure phpcs uninstall 

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


Après ces processus comme indiqué dans le format tabulaire, les résultats sont clairement signalées le long avec le statut . La capture d'écran suivante vous explique graphiquement sur le processus impliqué dans l'installation et la désinstallation de PHPCS .


.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS install 
 Install PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-74085209498.sh 
 chmod 755 /tmp/ptconfigure-temp-script-74085209498.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-74085209498.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-74085209498.sh 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 php-pear is already the newest version. 
 0 upgraded, 0 newly installed, 0 to remove and 3 not upgraded. 
 downloading PHP_CodeSniffer-2.3.0.tgz ... 
 Starting to download PHP_CodeSniffer-2.3.0.tgz (464,453 bytes) 
 .............................................................................................done: 464,453 bytes 
 install ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-74085209498.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS uninstall 
 Uninstall PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-50071430908.sh 
 chmod 755 /tmp/ptconfigure-temp-script-50071430908.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-50071430908.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-50071430908.sh 
 uninstall ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-50071430908.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Uninstaller: 
 ------------------------------ 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  



avantages
-----------

* Ce module facilite l'utilisateur dans l'installation de PHP CS avec la version mise à jour.
* L'utilisateur peut choisir leur propre chemin pour le répertoire des données du programme et l'exécuteur
* Les paramètres utilisés pour déclarer l'aide et les installations ne sont pas sensibles à la casse, qui est ajouté tout avantage par rapport 
  aux autres.
