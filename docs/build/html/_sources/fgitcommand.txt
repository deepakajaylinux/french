===============
GitCommand
===============

synopsis
-------------

Git est un système distribué de contrôle de version libre et open source conçu pour gérer tout de petits à très grands projets avec rapidité et efficacité . 


Commande Aide
---------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de git . Il énumère les autres paramètres du module de git . La commande d'aide pour le module de git est représentée ci-dessous .

.. code-block:: bash

	ptconfigure gitcommand help

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure gitcommand help

 ******************************



  This command handles Git Functionality

  Git, GitCommand, git-command, gitcommand

  - checkout-branch
    checkout a branch
    example: ptconfigure git checkout-branch --branch=*branchname*

  - create-checkout-branch
    checkout a branch, creating a new branch if needed
    example: ptconfigure git create-checkout-branch --branch=*branchname*

  - delete-branch
    delete a branch
    example: ptconfigure git delete-branch --branch=*branchname*
    
  - ensure-branch
    ensure a branch
    example: ptconfigure git ensure-branch --branch=*branchname*
    
  - add
    add new files to a git repository
    example: ptconfigure git add 
	
  - commit
    commit new messages to a git repository
    example: ptconfigure git  commit --message=*some commit message*

  - push
    push to a git repo
    example: ptconfigure git push --branch=*origin yourbranch*
  
  - pull
    pull a git repo
    example: ptconfigure git pull --branch=*origin yourbranch*

 ------------------------------
 End Help
 ******************************


Checkout-branch
-------------------

La commande git checkout vous permet de naviguer entre les branches créées par branche git . Cette commande commander une branche et le processus d'exécution est illustrée ci-dessous ,

.. code-block:: bash

	ptconfigure git checkout-branch --branch=*branchname*

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************



Create-checkout-branch
---------------------------

Le git checkout créer branche vous permet de récupérer une branche , la création d'une nouvelle branche si nécessaire. Le processus d'exécution de cette commande est comme le montre ci-dessous,


.. code-block:: bash

	ptconfigure git create-checkout-branch --branch=*branchname*

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure git create-checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Attempting to create branch karthi
 Switched to a new branch 'karthi'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************


delete-branch
-----------------

Cette commande est utilisée pour supprimer une branche si elle existe . Le processus d'exécution de cette commande est comme ci-dessous ,

.. code-block:: bash

	ptconfigure git delete-branch --branch=*branchname*

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git delete-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell exists, deleting...
 git branch -d mmmm
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


ensure-branch
----------------

Cette commande est utilisée pour assurer une branche existe , sinon crée une nouvelle branche. Le processus d'exécution de cette commande est ci-dessous ,

.. code-block:: bash

	ptconfigure git ensure-branch --branch=*branchname*

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell does not exist, creating...
 Switched to a new branch 'kevell'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Branch karthi already exists, continuing...
 Now in: /opt/ptconfigure-enterprise

 ******************************


 1 : In GitCommand View
 ******************************

Add
------

La commande git add est utilisée pour ajouter de nouveaux fichiers dans le dépôt git . Le processus d'exécution de cette commande est ci-dessous ,

.. code-block:: bash

	ptconfigure git add 

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git add
 
 Enter the file path to add ? (Enter nothing to add all new & modified files in the git repo).
 test1
 [Pharaoh Logging] All new files in the git repository were added
 ******************************


 0 : In GitCommand View
 ******************************

Commit
---------

Cette commande est utilisée pour commettre de nouveaux messages au dépôt git . Le processus d'exécution de cette commande est comme ci-dessous ,

.. code-block:: bash

	ptconfigure git  commit --message=*some commit message*

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git commit

 Enter message to commit:
 testing
 [Pharaoh Logging] Git commit successfully
 ******************************


 0 : In GitCommand View
 ******************************


Push
----------

Cette commande est utilisée pour pousser des fichiers vers le dépôt git . Le processus d'exécution de cette commande se affiche comme ci-dessous ,

.. code-block:: bash

	ptconfigure git push --branch=*origin yourbranch*

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git push

 What branch?
 origin master
 Username for 'https://github.com': muralivel
 Password for 'https://muralivel@github.com': 
 Counting objects: 5, done.
 Delta compression using up to 2 threads.
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (5/5), 394 bytes | 0 bytes/s, done.
 Total 5 (delta 0), reused 0 (delta 0)
 To https://github.com/muralivel/kumar.git
  * [new branch]      master -> master
 [Pharaoh Logging] Git push to branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************


Pull
----------

Cette commande est utilisée pour tirer un dépôt git . Le processus d'exécution de cette commande est comme ci-dessous ,

.. code-block:: bash

	ptconfigure git pull --branch=*origin yourbranch*

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash


 kevell@corp:/# ptconfigure git pull

 What branch?
 origin master
 remote: Counting objects: 3, done.
 remote: Compressing objects: 100% (2/2), done.
 Unpacking objects: 100% (3/3), done.
 remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 From https://github.com/muralivel/kumar
 * branch            master     -> FETCH_HEAD
   4f390f3..c3e9feb  master     -> origin/master
 [Pharaoh Logging] Git pull from branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************



Autres paramètres
--------------------------

Il ya quatre autres paramètres qui peuvent être utilisés dans la ligne de commande .

Git, GitCommand, git-command, gitcommand


avantages
--------------

* Libres et Open Source
* Rapide et petite
* Sauvegarde implicite
* Sécurité
* Pas besoin de matériel puissant
* Branchement facile



