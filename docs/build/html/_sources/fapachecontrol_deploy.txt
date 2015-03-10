================
ApacheControl
================

synopsis
-------------

Ce module est un des modules par défaut qui vise à manipuler les fonctions de commande du serveur Apache. Il permet et facilite les fonctions de contrôle nécessaires qui doivent être effectuées dans le serveur Apache. Voyons, le fonctionnement et le but des fonctions de contrôle et comment ces modules liés à la manipulation de ces fonctions de contrôle du serveur Apache.

Commande Aide
---------------------

Les actes de commandement de l'aide comme un guide de l'utilisateur brève qui conduit les utilisateurs comment manipuler et à utiliser ce module particulier.

La syntaxe de commande help sous le contrôle Apache est indiqué ci-dessous:

.. code-block:: bash

		ptdeploy ApacheControl help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La commande help répertorie également les autres paramètres qui peuvent être utilisés dans la déclaration. La capture d'écran ci-dessous vous visualiser sur la commande d'aide sous contrôle Apache.

.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheControl help
 ******************************


  This command is part of Default Modules and handles Apache Server Control Functions.

  ApacheControl, apachecontrol, apachectl

          - start
          Start the Apache server
          example: ptdeploy apachecontrol start
          example: ptdeploy apachecontrol start --yes --guess
          example: ptdeploy apachecontrol start --yes --apache-command="apache2"

          - stop
          Stop the Apache server
          example: ptdeploy apachecontrol stop
          example: ptdeploy apachecontrol stop --yes --guess
          example: ptdeploy apachecontrol stop --yes --apache-command="apache2"

          - restart
          Restart the Apache server
          example: ptdeploy apachecontrol restart
          example: ptdeploy apachecontrol restart --yes --guess
          example: ptdeploy apachecontrol restart --yes --apache-command="apache2"

          - reload
          Reloads the Apache server configuration without restarting
          example: ptdeploy apachecontrol reload
          example: ptdeploy apachecontrol reload --yes --guess
          example: ptdeploy apachecontrol reload --yes --apache-command="apache2"

 ------------------------------
 End Help
 ******************************

Les quatre fonctions de contrôle de base inclus dans le serveur Apache sont:

* Début
* Arrêtez
* Redémarrage
* Reload

Il ya trois façons possibles en définissant un fonctions de contrôle. Par exemple, si nous prenons fonction de démarrage, il peut être défini de trois manières différentes, comme l'exige l'utilisateur comme indiqué ci-dessous.

.. code-block:: bash
		
		ptdeploy ApacheControl start

or 

.. code-block:: bash

		ptdeploy ApacheControl start --yes --guess

or

.. code-block:: bash

		ptdeploy ApacheControl start --yes --apache-command="apache2"

Voyons l'utilisation de trois syntaxe différente en déclarant dans les prochains sujets.

paramètres alternatifs
-------------------------------

Voici les autres paramètres qui peuvent être définis dans les déclarations:

ApacheControl, apachecontrol, apachectl

fonction de démarrage
------------------------

Si l'utilisateur souhaite activer la fonction de commande d'Apache, le peut utiliser les syntaxes suivantes, comme indiqué:

.. code-block:: bash

		ptdeploy ApacheControl start

		(Ce est le premier type de syntaxe pour définir une fonction de contrôle pour apche serveur)

Après avoir saisi la commande comme ci-dessus, les étapes suivantes sont effectuées:

Étape 1: Voulez-vous commencer Apache? (Y / N).

L'utilisateur doit indiquer Y ou N.

Étape 2: Quel est le nom du service apache?

(0) apache2

(1) httpd

L'utilisateur doit spécifier si 0 ou 1 que par l'exigence.

Après avoir obtenu l'entrée du nom de service d'Apache, il sera démarre le processus.

La capture d'écran ci-dessous illustre le processus de démarrage imagée.

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol start
 Do you want to Start Apache? (Y/N)
 y
 What is the apache service name?
 (0) apache2
 (1) httpd
 0
 Starting Apache...
 * Starting web server apache2
 *
 ******************************


 1Apache Controller Finished
 ******************************

Fonction d'arrêt
------------------

Si l'utilisateur désire arrêter la fonction de contrôle d'Apache, le peut utiliser les syntaxes suivantes, comme indiqué:

.. code-block:: bash

		ptdeploy apachecontrol stop --yes --guess
		
		(Ce est le deuxième type de syntaxe dans la définition d'une des fonctions de contrôle pour serveur apache)

L'option de proposition peut être utilisé pour effectuer un valeurs par défaut des fonctions définies particulières.

Pour l'ubuntu apche2 est la valeur par défaut.

Pour Cent OS httpd est la valeur par défaut.

La capture d'écran ci-dessous vous montre à propos de la fonction d'arrêt et le but d'options guess imagée.

.. code-block:: bash

 kevells@corp:/# ptdeploy apachecontrol stop --yes --guess
 Stopping Apache...
 * Stopping web server apache2
 *
 ******************************


 1Apache Controller Finished
 ******************************

Redémarrez une fonction
-------------------------

Si l'utilisateur souhaite redémarrer la fonction de contrôle d'Apache, le peut utiliser les syntaxes suivantes, comme indiqué:

.. code-block:: bash
	
		ptdeploy apachecontrol restart --yes --apache-command="apache2"
	
		(Ce est le troisième type de syntaxe dans la définition d'une des fonctions de contrôle pour apche serveur)

L'utilisateur peut utiliser ce troisième type de syntaxe pour spécifier la valeur de la commande apache nécessaire. La capture d'écran comme ci-dessous illustre ce troisième type de syntaxe et processus de redémarrage fonction imagée.

.. code-block:: bash

 kevells@corp:/# ptdeploy apachecontrol restart --yes --apache-command="apache2"
 Restarting Apache...
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globa lly to suppress this message
 * Restarting web server apache2
 â€‚
  ....done.
 ******************************


 1Apache Controller Finished
 ******************************

Rechargement une fonction
----------------------------

Si l'utilisateur souhaite recharger la fonction de contrôle d'Apache, le peut utiliser les syntaxes suivantes, comme indiqué:

.. code-block:: bash

		ptdeploy apachecontrol reload

or

.. code-block:: bash

		ptdeploy apachecontrol --yes --guess
or

.. code-block:: bash

		ptdeploy apachecontrol --yes --apache-command="apache2"

La fonction de rechargement effectue le rechargement du serveur Apache sans redémarrer.

avantages
-----------

* Il est bon de le faire dans les deux cent-OS et Ubuntu.
* Les paramètres utilisés pour les déclarations ne sont pas sensibles à la casse, ce qui est un avantage supplémentaire en rapport aux autres.
* Il ya trois syntaxe différente utilisée pour la déclaration, l'utilisateur peut choisir un d'entre eux selon les exigences.
* La syntaxe trois différents sont applicables pour tous les quatre fonctions de contrôle de démarrage, d'arrêt, redémarrer, recharger.
