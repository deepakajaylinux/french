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

 +-------------------+-------------------+------------------------------+------------------------------------------------------------------+
 | paramètres        | Autres paramètres | fonctions                    | commentaire                                                      |
 +===================+===================+==============================+==================================================================+
 |start              | Service, service  | Lancer un service de système | ptconfigure service start –service-name=”apache2”                |
 |                   |                   |                              | –service-name=”apache2”                                          | 
 +-------------------+-------------------+------------------------------+------------------------------------------------------------------+
 |stop               | Service, service  | Arrêtez le service Asystem   | ptconfigure service stop –service-name=”apache2”                 |
 |                   |                   |                              |                                                                  |
 +-------------------+-------------------+------------------------------+------------------------------------------------------------------+
 |Restart            | Service, service  | Lancer un service de système | ptconfigure service restart –service-name=”apache2”              |
 |                   |                   |                              |                                                                  |
 +-------------------+-------------------+------------------------------+------------------------------------------------------------------+
 |Ensure-running     | Service, service  | Fournir un service système   | ptconfigure service ensure-running –service- name=”apache2”      |
 |                   |                   | running.In Lorsqu'il  ne est |                                                                  |
 |                   |                   | pas en cours d'exécution, il |                                                                  |
 |                   |                   | ne serait pas commencer à    |                                                                  |
 |                   |                   | essayer autrement            |                                                                  |
 +-------------------+-------------------+------------------------------+------------------------------------------------------------------+
 |Is-running         | Service, service  | Vérifier si un service de    | ptconfigure service is-running –service-name=”apache2”           |
 |                   |                   | système est en               |                                                                  |
 |                   |                   | fonctionnement ou pas, il ne |                                                                  |
 |                   |                   | serait pas commencer à       |                                                                  |
 |                   |                   | essayer autrement            |                                                                  |
 +-------------------+-------------------+------------------------------+------------------------------------------------------------------+
 |Run-at-reboots     | Service, service  | Assurer une autostart de     | ptconfigure service run-at-reboots –service- name=”apache2       |
 |                   |                   | service du système au        |                                                                  | 
 |                   |                   | redémarrage|                 |                                                                  |
 +-------------------+-------------------+------------------------------+------------------------------------------------------------------+


Le represenation picturale de la commande start , stop, restart , Ensure-running, Is-running and Run-at-reboots sont énumérés ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure service start --service-name="apache2"

 [Pharaoh Logging] Starting apache2 service
 * Starting web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure service stop --service-name="apache2"

 [Pharaoh Logging] Stopping apache2 service
 * Stopping web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure service restart --service-name="apache2"

 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptconfigure service ensure-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service is-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service run-at-reboots --service-name="apache2"

 [Pharaoh Logging] Removing current apache2 service startup links
 Removing any system startup links for /etc/init.d/apache2 ...
   /etc/rc0.d/K09apache2
   /etc/rc1.d/K09apache2
   /etc/rc2.d/S91apache2
   /etc/rc3.d/S91apache2
   /etc/rc4.d/S91apache2
   /etc/rc5.d/S91apache2
   /etc/rc6.d/K09apache2
 [Pharaoh Logging] Adding apache2 service startup links
 Adding system startup for /etc/init.d/apache2 ...
   /etc/rc0.d/K20apache2 -> ../init.d/apache2
   /etc/rc1.d/K20apache2 -> ../init.d/apache2
   /etc/rc6.d/K20apache2 -> ../init.d/apache2
   /etc/rc2.d/S20apache2 -> ../init.d/apache2
   /etc/rc3.d/S20apache2 -> ../init.d/apache2
   /etc/rc4.d/S20apache2 -> ../init.d/apache2
   /etc/rc5.d/S20apache2 -> ../init.d/apache2
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************



avantages
---------

* L'utilisateur peut vérifier l'état du système de travail à tout moment.
* Service fournit d'échanger des données entre le système.
* Il permet le partage des ressources de la machine
* Service fournit également la fonction de back-up.
* Service fournit un environnement de réseau flexible.
* Il se agit de la coordination des données distribuées.


