PTVirtualize
=============

Synopsis
------------

Tout en le comparant avec ptconfigure, le ptvirtualize est un outil de gestion de machine virtuelle qui fournit les fonctionnalités pour la machine virtuelle et développement gestion de l'environnement.

À l'aide de Devops, il gère la configuration de la machine virtuelle, facilite les différents types de contributeurs, même dans un environnement de développement extrêmement complexes.

Il facilite l'automatisation, à normaliser et gérer la configuration de l'environnement virtualisé. Ses fonctionnalités inclut la gestion de la Configuration, gestion d'Automation de Test, le déploiement automatisé, Équipez et Release Management, gestion de l'environnement de développement et ces fonctionnalités sont effectuées.

En ptvirtualize la gestion de la Configuration, Infrastructure et systèmes d'automatisation est encadré en php. Modifier un script php est très facile, car il n'y a aucune étape de compilation pour réaliser.

Le ptvirtualize est orienté objet qui enrichissent non seulement le type de données, mais aussi les types d'opérations qui peuvent être appliquées aux données. Donc, tout en comparant sur des techniques de programmation procédurales, les techniques de programmation orientée objet la programmation orientée objet permet aux utilisateurs finaux de créer des modules qui n'ont pas besoin d'être changé lorsqu'un nouveau type d'objet est ajouté.

Le ptvirtualize est extensible, comme si n'importe quel module supplémentaire est nécessaire l'utilisateur peut encadrer et concevoir le module selon leurs exigences et qu'ils peuvent comprendre.

En utilisant la fonctionnalité de création de modèles option extra-modèles peuvent être ajoutés, si nécessaire. L'option SSH permet de définir une valeur de clé SSH. Le SFTP facilite la capacité de lecture et d'écriture entre les deux OS différents à l'aide de la machine virtuelle.


exigences
-----------------

Si vous souhaitez utiliser la ptvirtualize, s'assurer si la boîte Virual est installée dans votre machine, ainsi que la fonctionnalité de compléments Virtual boîte Commentaires


Code pour installer la machine virtuelle 
---------------------------------------------

.. code-block:: bash

        sudo ptconfigure virtualbox install --yes --guess --with-guest-additions

installation 
---------------

Il y a deux façons d'installer l'outil de ptvirtualize pour votre machine :

1)Installation via ptconfigure

2)Installing ptvirtualize alone

Installation via ptconfigure
-------------------------------

Si vous avez ptconfigure outil dans votre machine, il est simple d'installer le ptvirtualize en utilisant le code comme indiqué ci-dessous,


.. code-block:: bash


        sudo ptconfigure ptvirtualize install --yes --guess

ici, la conjecture de mot peut être ignoré tout en choisissant votre propre répertoire lors de l'installation.


Installation ptvirtualize seule
----------------------------------

Si vous souhaitez installer l'outil ptvirtualize à votre machine sans selon l'outil de ptconfigure, il est plus facile à l'aide de la commande,

.. code-block:: bash

        sudo apt-get install php5 git
        
Cette commande va installer php5 et git sur votre machine. Après qu'utiliser la commande suivante,::


        git clone http://github.com/PharaohTools/ptvirtualize && sudo php ptvirtualize/install-silent

la commande sur la mentionnés ci-dessus peut être utilisé si vous ne souhaitez pas sélectionner l'emplacement pendant l'installation. Si vous souhaitez le faire, utilisez la commande suivante::

        git clone http://github.com/PharaohTools/ptvirtualize && sudo php ptvirtualize/install

Méthodologies en utilisation
--------------------------------

Ici, nous devons voir comment utiliser les commandes sous l'outil et son utilisation.  

Si vous tapez simplement la commande suivante::


    ptvirtualize

Comme le montre la capture d'écran, ci-dessous, vous obtiendrez l'affichage de tous les modules disponibles en vertu de cet outil.::


 kevell@Corp:/# ptvirtualize
 ******************************
 Pharaoh Tools - Virtualize
 ******************************


 Virtualize by Golden Contact Computing
 -------------------

 About:
 -----------------
 Virtualize is for controlling Virtual Machines in Development Environments.

 -------------------------------------------------------------

 Available Commands:
 ---------------------------------------

 AutoSSH - AutoSSH - Use your Papyrus details to automatically SSH or SFTP into your Virtualize box
 Box - Box - Manage Base Boxes for Virtualize
 Destroy - Destroy - Stop a Virtualize Box
 Flirtify - Virtualize Flirtify - Generate a Phalgrantfile
 Halt - Halt - Stop a Virtualize Box
 Invoke - SSH Invocation Functions
 PharaohTools - Pharaoh Tools Provisioner Integration
 Provision - Provision - Stop a Virtualize Box
 Resume - Resume - Stop a Virtualize Box
 SFTP - SFTP Functionality
 Shell - Shell Provisioner Integration
 Status - Status - Stop a Virtualize Box
 SystemDetection - System Detection - Detect the Running Operating System
 Up - Up - Create and Start a Virtualize Box
 Virtualbox - Virtualbox Provider Integration 

 ******************************


Commande Aide
---------------

Il est simple d'utiliser la commande help,


  ptvirtualize ModuleName help

Cette commande vous permet de fonctionnement les modules particuliers, et aussi sur ce que sont les actions qu'il peut effectuer.

La capture d'écran ci-dessous vous explique comment la commande help est utilisée pour expliquer le module AutoSSH.::


    kevell@Corp:/#ptvirtualize AutoSSH help

    ******************************
    Pharaoh Tools - Virtualize
    ******************************


    This command allows you to autoSSH a ptvirtualize box

    AutoSSH, auto-ssh, autossh, ssh, SSH

        - cli
        Open an SSH Cli to your ptvirtualize Box
        example: ptvirtualize auto-ssh cli --yes --guess

        - sftp-put
        SFTP Put a file on to your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-put --yes --guess --source=/path/to/source --target=/path/to/target

        - sftp-get
        SFTP Get a file from your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-get --yes --guess --source=/path/to/source --target=/path/to/target

    ------------------------------
    End Help
    ******************************

brève Exemple
---------------

voyons sur un exemple court au sujet de la ptvirtualize ici.


Créez un répertoire, ou tout simplement utiliser un projet web en cours comme votre nouveau Pharaon projet mkdir /var/ www/my-test-project && cd /var/ www/my-test-project
installer virtualbox à votre machine si vous ne l'avez pas déjà, c'est simple en utilisant la commande comme suit::

    sudo ptconfigure virtualbox install --yes --guess --with-guest-additions

Ajouter un fichier de Configuration Management pilote automatique ptconfigure par défaut à l'aide de la commande suivante::


    sudo ptconfigure cleofy install-generic-autopilots --yes --guess --template-group=ptvirtualize

flirtify ptvirtualize flirt now --template-group=default-php

install, configure and start the virtual machine ptvirtualize up now




Jouer avec ptvirtualize Modules 
------------------------------------

.. toctree::
   :maxdepth: 3


 fautossh_virtualize
 fbox_virtualize
 fdestroy_virtualize
 fflirtify_virtualize
 fhalt_virtualize
 fpharaohtools_virtualize
 fresume_virtualize
 fsftp_virtualize
 fshell_virtualize
 fstatus_virtualize
 fsystemdetection_virtualize
 fup_virtualize
 fvirtualbox_virtualize





















