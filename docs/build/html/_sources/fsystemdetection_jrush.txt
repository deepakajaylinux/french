======================
System Detection
======================

synopsis
-----------------

Ce module vise à détecter l'ordinateur de l'utilisateur et à la main leur fournit les informations nécessaires à eux concernant le système des utilisateurs. Il fournit également une installation pour les utilisateurs à configurer leurs paramètres d'applications. Les quelques exemples pour les paramètres des applications inclut mon sql admin utilisateur, Architecture, admin utilisateur, hôte, de version, de type linux, distribution. C'est à l'aise avec Ubuntu et cent OS.


Commande Aide
-----------------------

La commande help conduit les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans les modules de détection du système. La commande help répertorie les paramètres alternatifs de détection des systèmes sous le module de Jrush. Il décrit également la syntaxe pour détecter l'ordinateur de l'utilisateur. La commande help pour la détection des systèmes est illustrée ci-dessous.


.. code-block:: bash

	jrush systemdetection help


La syntaxe pour la commande help non respect de la casse qui ajoute un avantage pour ce module. La capture d'écran suivante visualiser l'utilisateur sur la commande aide dans la détection des systèmes.



.. code-block:: bash

 kevell@corp:/# jrush systemdetection help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This is a default Module and provides you with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  SystemDetection, system-detection, systemdetection

        - detect
        Detects the Operating System
        example: ptconfigure system-detection detect

 ------------------------------
 End Help
 ****************************************



Detect
----------


Détecter pour détecter les paramètres du système. À l'aide d'une seule commande, l'utilisateur peut obtenir toutes les informations sur l'application du système.  La commande utilisée pour la détection des systèmes est donnée ci-dessous.


.. code-block:: bash

	jrush systemdetection detect

Après la saisie de la commande ci-dessus, le processus de détection du système démarre. Lors de la détection du système les informations suivantes concernant la machine correspondante sont signalées :



* Operating System
* Linux Type
* Distro
* Version
* Architecture
* Host Name
* IP Address 0.
* IP Address 1.

Enfin, après détection de l'information au sujet de ce qui précède mentionné caractéristiques sont clairement signalés. La capture d'écran suivante vous montre le processus de détection des systèmes.



.. code-block:: bash

 kevell@corp:/# ptconfigure system-detection detect
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: udayakumar
 IP Address 0: 127.0.0.1
 IP Address 1: 192.168.1.24

 ------------------------------
 Detection Finished
 ******************************


Alternative Paramètre
----------------------------------

Au lieu de détection du système, les paramètres suivants peuvent être utilisés :


* System Detection
* system-detection
* system detection

avantages
-------------

* Les utilisateurs peuvent configurer les paramètres d'application à l'aide de détections de ce système. * Les paramètres utilisés pour 
  déclarer la commande help, détection des systèmes ne sont pas sensibles à la casse qui est un avantage supplémentaire alors que par rapport a  ux autres. 
* C'est aisée dans les deux Cent OS et ainsi comme dans Ubuntu. 
* La protection et la sécurité est possible. Prévention des dommages au système et aux ressources, par le biais de processus internes ou 
  étrangers malveillants.  L'authentification, la propriété et un accès restreint sont des pièces évidentes de ce système. 
* Les administrateurs système généralement déterminer quelle interface utilisateur commence par lorsqu'ils connectent tout d'abord po 
* généralement écrit en PHP, bien que certains soient écrits en Assemblée pour des performances optimales.


Le module de détection du système fournit la prise en charge :

* Identifier un processus distant et/ou l'hôte avec lequel communiquer. 
* Établir une connexion entre les deux processus. 
* Ouvrir et fermer la connexion si nécessaire. 
* Transmettre des messages le long de la connexion.


  


