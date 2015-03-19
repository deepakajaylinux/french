==========
JFeature
==========

synopsis
---------------

JFeatures est l'un des paquets de logiciels plus populaires au monde, utilisés pour construire, organiser, gérer et publier du contenu pour sites Web, blogs, réseaux intranet. Quand l'utilisateur pousse le fichier zip un autre fichier toutes les fonctionnalités s'ajouteront. En raison de son architecture évolutive, c'est aussi une base idéale pour créer des applications web. Il a utilisé pour gérer le volet de la migration de la scène. Il pratique avec Ubuntu et CentOS.

Commande Aide
----------------------

La commande help guide les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans le module JFeatures. Il énumère les paramètres alternatifs du module JFeatures. Il décrit également la syntaxe pour l'installation du module JFeatures. La commande help pour JFeatures module s'affiche comme ci-dessous.


.. code-block:: bash

	jrush JFeatures help

La syntaxe servant à déclarer la commande help est le non respect de la casse qui est un avantage supplémentaire. La capture d'écran suivante visualiser l'utilisateur sur la commande aide sous JFeatures.



.. code-block:: bash

 kevell@corp:/# jrush JFeature help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command manages the JFeature Component for Stage Migration.

  JFeature, jfeature

        - folder-defaults
          Reset the feature file storage folders being used to the default
          example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"

        - feature-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"

        - feature-pull
          perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
          example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

        - feature-push
          perform a push on an installed feature so it is saved locally.
          example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

        - group-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"

        - group-install-all
          Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
          Directory for group files, and install or update all found groups.
          example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"

        - group-push
          perform a push of a group profile into a locally saved file.
          example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"

        - group-pull
          perform a pull on all installed features in the specified group so they are integrated into the site, db and
          file changes executed.
          example jrush jfeature group-pull --group-id="XX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-name="my group" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-unique="XX1234" --config-file="/var/www/website/configuration.php"

 ------------------------------
 End Help
 ****************************************



Alternative Paramètre
-----------------------------------

Les autres paramètres qui peuvent être définis dans les déclarations sont les suivants :


JFeature, jfeature


Dossier par défaut
----------------------

Ce processus permet de définir la valeur par défaut pour le dossier de stockage de fichiers. Un paramètre prédéfini ou une valeur qui sera utilisée si aucun choix n'est fait dans le dossier. Intervention de l'utilisateur devrait être exigée. Définissant des valeurs par défaut aux options plus couramment sélectionnées sert cet objectif.

La commande help pour processus de dossier par défaut est illustrée ci-dessous.


.. code-block:: bash

	 Jrush JFeature folder-defaults

La capture d'écran suivante montre sa fonction.


.. code-block:: bash

 	folder-defaults
        Reset the feature file storage folders being used to the default
        example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"


Feature-install
----------------------
Ce processus permet d'installer les métadonnées pour une migration de base de données. Ici il demande nom fonction et le nom de fichier configuré. L'utilisateur doit saisir tous les détails ci-dessus un par un. Sinon, l'utilisateur peut entré comme tout dans une même ligne. La commande suivante est utilisée pour installer jfeature.


.. code-block:: bash

	 Jrush JFeature feature-install


La capture d'écran montre ses fonctions.


.. code-block:: bash

       feature-install
       Install the metadata for a database migration, fileset, or both from the GC Features component
       example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"


Feature-Pull
-------------------

Extraction de caractéristique utilisée pour effectuer une traction sur une fonctionnalité installée. En raison de l'intégration des modifications apportées au fichier peuvent être exécutées.La commande suivante peut être utilisée pour extraire le fichier de configuration.


.. code-block:: bash

	 Jrush JFeature feature-pull


Après saisie la commande dudit ci-dessus, il demande l'heure et une adresse Ip. Sur cette base traction peut être exécutée. La capture d'écran suivante expliquer sa fonction.


.. code-block:: bash

	feature-pull
        perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
        example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
        example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

Feature-Push
--------------------

Poussoir de fonction utilisé pour réalise une pression sur une fonctionnalité installée. Lorsque poussant se termine il peut être enregistré localement. La commande utilisée pour pousser la fonctionnalité.


.. code-block:: bash

	 Jrush JFeature feature-push


Après l'entrée de la commande dudit ci-dessus, il demande profil unique et type de fichier et appuyez sur configuration. L'utilisateur doit entrer un par un, ou tout dans la même ligne. Cela peut s'expliquer comme suit par le biais de clichés,


.. code-block:: bash

 	feature-push
        perform a push on an installed feature so it is saved locally.
        example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

Group-install
-------------------

Ce processus permet d'installer les métadonnées pour une migration de base de données. Ici il demande le nom de fichier pour le groupe fonction et nom de fichier configuré. L'utilisateur doit saisir tous les détails ci-dessus un par un. Sinon, l'utilisateur peut d'entrée comme tout dans une même ligne.


.. code-block:: bash

	 Jrush JFeature group-install

La capture d'écran montre ses fonctions.


.. code-block:: bash

	group-install
        Install the metadata for a database migration, fileset, or both from the GC Features component
        example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"


Group-install-all
-----------------------------

Ce processus permet d'installer des métadonnées pour le fichier de migration de base de données définie. Composant de caractéristiques de configuration de groupe. Installation et mise à jour est possible. La commande suivante permet d'installer le groupe tous.

.. code-block:: bash

	 Jrush JFeature group-install-all


Entrer la commande dudit ci-dessus qu'il demande le fichier de configuration. L'utilisateur peut entrer le nom de fichier de configuration. L'écran suivant tourné guides de l'utilisateur pour installer le groupe tous.



.. code-block:: bash

	group-install-all
        Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
        Directory for group files, and install or update all found groups.
        example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"



Group-push
------------------ 

Ce processus peut exécuter un push d'un profil de groupe en fichier local. Groupe unique et nom de fichier de configuration peuvent être mentionnés ici. La commande suivante utilisée pour pousser dans le profil du groupe local enregistré le fichier.



.. code-block:: bash

	 Jrush JFeature group-push

L'écran suivant tourné guides de l'utilisateur pour installer le poussoir de groupe.


.. code-block:: bash

	 group-push
         perform a push of a group profile into a locally saved file.
         example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"


avantages
-----------------

* Bien pris en charge pour tous les types d'utilisateurs 
* Easy aux mises à jour 
* chercher mieux, plus intelligent recherche 
* extensibilité puissante 
* faire plus avec moins de temps à passer pour le codage et faire plus avec 
  moins de commandes de jfeature 
* bien faire avec Ubuntu et Cent OS 
* Non respect de la casse
