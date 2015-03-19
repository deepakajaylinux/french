==============
Version
==============


synopsis
-------------

Cet article porte sur le terme « version » tel qu'il est utilisé dans différents contextes. Logiciel gestion des versions est le processus d'attribution des noms de version unique ou les numéros de version unique aux États uniques de logiciels. Dans une catégorie numéro version donnée (majeur, mineur), ces chiffres sont généralement assignés par ordre croissant et correspondent aux nouveaux développements dans le logiciel. À un niveau de granularité fin, un contrôle des versions est souvent utilisé pour conserver une trace de façon incrémentielle différentes versions de l'information électronique, que cette information soit logiciels ou non.


Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation du module version. L'utilisateur viendra à connaître le différent façons/format d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.


.. code-block:: bash
        
	jrush  version help

La représentation picturale de la commande help est listée ci-dessous,


.. code-block:: bash

 kevell@corp:/# jrush  version help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command Joomls Version information.

  Version, version

        - available
        Returns available Joomla Versions
        example: jrush version available

        - current
        Returns the current Joomla Version
        example: jrush version current

 ------------------------------
 End Help
 ****************************************


Available
----------------

Lorsque l'utilisateur a besoin de connaître la version de joomla disponibles, le dessous étant donné de commande exécutera le processus d'installation.


.. code-block:: bash
        
	jrush version available ..config file=”bootstrap file path”


La représentation picturale de la capture d'écran est listée ci-dessous,


.. code-block:: bash

 kevell@corp:/# jrush version available --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(1) {
  ["availableVersions"]=>
  array(2) {
    [0]=>
    string(5) "1.5.0"
    [1]=>
    string(6) "1.5.26"
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************

Current
----------------

Lorsque l'utilisateur a besoin de connaître la dernière version de joomla, le dessous étant donné de commande exécutera le processus d'installation.


.. code-block:: bash
        
	jrush version current ..config file=”bootstrap file path”

La représentation picturale de la commande ci-dessus est listée ci-dessous,


.. code-block:: bash

 kevell@corp:/# jrush version current --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(3) {
  ["shortVersion"]=>
  string(5) "3.3.3"
  ["longVersion"]=>
  string(53) "Joomla! 3.3.3 Stable [ Ember ] 25-July-2014 13:00 GMT"
  ["detailed"]=>
  object(ArrayObject)#47 (1) {
    ["storage":"ArrayObject":private]=>
    object(JVersion)#7 (11) {
      ["PRODUCT"]=>
      string(7) "Joomla!"
      ["RELEASE"]=>
      string(3) "3.3"
      ["DEV_LEVEL"]=>
      string(1) "3"
      ["DEV_STATUS"]=>
      string(6) "Stable"
      ["BUILD"]=>
      string(0) ""
      ["CODENAME"]=>
      string(5) "Ember"
      ["RELDATE"]=>
      string(12) "25-July-2014"
      ["RELTIME"]=>
      string(5) "13:00"
      ["RELTZ"]=>
      string(3) "GMT"
      ["COPYRIGHT"]=>
      string(72) "Copyright (C) 2005 - 2014 Open Source Matters, Inc. All rights reserved."
      ["URL"]=>
      string(107) "<a href="http://www.joomla.org">Joomla!</a> is Free Software released under the GNU General Public License."
    }
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************


Alternative Paramètre
----------------------------

Soit du paramètre alternatif deux peut être utilisé dans la commande-

jarticle, JArticle

eg:  jrush version current ..config file=”bootstrap file path”/ jrush Version current ..config file=”bootstrap file path”

avantages
--------------

* Aide à obtenir des informations sur une version en mode facile 
* permet à l'utilisateur pour connaître la disponibilité de la version de joomla * permet à l'utilisateur pour connaître la dernière version de  joomla
