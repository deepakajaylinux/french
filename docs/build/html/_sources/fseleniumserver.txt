=================
Selenium Server
=================


synopsis
-----------

Le sélénium est un framework de test de logiciel portable pour les applications web. Le sélénium est un outil d'enregistrement / lecture pour la création des tests sans avoir à apprendre un langage de script de test (Selenium IDE). Il fournit également un langage spécifique à un domaine test (Selenese) [1] pour écrire des tests dans un certain nombre de langages de programmation populaires, y compris Java, C #, Groovy, Perl, PHP, Python et Ruby. Les tests peuvent ensuite être exécutées sur la plupart des navigateurs web modernes. Sélénium déploie sur Windows, Linux et les plates-formes Macintosh

Voyons comment ce module facilite les utilisateurs dans l'installation du serveur de sélénium.

Commande Aide
--------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de serveur de sélénium. Il énumère les alternatives aux paramètres du module de serveur de sélénium. Il décrit également la syntaxe pour l'installer. La commande d'aide pour le module de serveur de sélénium est représenté comme ci-dessous.

.. code-block:: bash

	ptconfigure seleniumserver help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de module de serveur de sélénium.

.. code-block:: bash

 kevell@corp:/# ptconfigure SeleniumServer help
 ******************************


  This command allows you to install Selenium Server.

  SeleniumServer, selenium-server, selenium, selenium-srv, seleniumserver

        - install
        Installs Selenium Server. Note, you'll also need Java installed
        as it is a prerequisite for Selenium
        example: ptconfigure selenium install
        example: ptconfigure selenium install --with-chrome-driver # will set the executor command to use default chrome driver


 ------------------------------
 End Help
 ******************************

installation
----------------

La commande utilisée pour l'installation du serveur de sélénium est simple que d'entrer la commande qui est indiqué ci-dessous.

.. code-block:: bash

		ptconfigure seleniumserver install


Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/# ptconfigure selenium install 

 Install Selenium Server? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Selenium Srv        * 
 ******************************* 
 Enter Selenium Version 
 (0) 2.39 
 (1) 2.40 
 (2) 2.41 
 (3) 2.42 
 (4) 2.43 
 (5) 2.44 
 0 

 [Pharaoh Logging] Ensure module install is not checking versions 
 [Pharaoh Logging] Command 'git' found 
 [Pharaoh Logging] Command 'gitk' found 
 [Pharaoh Logging] Command 'git-cola' found 
 [Pharaoh Logging] Not installing as already installed 
 [Pharaoh Logging] Ensure module install is not checking versions 
 [Pharaoh Logging] Module Java reports itself as Installed 
 [Pharaoh Logging] Not installing as already installed 
 Creating /tmp/ptconfigure-temp-script-5204575277.sh 
 chmod 755 /tmp/ptconfigure-temp-script-5204575277.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-5204575277.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-5204575277.sh 
 --2015-03-26 15:54:02--  http://selenium-release.storage.googleapis.com/2.39/selenium-server-standalone-2.39.0.jar 
 Resolving selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)... 216.58.220.33, 2404:6800:4007:805::2001 
 Connecting to selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)|216.58.220.33|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 34603971 (33M) [application/x-java-archive] 
 Saving to: ‘selenium-server-standalone-2.39.0.jar’ 

 100%[========================================================================================================>] 3,46,03,971 48.6KB/s   in 19m
 15s 

 2015-03-26 16:13:18 (29.3 KB/s) - ‘selenium-server-standalone-2.39.0.jar’ saved [34603971/34603971] 

 Temp File /tmp/ptconfigure-temp-script-5204575277.sh Removed 
 Program Executor Deleted if existed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 SeleniumServer: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 




option
------------


Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +----------------------+--------------------------------------------------+-------------+-------------------------------------------+
 | paramètres           | Autres paramètres                                | Option      | commentaires                              |
 +======================+==================================================+=============+===========================================+
 |Install Selenium      | nous pouvons utiliser au lieu de seleniumserver, | Y(Yes)      | Si l'utilisateur veut le processus        |
 |Server? (Y/N)         | SeleniumServer, Selenium, selenium-srv ,         |             | d'installation, vous pouvez aller en      |
 |                      | selenium-server aussi.                           |             | entrée Y.                                 |
 +----------------------+--------------------------------------------------+-------------+-------------------------------------------+
 |Install Selenium      | nous pouvons utiliser au lieu de seleniumserver, | N(No)       | Si les utilisateurs veulent, ils peuvent  |
 |Server? (Y/N)         | SeleniumServer, Selenium, selenium-srv ,         |             | terminer l'entrée de processus            |
 |                      | selenium-server aussi.                           |             | d'installation N.|                        |
 +----------------------+--------------------------------------------------+-------------+-------------------------------------------+



avantages
-----------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Vous pouvez développer des tests automatisés dans le langage de programmation de votre choix tels que c #, Java, Python, PHP, Perl et Ruby 
  ainsi que la course ces tests sur différentes combinaisons de navigateurs tels que Chrome, Firefox ou IE
