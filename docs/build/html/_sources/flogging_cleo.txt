=========
Logging
=========

synopsis
------------------

Ce module se connecte une information sur le panneau de contrôle et éventuellement journal php.

Le processus d'utilisation de ce module pour recueillir des données grâce à des capteurs, analyser les données et enregistrer et d'afficher les résultats de la collecte et l'analyse. Logging implique aussi le panneau de configuration du système installe et analyse les données. Sensibilité non de cas est une couronne pour ce module. Cela convient de travailler avec Ubuntu et cent OS.

Commande Aide
-----------------------

Cette commande peut fonctionner sur les objectifs et les commandes disponibles dans le cadre du module de journalisation ptconfigure. Il explique également la commande pour installer le module de journalisation. Avant l'installation, l'utilisateur peut lire cette commande d'aide explique sa fonction.

.. code-block:: bash
        
	        ptconfigure logging help


Les captures d'écran suivantes peuvent visualiser la commande d'aide

.. code-block:: bash


 kevell@corp:/# ptconfigure Logging help

 ******************************


  Use this to log a message to the Console, and optionally also the php error log.

  Logging, logging

        - log
        Logs a message to the console and optionally the php log
        example: ptconfigure logging log --log-message="Here is something logging to the console and error log"
        example: ptconfigure logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************


installation
-----------------

Ces procédures d'installation sont log contrôle de php. Cette section fournit des informations sur la compatibilité et les exigences, instructions de base sur la façon d'installer et configurer ptconfigure à l'information plus détaillée. Cette commande peut fonctionner sur les objectifs et les commandes disponibles sous module de journalisation ptconfigure. Il explique également la commande pour installer le module de journalisation. Avant l'installation, l'utilisateur peut lire cette commande d'aide explique sa fonction.

.. code-block:: bash
        
                ptconfigure logging  log


Les captures d'écran suivantes peuvent visualiser la commande d'aide

.. code-block:: bash

 kevell@corp:/# ptconfigure logging log 

 Install Logging? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Logging: Success
 ------------------------------
 Installer Finished
 ******************************



Option
------------

.. cssclass:: table-bordered

 +--------------------------+---------------------------------+-------------+----------------------------------------------+
 | Paramètres               | alternative paramètres          | Option      | Commentaires                                 |
 +==========================+=================================+=============+==============================================+
 |ptconfigure logging       | Nous pouvons utiliser Logging,  | Y           | Le système démarre processus de journal      |
 |Install                   | logging                         |             | sous ptconfigure                             |
 +--------------------------+---------------------------------+-------------+----------------------------------------------+
 |ptconfigure logging       | Nous pouvons utiliser Logging,  | N           | Système arrête processus de journal          |
 |Install                   | logging                         |             | sous ptconfigure|                            |
 +--------------------------+---------------------------------+-------------+----------------------------------------------+


avantages
-------------

* Visualisation en temps réel de données
* Sensibilité non de cas
* Fonctionnalité définie par l'utilisateur
* Téraoctets de stockage de données
* Connectivité réseau
* Eh bien à faire dans Ubuntu et cent OS
