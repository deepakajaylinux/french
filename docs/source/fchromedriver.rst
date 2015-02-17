================
ChromeDriver
================

synopsis
------------

Ce module permet aux utilisateurs d'installer quelques outils GC recommandé standard qui comprend curl, vim, drush et zip. Pour obtenir le chrome installé l'utilisateur a besoin de se java installé. Voyons comment utiliser cela et comment installer les thèmes à venir.

Commande Aide
--------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module du pilote Chrome. La commande help répertorie les autres paramètres du module de pilote Chrome. Il décrit également la syntaxe pour l'installation module du pilote Chrome. La commande d'aide pour le module du pilote Chrome est représentée ci-dessous.

.. code-block:: bash

		cleopatra ChromeDriver help


La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu pilote Chrome.

.. code-block:: bash

 kevell@corp:/# cleopatra ChromeDriver help

 ********************************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  ChromeDriver, chromedriver-server, chromedriver, chromedriver-srv, chromedriverserver

        - install
        Installs ChromeDriver. Note, you'll also need Java installed
        as it is a prerequisite for ChromeDriver
        example: cleopatra chromedriver install

 ------------------------------------------------
 End Help
 ************************************************

installation
---------------

Installation du pilote chrome à votre machine, qui peut être fait simplement en utilisant la commande suivante comme indiqué:

.. code-block:: bash

		cleopatra chromedriver install

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +---------------------------+------------------------------------------------------+---------------+-------------------------------------+
 | paramètres	             | Autres paramètres                                    | requis        | commentaire	                  |
 +===========================+======================================================+===============+=====================================+
 |Install ChromeDriver       | au lieu de chromedriver, nous pouvons utiliser       | Y(Yes)        | Si l'utilisateur souhaite procéder  |
 |Server? (Y/N)              | ChromeDriver, chromedriver-server, chromedriver-srv, |               | le processus d'installation qu'ils  |
 |                           | chromedriverserver aussi                             |               | peuvent entrée comme Y              |
 +---------------------------+------------------------------------------------------+---------------+-------------------------------------+
 |Install ChromeDriver       | au lieu de chromedriver, nous pouvons utiliser       | N(No)         | Si l'utilisateur souhaite quitter   |
 |Server? (Y/N)              | ChromeDriver, chromedriver-server, chromedriver-srv, |               | le processus d'installation qu'ils  |
 |                           | chromedriverserver aussi                             |               | peuvent entrée comme N.|            |
 +---------------------------+------------------------------------------------------+---------------+-------------------------------------+


Si l'utilisateur procède le processus d'installation, lors de l'exécution de l'installation, le processus demande à l'utilisateur de

.. code-block:: bash

	Enter Chrome Driver Version

La liste des versions de pilote chrome qui sont disponibles est donnée ci-dessous:

.. code-block:: bash

 0. 2.0
 1. 2.10
 2. 2.1
 3. 2.11
 4. 2.2
 5. 2.3
 6. 2.4
 7. 2.5
 8. 2.6
 9. 2.7
 10. 2.8
 11. 2.9

L'utilisateur doit spécifier les numéros de 0 à 11 en fonction de leurs exigences de la version.

Après que l'utilisateur en spécifiant la version, le processus d'installation commence et se rempli comme représenté imagée de la capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# cleopatra chromedriver install

 Install ChromeDriver Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         ChromeDriver        *
 *******************************
 Enter Chrome Driver Version
 (0) 2.0 
 (1) 2.10 
 (2) 2.1 
 (3) 2.11 
 (4) 2.2 
 (5) 2.3 
 (6) 2.4 
 (7) 2.5 
 (8) 2.6 
 (9) 2.7 
 (10) 2.8 
 (11) 2.9 
 11
 PHP Notice:  Undefined index: version in /opt/cleopatra/cleopatra/src/Modules/ChromeDriver/Model/ChromeDriverAllLinux.php on line 42
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/cleopatra-temp-script-26804823734.sh
 chmod 755 /tmp/cleopatra-temp-script-26804823734.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-26804823734.sh Permissions
 Executing /tmp/cleopatra-temp-script-26804823734.sh
 --2015-02-02 21:35:49--  http://chromedriver.storage.googleapis.com//chromedriver_linux64.zip
 Resolving chromedriver.storage.googleapis.com (chromedriver.storage.googleapis.com)... 74.125.236.44, 74.125.236.43, 74.125.236.42, ...
 Connecting to chromedriver.storage.googleapis.com (chromedriver.storage.googleapis.com)|74.125.236.44|:80... connected.
 HTTP request sent, awaiting response... 404 Not Found
 2015-02-02 21:35:52 ERROR 404: Not Found.
 
 mv: cannot stat '/tmp/chromedriver/*': No such file or directory
 unzip:  cannot find or open chromedriver_linux64.zip, chromedriver_linux64.zip.zip or chromedriver_linux64.zip.ZIP.
 Temp File /tmp/cleopatra-temp-script-26804823734.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 ChromeDriver: Success
 ------------------------------
 Installer Finished
 *********************************************

avantages
---------------

* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
* L'utilisateur peut spécifier la version qu'ils souhaitent installer lors de l'installation.
