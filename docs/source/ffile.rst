======
File
======

synopsis
-------------

Fichier est un programme standard pour reconnaître le type de données contenues dans un fichier informatique. Les tentatives de commande de fichier pour classer chaque objet du système de fichiers (par exemple, fichier, un répertoire ou un lien) qui est fourni à elle comme un argument (ce est à dire, d'entrée). Fichier teste chaque argument dans une tentative de le classer. Il existe trois séries de tests, effectués dans cet ordre: tests de système de fichiers, tests des nombres magiques et tests de langues.

Le premier est un test du système de fichiers, qui utilise l'appel système stat pour obtenir des informations de l'inode de l'objet (qui contient des informations sur un fichier).

Les contrôles de second test pour voir se il ya un nombre magique, qui est un nombre intégré à ou près du début de nombreux types de fichiers qui indique le format de fichier (par exemple, le type de fichier).


Dans le cas où les deux premiers tests ne parviennent pas à déterminer le type d'un fichier, les tests de langue sont utilisées pour déterminer si ce est du texte brut (ce est à dire, entièrement composée de caractères lisibles par l'homme), et, si oui, quel type de texte brut , tels que HTML (Hypertext de markup language) ou le code source

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de fichier. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure file help

.. code-block:: bash

 kevell@corp:/# ptconfigure File help
 ******************************


  This command allows you to modify files or check their existence

  File, file

        - create
        Create a new system file
        example: ptconfigure file create --file="somename"

        - delete
        Delete a system file
        example: ptconfigure file delete --file="somename"

        - exists
        Check the existence of a file
        example: ptconfigure file exists --filename="somename"

        - append
        Append a line to a file
        example: ptconfigure file append --filename="somename" --line="a line"

        - should-have-line
        Ensure that a file contains a particular line
        example: ptconfigure file should-have-line --filename="somename" --line="a line"

 ------------------------------
 End Help
 ******************************


créer
------------

Lorsque l'utilisateur a besoin de créer un nouveau fichier du système, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

                ptconfigure file create --file="somename"

Les commandes ci-dessous donnés écraser des fichiers qui existent

.. code-block:: bash
         
	       ptconfigure file create --file="somename” --overwrite-existing

La commande ci-dessous donnée pour écrire les données dans le fichier

.. code-block:: bash
           
		ptconfigure file create –file="somename” --data="things to put in the file" 


.. code-block:: bash

 kevell@corp:/# ptconfigure file create --file="somename"

 [Pharaoh Logging] [File] Creating File somename
 File somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************



effacer
----------

Lorsque l'utilisateur doit supprimer un fichier système, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
		ptconfigure file delete --file="somename"


.. code-block:: bash

 kevell@corp:/# ptconfigure file delete --file="somename"

 [Pharaoh Logging] [File] Deleting File somename
 somename Deleted
 File somename not exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************




existe
-----------

Lorsque l'utilisateur doit vérifier l'existence d'un fichier, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash

		ptconfigure file exists --filename="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure file exists --filename="somename"

 Enter File Path:
 /home/kevells/Desktop/somename
 File /home/kevells/Desktop/somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************



ajouter
------------

Lorsque l'utilisateur a besoin d'ajouter une ligne dans un fichier, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
		ptconfigure file append --filename="somename" --line="a line"

* L'option de ligne - vous pouvez insérer une ligne à ajouter

.. code-block:: bash

 kevell@corp:/# ptconfigure file append --filename="somename" --line="a line"

 Enter File Path:
 /home/kevells/Desktop/somename                             
 Enter the input for append:
 this is for test
 [Pharaoh Logging] [File] Reading File /home/kevells/Desktop/somename
 [Pharaoh Logging] [File] Writing File /home/kevells/Desktop/somename
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************





Devrait-have en ligne
------------------------------

Lorsque l'utilisateur doit se assurer qu'un fichier contient une ligne particulière, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
	
		ptconfigure file should-have-line --filename="somename" --line="a line"

* Option Ligne - Déclaration qui doit être vérifié

Options
-----------                               

.. cssclass:: table-bordered

 +----------------------------+-----------------------------------------------------------------------------+
 | Paramètre                  | Alternative paramètres                                                      |
 +============================+=============================================================================+
 |ptconfigure file help       | Chacun des deux paramètre alternatif peut être utilisé dans le fichier      |
 |                            | commandement, fichier par exemple: ptconfigure fichier d'installation /     |
 |                            | fichier ptconfigure Installer|                                              |
 +----------------------------+-----------------------------------------------------------------------------+


avantages
---------------

* Spécifier un fichier spécialement formaté contenant des tests sensibles à la position; essais défaut sensible à la position et les tests 
  contextuels sera pas être effectuée.
