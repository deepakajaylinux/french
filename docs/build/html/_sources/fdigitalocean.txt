================
DigitalOcean
================


synopsis
------------

Ce module aide les utilisateurs à la manipulation serveurs sur l'océan numérique. Il enveloppe tous les besoins de base des utilisateurs dans le traitement des boîtes sur l'océan numérique.

Les thèmes à venir discute sur la façon d'utiliser ce module, les diverses caractéristiques de l'océan numérique cadre de ce module.

Commande Aide
-------------------

Les actes de commandement de l'aide que un manuel d'utilisation brève. Il décrit à propos de l'objectif majeur de ce module. Il énumère les aboutissants des paramètres alternatifs qui peuvent être utilisés dans les déclarations. En outre, il a souligne également les différentes caractéristiques de l'utilisation de l'océan numérique cadre de ce module avec la syntaxe pour les utiliser. La commande utilisée pour déclarer option d'aide est indiqué ci-dessous,

.. code-block:: bash

		ptconfigure DigitalOcean help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de Digital Ocean.

.. code-block:: bash

 kevell@corp:/# ptconfigure DigitalOcean help
 ******************************


    This is an extension provided for Handling Servers on Digital Ocean.

    DigitalOcean, digitaloceanv1, digital-ocean-v1

        - box-add
        Lets you add boxes to Digital Ocean, and adds them to your papyrusfile
        example: ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" --digital-ocean-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your digital ocean account - Careful - its irreversible
        example: ptconfigure digital-ocean box-destroy-all --yes --guess

        - save-ssh-key
        Will let you save a local ssh key to your Digital Ocean account, so you can ssh in to your nodes
        securely and without a password
        example: ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - list
        Will display data about your digital ocean account
        example: ptconfigure digital-ocean list
        example: ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys

 ------------------------------
 End Help
 ******************************

Caractéristiques de Digital Ocean
----------------------------------

Comme représenté dans la commande d'aide ci-dessus, ce module a des caractéristiques différentes en utilisant l'océan numérique comme indiqué ci-dessous

* Box_Add
* Box_Destroy
* Box_Destroy_All
* Save_ssh_Key
* Liste


Box_Add
------------

Cette fonction vise à ajouter des boîtes à l'océan numérique et à la main les ajouter au fichier de papyrus. Ceci peut être réalisé simplement en utilisant la syntaxe comme indiqué ci-dessous,

.. code-block:: bash

	ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"


Pour mettre en œuvre la commande ci-dessus, l'utilisateur à spécifier les champs suivants dans le format de la syntaxe mentionné ci-dessus.

* Chemin océan numérique ssh-clé
* Nom numérique océan clé ssh_key



Box_Destroy
----------------

Cette fonction vise à détruire les boîtes dans un environnement spécifié et à la main les supprimer à partir du fichier de papyrus. Ceci peut être réalisé simplement en utilisant la syntaxe comme indiqué ci-dessous,

.. code-block:: bash

	ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" 
        --digital-ocean-ssh-key-name="bastion"

Pour mettre en œuvre la commande ci-dessus, l'utilisateur à spécifier les champs suivants dans le format de la syntaxe mentionné ci-dessus.

* Chemin océan numérique ssh-clé
* Nom numérique océan clé ssh_key



Box_Destroy
----------------

Cette fonction vise à détruire les boîtes dans un environnement spécifié et à la main les supprimer à partir du fichier de papyrus. Ceci peut être réalisé simplement en utilisant la syntaxe comme indiqué ci-dessous,

.. code-block:: bash
   
	ptconfigure digital-ocean box-destroy-all --yes --guess


Save_Ssh_key
-------------------

Cette fonctionnalité permet aux utilisateurs d'enregistrer un ssh local à votre océan numérique afin que les utilisateurs peuvent ssh dans leurs noeuds en toute sécurité sans mot de passe. Ceci peut être réalisé en utilisant la commande ci-dessous,

.. code-block:: bash

	ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

Pour mettre en œuvre la commande ci-dessus, l'utilisateur à spécifier les champs suivants dans le format de la syntaxe mentionné ci-dessus.

* Chemin océan numérique ssh-clé
* Nom numérique océan clé ssh_key

liste
-----

Cette fonctionnalité permet aux utilisateurs de lister toutes les données sur leur compte de l'océan numérique. Ceci peut être réalisé simplement en utilisant la commande ci-dessous,
       
.. code-block:: bash

	ptconfigure digital-ocean list

Or

.. code-block:: bash

        ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys


Autres paramètres
----------------------------

Les autres paramètres de ce module, chacun pouvant être utilisés dans la déclaration est,

 DigitalOcean,   digitaloceanv1,   digital-ocean-v1


avantages
-----------

* Les paramètres utilisés déclarant aide et d'autres caractéristiques différentes de apt ne sont pas sensibles à la casse.
* Il est bien de choses à faire dans les deux cents os et ainsi que dans Ubuntu.
* Ce module enveloppe tous les besoins des utilisateurs dans le traitement de l'océan numérique.


