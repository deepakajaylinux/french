=========
PHPDox
=========

synopsis
------------

Ce module facilite les utilisateurs à installer le Php Dox avec la dernière version. phpdox est un générateur de documentation pour générer documentation de l'API au format HTML, par exemple, à partir du code source de PHP. Voyons comment ce module, aide à l'installation du Php Dox.

Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module Phpdox. Il énumère les alternatives aux paramètres du module Phpdox. Il décrit également la syntaxe pour l'installation du module Phpdox. La commande d'aide pour le module Phpdox est représentée ci-dessous.

.. code-block:: bash
	
		ptconfigure Phpdox help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu Phpdox.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPDox help

 ******************************

  This command allows you to update PHPDox.

   PHPDox, phpdox

         - install
         Installs the latest version of Docker
         example: ptconfigure phpdox install

 ------------------------------
 End Help
 ******************************

installation
----------------

La commande utilisée pour installer le phpdox dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash

		ptconfigure phpdox install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +----------------------+------------------------------------------+-------------+---------------------------------------------------+
 | paramaters           | paramètre alternatif                     | Options     | commentaires                                      |
 +======================+==========================================+=============+===================================================+
 |Install PHPDox? (Y/N) | Au lieu de phpdox, nous pouvons utiliser | Y(Yes)      | Si l'utilisateur souhaite procéder le processus   |
 |                      | PHPDox également.                        |             | d'installation qu'ils peuvent entrée comme Y.     |
 +----------------------+------------------------------------------+-------------+---------------------------------------------------+
 |Install PHPDox? (Y/N) | Au lieu de phpdox, nous pouvons utiliser | N(No)       | Si l'utilisateur souhaite quitter le processus    | 
 |                      | PHPDox également.                        |             | d'installation qu'ils peuvent entrée comme N|     |
 +----------------------+------------------------------------------+-------------+---------------------------------------------------+

Si l'utilisateur procède à l'installation, le processus d'installation ressemble à la capture d'écran ci-dessous:

.. code-block:: bash

 kevell@corp:/# ptconfigure phpdox install

 Install PHPDox? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPDox!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-27804177792.sh
 chmod 755 /tmp/ptconfigure-temp-script-27804177792.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-27804177792.sh Permissions
 Executing /tmp/ptconfigure-temp-script-27804177792.sh
 --2015-01-28 15:42:36--  http://phpdox.de/releases/phpdox.phar
 Resolving phpdox.de (phpdox.de)... 188.94.27.6
 Connecting to phpdox.de (phpdox.de)|188.94.27.6|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 801185 (782K) [application/phar]
 Saving to: â€˜phpdox.pharâ€™

 100%[=======================================================================================================>] 8,01,185    11.7KB/s   in 2m 9s  

 2015-01-28 15:44:47 (6.08 KB/s) - â€˜phpdox.pharâ€™ saved [801185/801185]
 
 PHP Warning:  PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open 
 shared object file: No such file or directory in Unknown on line 0
 Sorry, but your PHP environment is currently not able to run phpDox due to
 the following issue(s):

 ext/xsl not installed/enabled

 Please adjust your PHP configuration and try again.



 Oups... phpDox encountered a problem and has terminated!

 It most likely means you've found a bug, so please file a report for this
 and paste the following details and the stacktrace (if given) along:

 PHP Version: 5.5.9-1ubuntu4.5 (Linux)
 PHPDox Version: 0.7.0
 ErrorException: E_CORE_WARNING 
 Location: Unknown (Line 0)
 
 PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open shared object 
 file: No such file or directory

 No stacktrace available
 

 phpDox 0.7.0 - Copyright (C) 2010 - 2015 by Arne Blankerts

 Temp File /tmp/ptconfigure-temp-script-27804177792.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPDox: Success
 ------------------------------
 Installer Finished
 ******************************

avantages
-----------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce module de volonté installe le phpdox dans la version mise à jour.
* Si le module existe déjà dans la machine de l'utilisateur, il affiche un message comme il est déjà existant.
