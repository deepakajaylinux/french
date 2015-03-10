==============
Nginx Control
==============


Synopsis
-------------

Nginx (prononcez "moteur-x") est une inverse serveur open source proxy pour HTTP, HTTPS, SMTP, POP3 et protocoles IMAP, ainsi que d'un équilibreur de charge, cache HTTP, et un serveur Web (serveur d'origine). Le projet de nginx a commencé avec un fort accent sur la concurrence élevée, haute performance et faible utilisation de la mémoire. Il est placé sous la licence BSD-like 2 article et il fonctionne sur Linux, BSD, variantes Mac OS X, Solaris, AIX, HP-UX, ainsi que sur d'autres saveurs nix.

Nginx utilise une approche asynchrone event-driven aux demandes de manutention, à la place du modèle de serveur Apache HTTP par défaut à une approche fileté ou axée sur les processus, où le MPM de l'événement est nécessaire pour le traitement asynchrone. L'architecture événementielle modulaire de Nginx peut fournir une performance plus prévisible sous fortes charges.


Commande Aide
---------------------

Cette commande permet de déterminer l'utilisation d'un module Nginx. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash

	ptdeploy nginxcontrol help
  

 kevell@corp:/# ptdeploy NginxControl help

 ******************************

  This command is part of Default Modules and handles Nginx Server Control Functions.
  NginxControl, nginxcontrol, nginxctl

          - start
          Start the Nginx server
          example: ptdeploy nginxcontrol start

          - stop
          Stop the Nginx server
          example: ptdeploy nginxcontrol stop

          - restart
          Restart the Nginx server
          example: ptdeploy nginxcontrol restart

          - reload
          Reloads the Nginx server configuration without restarting
          example: ptdeploy nginxcontrol reload

 ------------------------------
 End Help
 ******************************

début
----------------

Lorsque l'utilisateur a besoin pour démarrer le serveur Nginx, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

		ptdeploy nginxcontrol start                           

Avant l'exécution, le système demander la confirmation de procéder, si vous voulez continuer entrez «Y», si aucune entrez 'N'.


Arrêtez
----------------

Lorsque l'utilisateur doit arrêter le serveur Nginx, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

		ptdeploy nginxcontrol stop	

Avant l'exécution, le système demander la confirmation de procéder, si vous voulez continuer entrez «Y», si aucune entrez 'N'.



redémarrage
----------------

Lorsque l'utilisateur a besoin de redémarrer le serveur Nginx (quand il ya des changements ont eu lieu dans le fichier de configuration de cette option sera utilisée), la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

		ptdeploy nginxcontrol restart                          

Avant l'exécution, le système demander la confirmation de procéder, si vous voulez continuer entrez «Y», si aucune entrez 'N'.


recharger
----------------

Lorsque l'utilisateur doit Recharger le serveur Nginx sans redémarrer, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

		ptdeploy nginxcontrol reload



Avant l'exécution, le système demander la confirmation de procéder, si vous voulez continuer entrez «Y», si aucune entrez 'N'.



Option
---------------
                               
.. cssclass:: table-bordered

 +------------------------------+----------------------------------------------------------------+----------------------------------------+
 | Paramètres                   | alternatifs  Paramètres                                        | Commentaires                           |
 +==============================+================================================================+========================================+
 |ptdeploy ngnixcontrolhelp     | Soit des trois paramètre alternatif peut être utilisé dans la  | Une fois que l'utilisateur fournit     |
 |                              | commande - ngnixcontrol , NgnixControl and nginxcil            | l'option, le système commence le       |
 |                              | eg: ptdeploy ngnixcontrol help/ ptdeploy ngnixControl help     | traitement|                            |
 +------------------------------+----------------------------------------------------------------+----------------------------------------+


avantages
--------------

* Capacité à gérer plus de 10 000 connexions simultanées avec une faible empreinte mémoire
* Gestion des fichiers statiques, les fichiers d'index, et l'auto-indexation
* Reverse proxy avec cache
* Équilibrage de charge avec des contrôles de santé dans la bande-
* Tolérance aux pannes
* TLS / SSL avec la SNI et OCSP soutien d'agrafage, via OpenSSL.
* FastCGI, SCGI, le soutien uwsgi avec la mise en cache
* Nom du produit- et IP des serveurs virtuels basés sur l'adresse
* Compatibles IPv6
* Support du protocole SPDY
* WebSockets et HTTP / 1.1 de mise à niveau (101 Protocoles de commutation)
* FLV et MP4 en streaming
* Page authentification d'accès Web
* Compression gzip et la décompression
* La réécriture d'URL
* Journalisation personnalisé avec la compression gzip sur la volée
* Le taux de réponse et de requêtes simultanées de limitation
* Limitation de bande passante
* Server Side Includes
* Géolocalisation basée sur l'adresse IP
* Suivi des utilisateurs
* WebDAV
* Le traitement des données de style XSLT
* Intégré scripts Perl


