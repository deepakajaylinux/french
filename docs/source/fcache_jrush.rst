=========
Cache
=========


synopsis
-----------------

Jrush auxiliaire pour effacer le cache en mémoire temporaire. Il a deux types de cache. Mais les deux ont des différentes fonctions tel que spécifié dans leur nom. Ils sont site clair et admin clair. Il se félicite avec Ubuntu et cent OS. Suppression des fichiers, dossiers et applications--et effacer les données de la mémoire temporaire--ne sera pas faire l'affaire si vous allez à recycler le contenu n'est pas disponible dans votre ordinateur.

Commande Aide
--------------------------

La commande help gère les utilisateurs au sujet de la détermination et aussi bien que sur les options qui sont incluses dans le cache. Il énumère les autres paramètres de cache. Il décrit également la syntaxe pour le fonctionnement du module Jrush. La commande help pour cache s'affiche comme ci-dessous.


.. code-block:: bash

	jrush cache help

Après avoir tapé la commande, il répertorie les options comme action. L'image suivante il envisager observable.


.. code-block:: bash

 kevell@corp:/# jrush cache help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to clear Cache.

  Cache, cache

        - site-clear
        Deletes a user
        example: jrush cache site-clear

        - admin-clear
        Clear the administrator cache
        example: jrush cache admin-clear

 ------------------------------
 End Help
 ****************************************

 
Alternative Paramètre
--------------------------------

D'autre part l'utilisation du cache de l'utilisateur peut accorder les options suivantes.

Cache, cache.

options
-------------

Il ya deux options sont disponibles. Ils sont comme suit.


* Site-clear 
* Admin-clear

Maintenant, laissez-nous savoir sur les deux options.


Site-clear
--------------

Site-clear est costoff pour supprimer l'utilisateur. La commande suivante sert à effacer le site.


.. code-block:: bash

	jrush cache site-clear 

Après les entrées comme au-dessus de la commande, la sortie est livré comme un codage. À la cache de fin fini de compensation peut être démontré. Les captures d'écran présente le même.


.. code-block:: bash

 kevell@corp:/# jrush cache site-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["site_cache_clear"]=>
  string(19) "Site Cache Clearing"
  ["site_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************

Admin-clear
-------------------

Cela porté effacer le cache de l'administrateur. La commande des services l'utilisateur pour effacer l'admin comme suit.


.. code-block:: bash

	jrush cache admin-clear

Les captures d'écran suivantes instruire l'usager sur fonction admin-clear.


.. code-block:: bash

 kevell@corp:/# jrush cache admin-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["admin_cache_clear"]=>
  string(20) "Admin Cache Clearing"
  ["admin_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************


avantages
---------------

* It complaisant à l'effort avec Ubuntu et cent OS. 
* Respect de la casse non. 
* Il d'occasion pour supprimer l'utilisateur. 
* Il aide clair admin.


