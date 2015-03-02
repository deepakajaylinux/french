==========
Service
==========


synopsis
----------
          
Ce module facilite l'état actuel du fichier dans le système. Il peut parler de l'état comme la course ou non. L'automatisation est possible. Ce module précise la configuration de votre environnement. Il est amical avec Ubuntu et cent OS utilisateur.

Commande Aide
-------------

Aide commande utilisée pour trouver des informations sur une commande spécifique. Pour plus d'informations sur les changements à la fonctionnalité du service que nous pouvons utiliser cette commande d'aide. La capture d'écran suivante vous guidera.

.. code-block:: bash

    ptconfigure Service help


.. code-block:: bash

	Kevell@corp:/# ptconfigure Service help

	******************************


	  This command allows you to view or modify service

	  Service, service

        - start
        Start a system service
        example: ptconfigure service start --service-name="apache2"

        - stop
        Stop a system service
        example: ptconfigure service restart --service-name="apache2"

        - restart
        Restart a system service
        example: ptconfigure service restart --service-name="apache2"

        - ensure-running
        Ensure a system service is running. If it is already running, dont attempt to start it
        If it is not running, start it
        example: ptconfigure service ensure-running --service-name="apache2"

        - is-running
        Checks whether a system service is running.
        example: ptconfigure service is-running --service-name="apache2"

        - run-at-reboots
        Ensure a system service will auto start on reboots.
        example: ptconfigure service run-at-reboots --service-name="apache2"

	------------------------------
	End Help
	******************************


Options
------------

.. cssclass:: table-bordered

 +-------------------+-------------------------------------------------+-------------------------------------------------------------------+
 | paramètres        | fonctions                                       | commentaire                                                       |
 +===================+=================================================+===================================================================+
 |start              | Lancer un service de système                    | ptconfigure service start –service-name=”apache2”                 |
 +-------------------+-------------------------------------------------+-------------------------------------------------------------------+
 |stop               | Arrêtez le service Asystem                      | ptconfigure service stop –service-name=”apache2”                  |
 +-------------------+-------------------------------------------------+-------------------------------------------------------------------+
 |Restart            | Lancer un service de système                    | ptconfigure service restart –service-name=”apache2”               |
 +-------------------+-------------------------------------------------+-------------------------------------------------------------------+
 |Ensure-running     | Fournir un service système running.In Lorsqu'il | ptconfigure service ensure-running –service- name=”apache2”       |
 |                   | ne est pas en cours d'exécution, il ne serait   |                                                                   |
 |                   | pas commencer à essayer autrement               |                                                                   |
 +-------------------+-------------------------------------------------+-------------------------------------------------------------------+
 |Is-running         | Vérifier si un service de système est en        | ptconfigure service is-running –service-name=”apache2”            |
 |                   | fonctionnement ou pas, il ne serait pas         |                                                                   |
 |                   | commencer à essayer autrement                   |                                                                   |
 +-------------------+-------------------------------------------------+-------------------------------------------------------------------+
 |Run-at-reboots     | Assurer une autostart de service du système au  | ptconfigure service run-at-reboots –service- name=”apache2        |
 |                   | redémarrage|                                    |                                                                   |
 +-------------------+-------------------------------------------------+-------------------------------------------------------------------+


avantages
---------

* L'utilisateur peut vérifier l'état du système de travail à tout moment.
* Service fournit d'échanger des données entre le système.
* Il permet le partage des ressources de la machine
* Service fournit également la fonction de back-up.
* Service fournit un environnement de réseau flexible.
* Il se agit de la coordination des données distribuées.


