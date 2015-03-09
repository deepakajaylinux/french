======
Copy
======

Synopsis
-------------

Copier la commande est entré dans un shell Linux pour copier un fichier d'un endroit à l'autre, peut-être sur un système de fichier différent. Le fichier original reste inchangé, et le nouveau fichier peut avoir le même ou un nom différent. Copier est la commande qui fait une copie de vos fichiers ou répertoires.

Les façons les fichiers sont copiés dans Linux dépendent de votre distribution et système de fichiers. Toutes les versions de Linux pourraient copier des fichiers depuis la ligne de commande. Il ya aussi un certain nombre de gestionnaires de fichiers deux mode texte et graphique qui pourrait être utilisé.

Par exemple, disons que vous avez un fichier nommé picture.jpg dans votre répertoire de travail, et que vous voulez faire une copie de celui-ci a appelé l'image-02.jpg. Vous exécutez la commande et le fichier sera copié. Ici, picture.jpg est la source de la copie et de l'image-02.jpg est la destination. Les deux fichiers existent maintenant dans votre répertoire de travail.

Les fichiers source et de destination peuvent également résider dans des répertoires différents. Par exemple, faire une copie du fichier /home/chuck/pictures/picture.jpg dans le répertoire / home / Chuck / sauvegarde. Le fichier de destination sera également nommé picture.jpg.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de copie. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
        ptconfigure copy help

La représentation picturale de la commande de copie d'écran ci-dessous est,

.. code-block:: bash

 kevell@corp:/# ptconfigure copy help
 ******************************


  This command handles file copying functions.

  Copy, copy

        - put
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure copy put
        example: ptconfigure copy put --yes --source="/tmp/file" --target="/home/user/file"

 ------------------------------
 End Help
 ******************************



mettre
--------

Lorsque l'utilisateur a besoin de copier un fichier dans notre source vers une autre destination, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
        
        ptconfigure copy put


Le système demande pour le chemin du fichier source et le chemin du fichier cible.

.. code-block:: bash


 kevell@corp:/# ptconfigure copy put
 Copy files? (Y/N) 
 Y
 Enter source file path
 /kevell.html
 Enter target file path
 /home/desktop
 [Pharaoh Logging] [Copy] Executing cp -r /kevell.html /home/desktop
 ******************************


 Copy Result: Success
 ------------------------------
 Copy Finished
 ******************************


Il est une autre option, dans laquelle vous pouvez donner le chemin source et de destination dans la ligne de commande.

.. code-block:: bash

 kevell@corp:/# ptconfigure copy put --yes --source="/kevell.html" --target="/opt"
 [Pharaoh Logging] [Copy] Executing cp -r /kevell.html /opt
 ******************************


 Copy Result: Success
 ------------------------------
 Copy Finished
 ******************************



Alternative Paramètre
--------------------------------

Il ya deux paramètres alternative qui peut être utilisé dans la ligne de commande Copy , copy.

Par exemple: ptconfigure copy put/ ptconfigure Copy help


avantages
--------------

* Cette commande permet de faire une copie de vos fichiers ou répertoires.
* Copie d'un fichier ou répertoire de la source à la destination en utilisant la commande unique
* Si vous souhaitez copier un fichier d'un dossier à l'autre avec le même nom, juste le nom du répertoire de destination est assez bon
* Un répertoire (et tout son contenu) peuvent être copiés de la source à la destination avec l'option -r récursive
