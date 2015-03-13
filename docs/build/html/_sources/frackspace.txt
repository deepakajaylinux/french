============
Rackspace
============

synopsis
-------------

Rackspace offre une haute performance, une infrastructure fiable pour réussir dans le nuage . Il faut , plates-formes riches en fonctionnalités optimisées , et une équipe d'experts pour exécuter des charges de travail .

Rackspace a deux pôles d'activité: - Serveurs de Cloud et serveurs dédiés . Rackspace contribue à la conception , la construction, et l'exploitation des charges de travail à travers les deux environnements en fonction des besoins individuels du client .

Serveurs cloud - Le niveau de service des infrastructures Géré fournit un ensemble de services nécessaires à la mise en place des clients dans le nuage , y compris des conseils d'architecture , assistance à la sécurité , et de l'aide au développement de code ( via les API et SDK ) de base . Le niveau de soutien des opérations Géré fournit tous les services d'infrastructure gérés , plus un support proactif supplémentaire.

Serveurs dédiés - Le niveau de service Managed consiste en un soutien à la demande où les services sont fournis proactives .


Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de Rackspace . L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l' utilisateur final de connaître le but de cette commande . Ci-dessous sont donnés la commande et la capture d'écran de la même. 

.. code-block:: bash


 kevell@corp:/# ptconfigure Rackspace help

 ******************************


    This is an extension provided for Handling Servers on Rackspace.

    Rackspace, rackspace

        - box-add
        Lets you add boxes to Rackspace, and adds them to your papyrusfile
        example: ptconfigure rackspace box-add
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your Rackspace account - Careful - its irreversible
        example: ptconfigure rackspace box-destroy-all --yes --guess

        - save-ssh-key, sshkey, ssh-key
        Will let you save a local ssh key to your Rackspace account, so you can ssh in to your nodes with it
        securely and without a password
        example: ptconfigure rackspace save-ssh-key
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - list
        Will display data about your Rackspace account
        example: ptconfigure rackspace list
        example: ptconfigure rackspace list --yes
                    --guess # use project saved connection details if possible
                    --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys

        - list-containers
        Will display Container data about your Rackspace account
        example: ptconfigure rackspace list-containers
        example: ptconfigure rackspace list-containers --yes
                    --guess # use project saved connection details if possible

        - list-objects
        Will display object of Containers data about your Rackspace account
        example: ptconfigure rackspace list-objects
        example: ptconfigure rackspace list-objects --yes
                    --guess # use project saved connection details if possible

 ------------------------------
 End Help
 ******************************


Box- add
----------------

Cette commande permet d'ajouter des cases à Rackspace , et les ajoute à votre fichier de papyrus . La commande ci-dessous donnée exécuter le processus .

.. code-block:: bash

 ptconfigure rackspace box-add --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box- détruire
-------------------

Cette commande permet de détruire boîte / es dans un environnement pour vous , et de les supprimer à partir du fichier de papyrus . La commande ci-dessous donnée exécuter le processus .

.. code-block:: bash

 ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box- détruire - tout
-----------------------

Cette commande permet de détruire toutes les cases dans votre compte Rackspace . La partie la plus critique est elle est irréversible .

.. code-block:: bash     

 ptconfigure rackspace box-destroy-all --yes --guess

Enregistrez - ssh- clé
------------------------

Cette commande permet d'enregistrer une clé ssh locale à votre compte Rackspace , donc vous pouvez ssh pour vos nœuds avec elle en toute sécurité et sans un mot de passe . Il ya trois paramètres alternative utilisée pour cette commande particulière - ssh- clé , sshkey , ssh- clé. La commande ci-dessous donnée exécuter le processus .

.. code-block:: bash     
	
	ptconfigure rackspace save-ssh-key --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

liste 
---------------------

Cette commande permet de données sur votre compte Rackspace . La commande ci-dessous donnée exécuter le processus .

.. code-block:: bash 
	
	ptconfigure rackspace list
        
.. code-block:: bash 

	ptconfigure rackspace list --yes --guess # use project saved connection details if possible --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys

Liste des conteneurs-
-----------------------

Cette commande permet d' afficher les données de conteneurs sur votre compte Rackspace . La commande ci-dessous donnée exécuter le processus .

.. code-block:: bash 
	
 	ptconfigure rackspace list-containers

.. code-block:: bash 

	ptconfigure rackspace list-containers --yes --guess # use project saved connection details if possible


Liste -objets
---------------------

Cette commande permet d' afficher des données objet Conteneurs sur votre compte Rackspace . La commande ci-dessous donnée exécuter le processus .

.. code-block:: bash 

 	ptconfigure rackspace list-objects

.. code-block:: bash 

	ptconfigure rackspace list-objects --yes --guess # use project saved connection details if possible

Alternative Paramètre
------------------------------       

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande .

Rackspace, rackspace


avantages
--------------

Rackspace offre une solution complète pour les clients exigeants une haute performance , de l'infrastructure construite à cet effet conçu pour bases de données relationnelles soutenus et appuyés par des ingénieurs qui se spécialisent dans les charges de travail MySQL . Rackspace est un service entièrement géré pour les clients qui veulent se concentrer sur le développement de leurs applications et de ne pas se inquiéter à propos de l' infrastructure sous-jacente . Le service offre sur les sauvegardes et les restaurations de la demande , la surveillance intégrée , stockage redondant , l'évolutivité de croître en fonction des besoins de vos applications , et le plein contrôle de votre base de données .
