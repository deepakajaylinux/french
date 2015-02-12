=======
Aptana
=======

synopsis
--------------

Aptana est un environnement de développement intégré open source (IDE) pour construire des applications web. Cette commande utilisé pour permettre à l'utilisateur d'installer aptana. Ce est un développement web open source .Basée sur Eclipse, il prend en charge JavaScript, HTML, CSS et DOM avec complétion de code, décrivant, JavaScript débogage, erreur et notifications d'avertissement et la documentation intégrée. Plugins supplémentaires permettent de soutenir Aptana PHP, Python, Perl. Aptana est disponible en autonome sur Windows, Mac OS X et Linux, ou comme un plugin pour Eclipse.

Aide command
--------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module Aptana. Il décrit également la syntaxe pour l'installation Aptana. La commande d'aide pour le module Aptana est représentée ci-dessous.

.. code-block:: bash

		cleopatra Aptana help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu Aptana.

.. code-block:: bash


 kevells@corp:/# cleopatra Aptana help

 ******************************


 This command allows you to install Aptana, The open-source web development IDE.

 Aptana, aptana

       - install
       Installs Aptana.
       example: cleopatra aptana install

       - uninstall
       Uninstalls Aptana.
       example: cleopatra aptana uninstall

 ------------------------------
 End Help
 ******************************


Installation
--------------

La commande utilisée pour installer le Aptana à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash
		
		cleopatra Aptana install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format d'écran ..


.. cssclass:: table-bordered

 +----------------------------+-------------+------------------------------------------+---------------------------------------------+
 | Paramètre 		      | Option      | alternatifs 			       | Commentaires				     |
 +============================+=============+==========================================+=============================================+
 |Install Aptana?(Y/N)        | Yes         | Au lieu d'utiliser Aptana l'utilisateur  | Il va installer le module Aptana sous       |
 |			      |             | peut utiliser aptana		       | Cleopatra				     | 
 +----------------------------+-------------+------------------------------------------+---------------------------------------------+
 |Install Aptana?(Y/N)        | No          | Au lieu d'utiliser Aptana l'utilisateur  | L'utilisateur doit quitter l'installation.  |
 |                            |             | peut utiliser aptana|                    |                                             | 
 +----------------------------+-------------+------------------------------------------+---------------------------------------------+
 


Désinstallation
-------------------

La commande utilisée pour la désinstallation du Aptana à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash

		cleopatra Aptana uninstall

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format d'écran.


.. cssclass:: table-bordered

 +----------------------------+-------------+------------------------------------------+---------------------------------------------+
 | Paramètre                  | Option      | alternatifs                              | Commentaires                                |
 +============================+=============+==========================================+=============================================+
 |UnInstall Aptana?(Y/N)      | Yes         | Au lieu d'utiliser Aptana l'utilisateur  | Il permet de désinstaller le module dans    |
 |                            |             | peut utiliser aptana                     | Aptana Cleopatra                            | 
 +----------------------------+-------------+------------------------------------------+---------------------------------------------+
 |UnInstall Aptana?(Y/N)      | No          | Au lieu d'utiliser Aptana l'utilisateur  | L'utilisateur doit quitter la               |
 |                            |             | peut utiliser aptana                     | désinstallation..|                          | 
 +----------------------------+-------------+------------------------------------------+---------------------------------------------+



Plate-forme & Langue support
----------------------------------------

Aptana Studio 3 fournit le support suivant pour le développement d'applications PHP:

* Coloration de la syntaxe en fonction du thème choisi dans les préférences;
* Assistant de code;
* Annotations d'erreur de syntaxe;
* Auto indentation et le Code de formatage;
* Hyper-liens vers des classes, des fonctions et des variables en survolant éléments et en appuyant sur la touche Ctrl;
* Popups PHPDoc Lorsque vous survolez les éléments qui ont attachés documentation;
* Lire et écrire Événements marqueurs en cliquant sur les éléments spécifiques de PHP.

Aptana version 1.5 fourni un appui pour développer des applications PHP via le plugin add-on PHP. Cela comprenait:

* Built-in serveur PHP pour la prévisualisation dans les Aptana,
* Code complet aider, le code décrivant et le formatage du code,
* Débogueur PHP intégré,
* Construit en Smarty,
* Tapez vue hiérarchique,
* Aller à la déclaration,
* Manuel PHP intégré

Avantages
--------------

* Il est utilisé pour installer et non installer aptana
* Sensibilité non de cas
* Il soutient Ubuntu et Cent OS
* PHP intégré débogueur
* Code complet aider, le code décrivant et le formatage du code

