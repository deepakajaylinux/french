============
Parallax
============

synopsis
----------

La parallaxe favorise les fonctions multitâches dans la machine de l'utilisateur. Les paramètres pour définir l'installation et de l'aide ne sont pas sensibles à la casse, alors que par rapport à d'autres. Il est plus facile de définir la fonction multi-tâches, soit au moment de l'installation ou au moment de l'exécution du processus d'installation.

Commande Aide
--------------

La commande help guide l'utilisateur à travailler avec cette parallaxe. Il précise également la commande utilisée pour l'installation de la parallaxe et également la syntaxe pour deux types de déclarer l'installation. La commande help liste également les autres paramètres qui peuvent être utilisés. La commande utilisée pour l'aide option sous la parallaxe est donnée ci-dessous.

.. code-block:: bash

	ptconfigure parallax help

L'affichage des résultats après l'entrée de commande d'aide est représenté dans la capture d'écran ci-dessous.

.. code-block:: bash


	kevell@corp:/# ptconfigure Parallax help
	******************************



	This Module lets you execute commands in parallel

        Parallax, parallax

        - cli
        Go through all questions to execute parallel programs
        example: ptconfigure parallax cli
        example: ptconfigure parallax cli --yes --command-1="pwd" --command-2="ls"

        - child
        Unlikely you'll use this, its used by cli to spawn child processes
        example: parallax cli child

	------------------------------
	End Help
	******************************

installation
--------------

Il est plus facile d'aller avec la parallaxe pour l'installation que l'installation peut être définie de deux manières différentes selon les exigences des utilisateurs. Ces deux manières sont définis comme ci-dessous:

* En mentionnant les types de multi-tâches qui sont nécessaires tout en définissant la commande d'installation.
* Ou, en mentionnant les types de tâches lors de l'exécution (Run-time) installation.

La commande utilisée pour spécifier les multi-tâches au moment de la commande d'installation déclarant est indiqué ci-dessous:

.. code-block:: bash

	ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"

Après avoir mentionné cette commande, la parallaxe exécute à la fois des tâches comme spécifié ci-dessus dans une commande et de commande 2. Les deux tâches sont exécutées en parallèle et le résultat sont affichés. La capture d'écran ci-joint est un très bon exemple pour type de déclaration défini ci-dessus.

.. code-block:: bash

	kevell@corp:/# ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"
	Completed task: pwd
	Completed task: who
	******************************


	COMMAND: pwd
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: /home/kevells


	COMMAND: who
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
	kevells   pts/2        2015-01-08 14:11 (:0)
	kevells   pts/1        2015-01-08 16:36 (:0)
	kevells   pts/10       2015-01-08 16:36 (:0)



	-----------------

	In Cli


	******************************




La commande utilisée pour déclarer les tâches multiples au moment de l'exécution est indiqué ci-dessous:

.. code-block:: bash

	ptconfigure parallax cli child

Après avoir saisi la commande ci-dessus le processus suivant se produit:

.. cssclass:: table-bordered

 +-------------------------+------------------------------------------------+-------------+----------------------------------------------+
 | paramaters              | Alternative Paramètre                          | options     | commentaires                                 |
 +=========================+================================================+=============+==============================================+
 |Run Commands in          | Au Lieu De parallaxles solutions suivantes     | Y(Yes)      | Si l'utilisateur souhaite procéder le        |
 |Parallel? (Y/N)          | peuvent également être utilisés: parallax,     |             | processus d'installation qu'ils peuvent      |
 |                         | Parallax                                       |             | entrée comme Y.                              |
 +-------------------------+------------------------------------------------+-------------+----------------------------------------------+
 |Run Commands in          | Au Lieu De parallaxles solutions suivantes     | N(No)       | Si l'utilisateur souhaite quitter le         |
 |Parallel? (Y/N)          | peuvent également être utilisés: parallax,     |             | processus d'installation qu'ils peuvent      |
 |                         | Parallax                                       |             | entrée comme N.|                             |
 +-------------------------+------------------------------------------------+-------------+----------------------------------------------+


Si l'utilisateur souhaite de procéder l'installation, l'utilisateur peut spécifier les tâches multiples selon leurs besoins. Après l'achèvement de la spécification des tâches multiples, si les utilisateurs souhaitent arrêter, ils peuvent se arrêter en entrant simplement pas.

Enfin, les résultats des tâches accomplies ainsi que son statut sont définis à la fin. Les captures d'écran suivantes vous pouvez une représentation graphique concernant le processus mentionné ci-dessus.

.. code-block:: bash

   
	kevell@corp:/# ptconfigure parallax cli child
	
	Run Commands in Parallel? (Y/N) 
	y
	Enter Command to include next. Enter none to end.
	pwd
	Enter Command to include next. Enter none to end.
	who
	Enter Command to include next. Enter none to end.

	Completed task: pwd
	Completed task: who
	******************************


	COMMAND: pwd
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: /home/kevells


	COMMAND: who
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
	kevells   pts/2        2015-01-08 14:11 (:0)
	kevells   pts/1        2015-01-08 16:36 (:0)
	kevells   pts/10       2015-01-08 16:36 (:0)



	-----------------

	In Cli


	******************************



avantages
----------

* L'utilisateur peut définir les tâches parallèles soit en run-temps ou dans un moyen de pré-définis selon leurs besoins.
* Enfin, après l'achèvement de multi-tâches les résultats et le statut des tâches accomplies sont clairement signalés.
* La syntaxe utilisée pour déclarer ne est pas sensible à la casse lors de la comparaison à d'autres ce qui est un avantage supplémentaire.
* Il est bien de choses à faire dans les deux cent Os et aussi bien que sensible à la casse.
