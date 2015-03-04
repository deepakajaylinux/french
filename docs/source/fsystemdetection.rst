==================
System Detection
==================

synopsis
-------------

Ce module vise à détecter la machine de l'utilisateur et dans la main leur fournit les informations nécessaires à leur sujet le système des utilisateurs. Il fournit également une installation pour les utilisateurs de configurer leurs paramètres d'applications. Les quelques exemples de paramètres d'applications comprend utilisateur admin mysql, hôte, passe.

Commande Aide
----------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules de détection du système. Les listes de commandes de l'aide sur les autres paramètres de détection Système. Il décrit également la syntaxe pour détecter la machine de l'utilisateur. La commande d'aide pour la détection du système est illustré ci-dessous.

.. code-block:: bash

	ptconfigure systemdetection help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de détection du système.

.. code-block:: bash

	kevell@corp:/# ptconfigure SystemDetection help
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

détection
------------

La commande utilisée pour la détection du système est donnée ci-dessous.

.. code-block:: bash

		ptconfigure systemdetection detect

Après avoir saisi la commande ci-dessus, le processus de détection du système commence. Pendant la détection du système de l'information suivante au sujet de la machine correspondante sont signalés:

* Système d'exploitation
* Type Linux
* Distro
* Version
* architecture
* Nom d'hôte
* Adresse IP 0.
* Adresse IP 1.

Enfin, la détection Après les informations concernant les caractéristiques mentionnées ci-dessus sont clairement signalé. La capture d'écran suivante vous montre sur le processus de détection du système.

.. code-block:: bash

        Kevell@corp:/# ptconfigure system-detection detect
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
	IP Address 1: 192.168.1.3

	------------------------------
	Detection Finished
	******************************


Autres paramètres
------------------------

Au lieu de systemdetection, les paramètres suivants peuvent être utilisés:

* SystemDetection
* Système de détection

avantages
------------

* Les utilisateurs peuvent configurer les paramètres de l'application en utilisant ce système détections.
* Les paramètres utilisés pour déclarer commande d'aide, la détection du système ne sont pas sensibles à la casse qui est un avantage 
  supplémentaire par rapport à tout autres.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
