=============
Extension
=============

synopsis
--------------

Extension doivent être identifiés pour le système d'exploitation peut y remédier. Ces noms de fichiers ont une réglementation spécifique. La première partie du nom à gauche de la période est appelée le nom de racine. Le nom de racine ne peut pas être identique à un nom de périphérique. La deuxième partie à droite de la période est l'extension. Elle est facultative et est souvent, mais pas nécessairement, trois caractères de long. Extension peut être ajoutée par le biais de codage. Elle a renforcé pour escroquer avec Ubuntu et cent OS.


Commande Aide
-----------------

La commande help guide les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans l'extension. Il énumère les paramètres alternatifs de l'extension. Il décrit également la syntaxe pour le fonctionnement du module Jrush. La commande help pour extension s'affiche comme ci-dessous.


.. code-block:: bash

	jrush extension help

Après avoir tapé la commande, il répertorie les options comme action. L'image suivante le visualiser évidemment.



.. code-block:: bash

 kevell@corp:/# jrush Extension help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla Extensions (Component, Module or Plugin).

  Extension, extension

        - disable
        Deletes a extension
        example: jrush extension disable

        - enable
        Enables a extension
        example: jrush extension enable

        - info
        Display the details of a extension
        example: jrush extension info


 ------------------------------
 End Help
 ****************************************


Alternative Paramètre
----------------------------

Comme une question de choix à l'aide d'extension, l'utilisateur peut faire utiliser des options suivantes.

Extension, extension

options
------------

Il y a trois options sont disponibles. Nous verrons sur l'option de prolongation.


* Enable
* Disable
* Info

Disable
-----------

Lorsque l'utilisateur d'entrée que lui permettre automatiquement supprime l'extension. La commande suivante permet d'activer.


.. code-block:: bash

	jrush extension Disable

Le coup du manteau suivant permet de visualiser sa fonction.


.. code-block:: bash

 kevell@corp:/# jrush Extension disable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************


Enable
-----------

Enable utilise pour activer l'extension. La commande suivante aider l'utilisateur à activer.


.. code-block:: bash

 	jrush extension enable

Les captures d'écran suivantes guide l'utilisateur pour activer sa fonction.



.. code-block:: bash

 kevell@corp:/# jrush Extension enable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:
 
 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 1
 ------------------------------
 Extension Manage Finished
 ****************************************



Info
--------

Info est une aide pour aider l'utilisateur à afficher les détails de l'expansion. Il demande pour l'id de l'extension. Après entre la valeur il affiche les détails de l'extension. La commande suivante permet d'afficher les informations.


.. code-block:: bash

	jrush extension info

On visualise par la capture d'écran.



.. code-block:: bash

 kevell@corp:/# jrush Extension info --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************

avantages
----------------

* Extensions peuvent être considéré comme un type de métadonnées. 
* Plusieurs applications d'être associé à une extension donnée. 
* La casse non * confortable avec Ubuntu et cent OS. 
* Utilise pour supprimer l'extension 
* Info utilise pour afficher des informations sur l'extension.


