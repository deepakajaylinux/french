==========
Memcached
==========

Synopsis
---------------

L'aspect majeur de ce module est d'installer et de mettre à jour le memcache avec la dernière version.

Memcached est un système de mise en antémémoire distribué mémoire d'usage général. Il est souvent utilisé pour accélérer des sites Web dynamiques de bases de données dynamiques en mettant en cache les données et les objets dans la mémoire RAM de réduire le nombre de fois qu'une source de données externe (comme une base de données ou API) doit être lu.

Memcached est un logiciel libre et open-source, sous réserve des termes de la licence BSD révisée. [2] Memcached fonctionne sur Unix (au moins Linux et OS X) et les systèmes d'exploitation Microsoft Windows. Il ya une dépendance stricte sur libevent.

Voyons sur le processus d'installation et de l'utilisation de ce module dans les prochains sujets.



Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module Memcached. Il énumère les alternatives aux paramètres du module Memcached. Il décrit également la syntaxe pour l'installation du module Memcached. La commande d'aide pour le module Memcached est représentée ci-dessous.

.. code-block:: bash

		ptconfigure Memcached help


La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu Memcached.

.. code-block:: bash

 kevell@corp:/# ptconfigure Memcached help

 ******************************


  This command allows you to update Memcached.

  Memcached, memcached

        - install
        Installs the latest version of memcache
        example: ptconfigure memcached install

 ------------------------------
 End Help
 ******************************


installation
----------------

La commande utilisée pour installer le Memcached dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash

	ptconfigure memcached install


Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +-----------------------+-----------------------------------------+-------------+-------------------------------------------+
 | paramètres            | Alternative Paramètre                   | options     | commentaires                              |
 +=======================+=========================================+=============+===========================================+
 |Install Memcached?     | Au lieu de memcached, nous pouvons      | Y(Yes)      | Si l'utilisateur souhaite procéder le     |
 |(Y/N)                  | utiliser Memcached également.           |             | processus d'installation qu'ils peuvent   |
 |                       |                                         |             | entrée comme Y.                           |
 +-----------------------+-----------------------------------------+-------------+-------------------------------------------+
 |Install Memcached?     | Au lieu de memcached, nous pouvons      | N(No)       | Si l'utilisateur souhaite quitter le      |
 |(Y/N)                  | utiliser Memcached également.           |             | processus d'installation qu'ils peuvent   |
 |                       |                                         |             | entrée comme N.|                          |
 +-----------------------+-----------------------------------------+-------------+-------------------------------------------+


La capture d'écran ci-dessous peut vous donner une représentation picturale sur le processus d'installation.

.. code-block:: bash


Fonctions de memcached
-------------------------------

Tout en utilisant le memcached, le processus peut lire et mettre en œuvre les fonctions suivantes qui sont inclus dans memcached,

* Memcache :: add - Ajoute un élément au serveur
* Memcache :: addServer - Ajout d'un serveur memcache à pool de connexion
* Memcache :: close - connexion au serveur Fermer memcached
* Memcache :: connect - connexion à un serveur de memcached
* Memcache :: decrement - Diminuer la valeur de l'article
* Memcache :: delete - Efface un élément du serveur
* Memcache :: flush - Vide tous les éléments existants sur le serveur
* Memcache :: get - Récupère un élément du serveur
* Memcache :: getExtendedStats - Récupère des statistiques de tous les serveurs dans la piscine
* Memcache :: getServerStatus - l'état du serveur de retour
* Memcache :: getStats - les statistiques du serveur
* Memcache :: getVersion - Retour version du serveur
* Memcache :: increment - Incrément la valeur de l'article
* Memcache :: pconnect - serveur de cache Ouvre une connexion persistante
* Memcache :: replace - Remplace la valeur d'un élément existant
* Memcache :: set - Stocke des données dans le serveur
* Memcache :: setCompressThreshold - Activer la compression automatique de grandes valeurs
* Memcache :: setServerParams - Changements __gVirt_NP_NNS_NNPS<__ paramètres du serveur et le statut à l'exécution


Avantages
------------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce module de volonté installe le memcached dans la version mise à jour.
* Si le module existe déjà dans la machine de l'utilisateur, il affiche un message comme il est déjà existant.
