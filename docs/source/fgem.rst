====
Gem
====

synopsis
-----------

Ce module enveloppe tous les besoins des utilisateurs pour travailler avec GEM. Il couvre diverses fonctions, et dans la main favorise diverses fonctions à exercer.

RubyGems est un gestionnaire de paquets pour le langage de programmation Ruby qui fournit un format standard pour la distribution de programmes et bibliothèques Ruby (dans un format autonome appelé un "bijou"), un outil conçu pour gérer facilement l'installation de pierres précieuses, et un serveur pour les distribuer.

Voyons les diverses caractéristiques et la façon d'utiliser ce module parmi les sujets à venir.

Commande Aide
-------------------

La commande help instruit les utilisateurs quant à la finalité et diverses caractéristiques et la syntaxe pour la mise en œuvre de ces différentes caractéristiques. Il indique également les sorties de paramètres alternatifs qui peuvent être utilisés dans les déclarations. Le format de la syntaxe pour appliquer option d'aide en vertu de ce module, est donnée ci-dessous,

.. code-block:: bash

	ptconfigure gem help

Visualiser la sortie et le travail de l'option d'aide en vertu de ce module L'écran suivant.

.. code-block:: bash


 kevell@corp:/# ptconfigure gem help
 ******************************


  This command allows you to modify create or modify gems

  Gem, gem

        - install
        Install
        example: ptconfigure gem pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure gem pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure gem pkg-ensure --package-name="somename"

 ------------------------------
 End Help
 ******************************


Différentes caractéristiques de Gem
--------------------------------------

Comme le montre de la commande d'aide ci-dessus, les diverses caractéristiques de Gem est énumérés ci-dessous,

* Remove
* Ensure

Voyons en détail sur ces fonctions.

Remove
-----------

Cette fonction vise à la suppression d'un joyau existant. Cette fonction de gemme utilisant ce module peut être atteint par la syntaxe suivante,

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"

A la place de gemname l'utilisateur peut spécifier le nom de la gemme qui doit être supprimé. Après avoir saisi la commande comme indiqué ci-dessus, le joyau spécifié sera supprimé.

.. code-block:: bash

Ensure
----------

Cette fonction assure le paquet est installé correctement dans la machine .

.. code-block:: bash

	ptconfigure gem pkg-ensure --package="ssh"

.. code-block:: bash


 kevell@corp:/# ptconfigure gem pkg-ensure --package="ssh" 

 true 
 [Pharaoh Logging] Package ssh from the Packager Gem is Installed 
 ****************************** 


 Gem Modifications: 
 -------------------------------------------- 

 Gem: Success 

 ------------------------------ 
 Gem Mods Finished 
 ****************************** 




Autres paramètres
-------------------

Les autres paramètres de ce module, chacun pouvant être utilisés dans la déclaration est,

* Gem
* gem

avantages
---------

* Les paramètres utilisés déclarant aide et d'autres caractéristiques différentes de gemme ne sont pas sensibles à la casse.
* Il est bien de choses à faire dans les deux cents os et ainsi que dans Ubuntu.
* L'utilisation de ce module, l'utilisateur peut créer et modifier ainsi que la gemme selon leurs besoins.
* L'existence d'un bijou peut être assuré dans ce module.
