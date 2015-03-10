========
Invoke
========


synopsis
-------------

Invoke récupère le fichier SSH particulier de machine de base de machine virtuelle. En informatique, le protocole SSH File Transfer (également de protocole de transfert de fichiers sécurisé, ou SFTP) est un protocole réseau qui fournit l'accès aux fichiers, transfert de fichiers, et des fonctionnalités de gestion de fichiers sur ne importe quel flux de données fiable.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module d'invocation. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure invoke help

obtenir
--------

Lorsque l'utilisateur doit récupère un fichier dans notre source vers une autre destination, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
        
	        ptconfigure invoke get


Le système demande pour le chemin du fichier source et le chemin du fichier cible.

Il est une autre option, dans laquelle vous pouvez donner le chemin source et de destination dans la ligne de commande.


Alternative Paramètre
--------------------------------

Il ya deux paramètres alternative qui peut être utilisé dans la ligne de commande 

Invoke , invoke.

Eg: ptconfigure invoke get/ ptconfigure invoke get

avantages
--------------

* Cette commande permet d'récupère les fichiers SSH ou répertoires.
* Récupère un fichier ou répertoire de la source à la destination en utilisant la commande unique
