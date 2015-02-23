=======
GIMP
=======


Synopsis
-----------

Ce module permet aux utilisateurs d'installer GIMP qui est un éditeur d'image populaire.

GIMP un acronyme pour Programme GNU Image Manipulation) est utilisé pour la retouche d'image et l'édition, de forme libre dessin, redimensionnement, recadrage, photo-montages, la conversion entre les différents formats d'image, et les tâches plus spécialisées.

GIMP est distribué gratuitement (et par) ne importe qui, et ne importe qui peut regarder son contenu et son code source et peut ajouter des fonctionnalités ou corriger les problèmes. Il est distribué sous licence GPLv3 LGPLv3 et +. GIMP a commencé en 1995 comme le projet d'école de deux étudiants universitaires; maintenant GIMP est une application à part entière, disponible sur toutes les distributions de GNU / Linux et les versions récentes de Microsoft Windows et Mac OS X.

Voyons comment ce module facilite l'installation de GIMP parmi les sujets à venir.


Commande Aide
-------------------

La commande d'aide est un manuel d'utilisation brève qui représente les utilisateurs concernant l'objectif de ce module, ses listes aboutissants ses paramètres alternatifs qui peuvent être utilisés dans les déclarations, avec la syntaxe pour l'installation de GIMP grâce à apt-get. La syntaxe d'utilisation de l'aide option dans ce module est illustré ci-dessous,

.. code-block:: bash

	ptconfigure GIMP help


La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de GIMP.


installation
--------------

La commande utilisée pour l'installation de GIMP grâce à apt-get en utilisant ce module est simple en utilisant simplement la commande ci-dessous,
.. code-block:: bash

	ptconfigure GIMP install

Après avoir saisi la commande ci-dessus, les étapes suivantes sont effectuées comme décrit dans le tableau,

.. cssclass:: table-bordered


 +-----------------------+---------------------------------+------------+------------------------------------------------------+
 | Paramètres            | Alternative paramètres          | Option     | Commentaires                                         |
 +=======================+=================================+============+======================================================+
 |GIMP Install? (Y/N)    | Au lieu de GIMP nous pouvons    | Y(Yes)     | Si l'utilisateur souhaite continuer l'installation,  |
 |                       | utiliser gimp également.        |            | ils peuvent entrée comme Y.                          |
 +-----------------------+---------------------------------+------------+------------------------------------------------------+
 |GIMP Install? (Y/N)    | Au lieu de GIMP nous pouvons    | N(No)      | Si l'utilisateur souhait de quitter l'installation,  |
 |                       | utiliser gimp également.        |            | ils peuvent entrée comme N.|                         |
 +-----------------------+---------------------------------+------------+------------------------------------------------------+


La capture d'écran ci-dessous illustre visuellement sur le processus d'installation.



avantages
----------

* Les paramètres utilisés déclarant aide et d'autres caractéristiques différentes de apt ne sont pas sensibles à la casse.
* Il est bien de choses à faire dans les deux cents os et ainsi que dans Ubuntu.


GIMP fournit également des outils «intelligents» qui utilisent un algorithme plus complexe de faire des choses qui seraient autrement de temps, voire impossible. Il se agit notamment d'un:

* Outil Clone, qui copie pixels en utilisant une brosse
* Healing Brush, qui copie les pixels d'une zone et corrige ton et la couleur
* Outil Perspective de clone, qui fonctionne comme l'outil clone, mais corrige des changements de distance
* Blur et aiguiser les flous d'outils et aiguise aide d'un pinceau
* Dodge et un outil de gravure est une brosse qui rend cibles pixels plus clairs (esquives) ou plus sombre (brûlures)


GIMP transformer outils comprennent:

* Aligner
* Déplacer
* cultures
* Rotation
* échelle
* Shear
* perspective
* flip
