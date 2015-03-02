========
Port
========

synopsis
-------------

Port certifie pour vérifier l'état des ports et des services. Ce module permet de vérifier le service portuaire en vertu de ptconfigure. Ce module est le plus à l'aise avec Ubuntu et cent OS.

Aidez-Moi
-------------

Cette commande d'aide à guider l'utilisate

.. code-block:: bash

          ptconfigure port help

La commande d'aide montre une courte liste des commandes intégrées dans le module de port.

.. code-block:: bash

	kevell@corp:/# ptconfigure Port  help
	******************************


	  This command allows you to test the status of ports and services running on them

	  Port, port

        - is-responding
        Test if a port is responding
        example: ptconfigure port is-responding --port-number="25"

        - process
        See which process is using a port
        example: ptconfigure port process --port-number="25"

	------------------------------
	End Help
	******************************


hôte local
---------------

Lorsque l'utilisateur veut vérifier l'état du port de l'hôte local alors il peut demander à l'utilisateur son adresse IP. Se expliquer la capture d'écran ci-dessous.

.. code-block:: bash


   	kevell@corp:/# ptconfigure port process --port-number="22"

	[Pharaoh Logging] Port 22 is being used by the process sshd
	******************************


	Port Modifications:
	--------------------------------------------

	Port: Success

	------------------------------
	Port Mods Finished
	******************************


Options
--------------- 

.. cssclass:: table-bordered


 +------------------------+----------------------------------------+----------------------+-------------------------------------+
 | Paramètres             | Fuctions                               | Autres paramètres    | sortie                              |
 +========================+========================================+======================+=====================================+
 |is-responding           | Essai de port est de répondre ou pas   | Port,port            | Il répond au processus de Port      |
 +------------------------+----------------------------------------+----------------------+-------------------------------------+
 |Process                 | Testez l'état du processus de ports    | Port,port            | Il affichera le processus de Port|  |
 +------------------------+----------------------------------------+----------------------+-------------------------------------+



avantages
-------------

* L'utilisateur peut vérifier l'état de fonctionnement actuel du port.
* Ce est un module convivial.
* Moins de temps.
