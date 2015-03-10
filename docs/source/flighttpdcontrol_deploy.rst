=====================
LighttpdControl
=====================

synopsis
---------------

Lighttpd est un serveur web sécurisé, rapide, conforme, et très flexible qui a été optimisé pour les environnements haute performance. Lighttpd qui est en train de redéfinir rapidement l'efficacité d'un ptdeploy; comme il est conçu et optimisé pour les environnements de haute performance. Avec une faible empreinte mémoire par rapport à d'autres serveurs web, une gestion efficace de la charge CPU, et ensemble de fonctionnalités avancées lighttpd est la solution parfaite pour chaque serveur qui souffre des problèmes de charge. Ce est apte à travailler avec Ubuntu et cent OS.

Commande Aide
----------------------

Aide permet d'accéder à l'information sur lighttpd. Pour une référence rapide aux commandes d'aide de l'une des versions de ptdeploy vous pouvez également utiliser la commande d'aide. La commande d'aide est une commande interne et est disponible dans le module ptdeploy.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol help


La capture d'écran ci-dessous aide l'utilisateur à la servitude avec ptdeploy.

.. code-block:: bash

 kevell@corp:/# ptdeploy LighttpdControl help
 ******************************


  This command is part of Default Modules and handles Lighttpd Server Control Functions.

  LighttpdControl, lighttpdcontrol, lighttpdctl

          - start
          Start the Lighttpd server
          example: ptdeploy lighttpdcontrol start
          example: ptdeploy lighttpdcontrol start --yes

          - stop
          Stop the Lighttpd server
          example: ptdeploy lighttpdcontrol stop
          example: ptdeploy lighttpdcontrol stop --yes

          - restart
          Restart the Lighttpd server
          example: ptdeploy lighttpdcontrol restart
          example: ptdeploy lighttpdcontrol restart --yes

          - reload
          Reloads the Lighttpd server configuration without restarting
          example: ptdeploy lighttpdcontrol reload
          example: ptdeploy lighttpdcontrol reload --yes

 ------------------------------
 End Help
 ******************************


Alternative Paramètre
--------------------------------

De préférence en utilisant Lighttpd l'utilisateur peut l'effort les options suivantes.

LighttpdControl, lighttpdcontrol, lighttpdctl.

début
--------

Lancer option utilisée pour démarrer le serveur lighttpd. Lighttpdcontrol est une session interactive qui est exécuté avec l'option de module ptdeploy. Selon la façon dont le serveur est exécuté, la commande de démarrage peut être stockée dans un script, dans le registre Linux.

Le serveur peut être démarré à l'aide d'une simple commande avec une option pour vous connecter Retour à contrôler serveur pour obtenir des options supplémentaires.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol start

après avoir tapé la commande, il permet à l'utilisateur de démarrer le fonctionnement du serveur lighttpd.

Arrêtez
---------

Cette option d'arrêt utilisé pour arrêter le service lighttpd. Plus précisément Ubuntu Linux, la commande d'arrêt appelle la lighttpd pour arrêter un travail qui est en cours d'exécution sur le système. Ce est l'équivalent de l'arrêt de service de commande. Voici une description complète de la commande d'arrêt.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol stop


Après l'entrée que la commande ci-dessus, le service se arrête la fonction.

redémarrage
------------

Le terme se réfère à un redémarrage du système d'exploitation de fermer tous les programmes avant un redémarrage à chaud du serveur lighttpd. Le redémarrage est parfois nécessaire pour récupérer d'une erreur, ou pour réinitialiser les pilotes ou périphériques. Un programme de stockage informatique devrait normalement effectuer un redémarrage avec la commande simple suivant.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol restart

After input as the above command, the service restart the lighttpd service.


Reload
------------

Reload means things are changing. The lighttpd is undergoing an overhaul and a clean-up. It facilitates the reuse of lighttpd and services. Without kill the process it can reload lighttpd. The following command assis the user to reload. Along with the command if the user use yes.. options without asking any questions automatically it can function.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol reloadAprès l'entrée que la commande ci-dessus, le service redémarrez le service lighttpd.


recharger
------------

Recharger signifie que les choses sont en train de changer. Le lighttpd est l'objet d'une révision et un nettoyage. Il facilite la réutilisation des lighttpd et des services. Sans tuer le processus, il peut recharger lighttpd. La commande suivante Assis à l'utilisateur de recharger. Avec la commande si l'utilisation de l'utilisateur oui .. options sans se poser de questions qu'il peut fonctionner automatiquement.

avantages
--------------

* Hébergement virtuel flexible.
* Prend en charge tous les types de modules.
* Léger (moins de 1 Mo).
* Non sensible à la casse.
* L'utilisateur peut fonctionner selon leur souhait.
* Résiliation est possible.
* L'automatisation est possible.

