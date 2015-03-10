========
Logging
========


synopsis
-----------

Ce module de journalisation est utilisé dans le but de connecter un message à la console, et est éventuellement utilisé pour log d'erreur de php. Voyons comment installer et utiliser le journal pour déclarer message et dans le journal d'erreur php.


Commande Aide
--------------------

Les actes de commandement de l'aide que un manuel d'utilisation brève qui mène l'utilisateur sur son utilisation et les méthodologies. Il spécifie les paramètres alternatifs qui peuvent être utilisés dans la déclaration, et un exemple de syntaxe pour définir un journal. La commande utilisée pour déclarer l'option d'aide est donnée ci-dessous:

.. code-block:: bash

		ptdeploy Logging help

La capture d'écran ci-dessous illustre imagée sur le fonctionnement de la commande d'aide.

.. code-block:: bash

 kevells@corp:/# ptdeploy Logging help
 ******************************


  Use this to log a message to the Console, and optionally the php error log.

  Logging, logging

        - log
        Logs a message the console or
        example: ptconfigure logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************


installation
---------------

La commande utilisée pour l'installation de l'enregistrement en vertu ptdeploy est donnée ci-dessous:

.. code-block:: bash

		ptdeploy logging log


Après la saisie, la commande ci-dessus, le processus d'installation est décrite dans la colonne de tableau suivant.

.. cssclass:: table-bordered

 +--------------------------+-----------------------------------------+--------------+------------------------------------------------------+
 | paramètre                | Autres paramètres                       | Option       | commentaires                                         |
 +==========================+=========================================+==============+======================================================+
 |Install Logging ? (Y/N)   | au lieu de Logging nous pouvons         | Y(Yes)       | Si l'utilisateur souhaite procéder le processus      |
 |                          | utiliser, logging                       |              | d'installation qu'ils peuvent entrée comme Y.        |
 +--------------------------+-----------------------------------------+--------------+------------------------------------------------------+
 |Install Logging ? (Y/N)   | au lieu de Logging nous pouvons         | N(No)        | Si l'utilisateur souhaite quitter le processus       |
 |                          | utiliser, logging                       |              | d'installation qu'ils peuvent entrée comme N.|       |
 +--------------------------+-----------------------------------------+--------------+------------------------------------------------------+


Si l'utilisateur procède le processus d'installation, le processus demande aux utilisateurs de spécifier le message du journal en demandant

.. code-block:: bash

	"Enter Log Message"
	
	"Good Morning"


Une fois que l'utilisateur entrée le message, le message du journal de donner fera une apparition à l'écran, comme indiqué:

"Good Morning"

Enfin, l'installation se rempli. La capture d'écran ci-dessous illustre le processus d'installation imagée.

.. code-block:: bash

 kevells@corp:/#  ptdeploy logging log
 Install Logging? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 No Data.

 ------------------------------
 Installer Finished



Comment définir php journal des erreurs
------------------------------------------

La syntaxe pour déclarer le journal log d'erreur de php est indiqué ci-dessous:

.. code-block:: bash

	ptconfigure logging log --php- log --log-message="Here is something logging to the console and error log"

au lieu de

.. code-block:: bash

 	log-message="Here is something logging to the console and error log"


l'utilisateur peut ajouter ne importe quel texte à la partie du message de journal en fonction de leurs exigences.

avantages
-----------

* L'utilisateur peut ajouter leur message de journal fréquemment utilisé pour le journal d'erreur de php.
* Lors de l'installation le journal l'utilisateur peut entrer et d'assurer l'affichage de message de journal.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que dans cent OS.
* Les paramètres utilisés dans la déclaration ne est pas sensible à la casse.
