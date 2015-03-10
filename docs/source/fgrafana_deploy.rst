synopsis
-------------

Grafana dispose d'un éditeur de graphite de recherche avancée qui vous permet de naviguer rapidement à l'espace métrique, ajouter des fonctions. Changer paramaters de fonction et beaucoup plus.

Grafana est une source ouverte, en vedette métriques riches tableau de bord et éditeur de graphe pour Graphite, InfluxDB & OpenTSDB.

Voyons comment ce module facilite les utilisateurs dans l'installation du grafana.

Aide Command
-------------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module Grafana. Il énumère les alternatives aux paramètres du module Grafana. Il décrit également la syntaxe pour l'installation du module Grafana. La commande d'aide pour le module Grafana est représentée ci-dessous.

.. code-block:: bash
                                               
         ptdeploy grafana help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide pour le module Grafana.

Installation
------------------

La commande utilisée pour installer les modules de grafana dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash
			
	ptdeploy grafana install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered


 +------------------------+-------------------------------------+------------+--------------------------------------------------+
 | paramètre              | Autres paramètres                   | Option     | commentaires                                     |
 +========================+=====================================+============+==================================================+
 |Install Grafana? (Y/N)  | au lieu de Grafana nous pouvons     | Y(Yes)     | Si l'utilisateur souhaite procéder le processus  | 
 |                        | utiliser, grafana                   |            | d'installation qu'ils peuvent entrée comme Y.    |
 +------------------------+-------------------------------------+------------+--------------------------------------------------+
 |Install Grafana? (Y/N)  | au lieu de Grafana nous pouvons     | N(No)      | Si l'utilisateur souhaite quitter le processus   |
 |                        | utiliser, grafana                   |            | d'installation qu'ils peuvent entrée comme N.|   |
 +------------------------+-------------------------------------+------------+--------------------------------------------------+


La capture d'écran ci-dessous représente graphiquement le processus décrit ci-dessus de l'installation.

Avantages
------------------

Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux autres.
Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.

Graphite cible Editor
----------------------------

* Graphite expression cible analyseur
* Riche en fonctionnalités compositeur requête
* Ajouter rapidement et modifier les fonctions et paramètres
* Requêtes basés sur des modèles
* Le voir en action


Graphing
----------------

* Rendu rapide, même sur de grandes plages horaires.
* Cliquez et faites glisser pour effectuer un zoom.
* Axe des Y multiple.
* Bars, lignes, points.
* Intelligente axe Y formatage
* bascule de la série et sélecteur de couleur
* valeurs de légende, et les options de formatage
* seuils de grille, étiquettes des axes
* Annotations


Dashboards
------------------

* Créer, modifier, enregistrer et recherche des tableaux de bord
* Changer travées de colonnes et la hauteur des lignes
* Glissez et déposez les panneaux pour réorganiser
* Utilisez InfluxDB ou ElasticSearch que le stockage de tableau de bord
* Import & Export tableau de bord (fichier JSON)
* Importer tableau de bord à partir de graphite
* Templating
* Tableaux de bord scriptées
* Tableau de bord des playlists
* Temps contrôles de gamme


