======================
System Detection
======================


synopsis
-----------

Ce module vise à détecter la machine de l'utilisateur et dans la main leur fournit les informations nécessaires à leur sujet le système des utilisateurs. Il fournit également une installation pour les utilisateurs de configurer leurs paramètres d'applications. Les quelques exemples de paramètres d'applications comprend mon utilisateur sql admin, Architecture, utilisateur admin, hôte, la version, le type de linux, Distro. Il est à l'aise avec Ubuntu et cent OS.

Commande Aide
--------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules de détection du système. Les listes de commandes de l'aide sur les autres paramètres de détection du système sous module de ptdeploy. Il décrit également la syntaxe pour détecter la machine de l'utilisateur. La commande d'aide pour la détection du système est illustré ci-dessous.

.. code-block:: bash

		ptdeploy systemdetection help

La syntaxe de la non cas de commande d'aide sensible qui ajoute un avantage pour ce module. Visualiser l'utilisateur sur la commande d'aide en vertu du système de détection de la capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptdeploy systemdetection help
 ******************************


  This is a default Module and provides you with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  SystemDetection, system-detection, systemdetection

        - detect
        Detects the Operating System
        example: ptdeploy system-detection detect

 ------------------------------
 End Help
 ******************************


détecter
-----------

Détecter utilisé pour détecter les paramètres du système. En utilisant une seule commande, l'utilisateur peut obtenir toutes les informations sur l'application du système.
La commande utilisée pour la détection du système est donnée ci-dessous.

.. code-block:: bash

		ptdeploy systemdetection detect

Après avoir entré la commande ci-dessus, le processus de détection du système commence. Pendant la détection du système de l'information suivante au sujet de la machine correspondante sont signalés:


* Système d'exploitation
* Type Linux
* Distro
* Version
* architecture
* Nom d'hôte
* Adresse IP 0.
* Adresse IP 1.

Enfin, après la détection des informations concernant les caractéristiques mentionnées ci-dessus sont clairement signalé. La capture d'écran suivante vous montre sur le processus de détection du système.

.. code-block:: bash

 kevell@corp:/# ptdeploy system-detection detect
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: Kevells
 IP Address 0: 127.0.0.1
 IP Address 1: 192.168.1.18

 ------------------------------
 Detection Finished
 ******************************




Autres paramètres
----------------------------------

Au lieu de détection du système, les paramètres suivants peuvent être utilisés:
* System Detection
* system-detection
* system detection


Avantages
-------------
* Les utilisateurs peuvent configurer les paramètres de l'application en utilisant ce système détections.
* Les paramètres utilisés pour déclarer commande d'aide, la détection du système ne sont pas sensibles à la casse, dont un avantage 
  supplémentaire par rapport à tout autres est.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
* Non sensible à la casse.
* Protection et sécurité est possible. Prévention des dommages au système et aux ressources, grâce à des processus internes ou de tiers 
  malveillants. 
* Authentification, la propriété et l'accès restreint sont parties évidentes de ce système.
* Les administrateurs système déterminent généralement l'interface utilisateur démarre avec lors de leur première connexion.
* Généralement écrit en PHP, même si certains sont écrits en assembleur pour des performances optimales.

Le module de détection de système fournit le support:

* Identifier un processus à distance et / ou de l'hôte avec lequel communiquer.
* Établir un lien entre les deux processus.
* Ouvrez et fermez la connexion si nécessaire.
* Transmettre les messages le long de la connexion.

