========
Invoke
========


synopsis
-------------

Invoquer récupère le fichier SSH particulier de machine de base à la machine virtuelle. En informatique, le protocole de transfert de fichier par SSH (SFTP ou aussi Secure File transfert Protocol) est un protocole réseau qui fournit l'accès aux fichiers, transfert de fichiers et fonctionnalités de gestion de fichiers sur n'importe quel flux de données fiables.


Commande Aide
----------------------


Cette aide de commande afin de déterminer l'utilisation d'invoque module. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.

.. code-block:: bash
        
	ptvirtualize invoke help

Get
--------

Lorsque l'utilisateur doit récupère un fichier dans notre source pour toute autre destination, l'inférieur compte tenu de la commande s'exécutera le processus.


.. code-block:: bash
        
	ptvirtualize invoke get


Le système demande chemin du fichier source et le chemin d'accès du fichier cible.

Il y a une autre option, dans laquelle vous pouvez donner le chemin d'accès source et de destination dans la ligne de commande.


Alternative Paramètre
------------------------------

Il y a deux paramètre alternatif qui peut être utilisé en ligne de commande 

Invoke , invoke.

Eg: ptvirtualize invoke get/ ptvirtualize Invoke get

avantages
--------------

* Cette commande permet d'extractions SSH fichiers ou répertoires.  
* Récupère un fichier ou un répertoire de source à la destination à l'aide de la commande unique


