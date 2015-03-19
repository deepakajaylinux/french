===================
SystemDetection
===================


synopsis
-----------

Ce module vise à détecter l'ordinateur de l'utilisateur et à la main leur fournit les informations nécessaires à eux concernant le système des utilisateurs. Il fournit également une installation pour les utilisateurs à configurer leurs paramètres d'applications. Les quelques exemples pour les paramètres des applications comprennent utilisateur mysql admin utilisateur, Architecture, admin, hébergent, version, type de linux, distribution. C'est à l'aise avec Ubuntu et cent OS.


Commande Aide
---------------

La commande help conduit les utilisateurs concernant l'objectif et ainsi que sur les options qui sont incluses dans les modules de détection du système. La commande help répertorie les paramètres alternatifs de détection des systèmes sous le module de pttest. Il décrit également la syntaxe pour détecter la machine de l'utilisateur. La commande help pour la détection des systèmes est illustrée ci-dessous.

.. code-block:: bash

	pttest systemdetection help

La syntaxe pour la commande help est le non respect de la casse qui ajoute un avantage pour ce module. La capture d'écran suivante visualiser sur la commande aide dans la détection des systèmes.


.. code-block:: bash

 kevell@corp:/# pttest systemdetection help
 ******************************


  This is a default Module and provides you with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  SystemDetection, system-detection, systemdetection

        - detect
        Detects the Operating System
        example: ptconfigure system-detection detect

 ------------------------------
 End Help
 ******************************


détecter
-----------
 

Lorsque l'utilisateur a besoin détecter les paramètres du système, le dessous étant donné de commande obtiendrez toutes les informations sur l'application du système.


.. code-block:: bash
	
	pttest systemdetection detect

Système finit de fournir le ci-dessous donnons tous les détails: 

* système d'exploitation 
* Linux Type 
* Distro 
* Version 
* Architecture 
* nom d'hôte 
* adresse IP 0.


La capture d'écran suivante vous montre le processus de détection des systèmes.


.. code-block:: bash

 kevell@corp:/# pttest system-detection detect
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: kevells
 IP Address 0: 172.16.201.1
 IP Address 1: 172.16.39.1
 IP Address 2: 192.168.1.16

 ------------------------------
 Detection Finished
 ******************************


Alternative Paramètre
----------------------------------

Au lieu de détection du système, les paramètres suivants peuvent être utilisés :


* SystemDetection
* system-detection
* systemdetection


avantages
-------------

* Les utilisateurs peuvent configurer les paramètres de l'application utilisant la détection de ce système. 
* Les paramètres utilisés pour déclarer la commande help, détection des systèmes ne sont pas sensibles à la casse qui est un avantage
  supplémentaire alors que par rapport aux autres. 
* C'est aisée dans les deux Cent OS et ainsi comme dans Ubuntu. 
* La protection et la sécurité est possible. Prévention des dommages au système et aux ressources, par le biais de processus internes ou 
  étrangers malveillants.  Authntication, propriété et accès restreint sont évidentes certaines parties de ce système. 
* Les administrateurs système généralement déterminer quelle interface utilisateur commence par lorsqu'ils connectent tout d'abord po 
* généralement écrit en PHP, bien que certains soient écrits en Assemblée pour des performances optimales.



  


