==========
Process
==========

synopsis
---------

Ce module aide les utilisateurs à la manipulation d'un fonctions de processus nécessaires, et aussi pour tuer un processus. L'utilisateur peut spécifier le processus notamment en fonction de leurs exigences. L'utilisateur peut spécifier le nom du processus, le fichier ou le répertoire soit du local ou sur une machine distante. Voyons, l'utilisation et les méthodes qui en sont responsables.

Commande Aide
--------------

La commande d'aide sert les utilisateurs sur la façon de gérer et de travailler avec le processus selon leurs besoins. Il énumère également les autres paramètres de processus. Il décrit la syntaxe pour tuer un processus, et aussi sur la manière de spécifier le meurtre d'un processus sur la base de leurs besoins. La commande d'aide pour le module de processus est illustré ci-dessous.

.. code-block:: bash

		ptconfigure process help

La capture d'écran ci-dessous, comme indiqué ci-dessous, montre comment tuer un processus, et comment définir tuer un processus.

Comment définir et d'utiliser le processus
-------------------------------------------------

Pour tuer un processus la syntaxe suivante peut être utilisée.

.. code-block:: bash

		ptconfigure process kill

ou

.. code-block:: bash

		ptconfigure process kill --yes --name="selenium" --use-psax # défaut

La syntaxe comme indiqué ci-dessus ressemble à la corde dans le résultat des.

.. code-block:: bash

		ptconfigure process kill --yes --name="selenium" --use-pkill #

La syntaxe comme indiqué ci-dessus est utilisé pour spécifier ou de trouver une chaîne qui doit être tué.

.. code-block:: bash

		ptconfigure process kill --yes
				--guess
				id="1234 # 

La commande comme indiqué ci-dessus volonté tue un processus selon l 'id donné.

.. code-block:: bash

		ptconfigure process kill --yes
			--level #

La commande ci-dessus est utilisé pour tuer un processus selon le niveau spécifié.

.. code-block:: bash

	ptconfigure process kill --yes --guess --name="skype"

La commande ci-dessus est utilisé pour tuer un processus en spécifiant son nom. Représente le travail de tuer un processus La capture d'écran suivante.

Tuer un procédé utilisant un PID
------------------------------------

Si le PID # 3486 est affecté au processus d'lighttpd. Pour tuer le serveur lighttpd, vous devez passer un PID comme suit:

.. code-block:: bash

 # kill 3486

ou

.. code-block:: bash
 
 $ sudo kill 3486

Ce sera fin à un processus avec un PID de 3486.

Comment puis-je vérifier que le processus est allé / tué?
---------------------------------------------------------------

Utilisez la commande ps ou pidof:

.. code-block:: bash
 
 $ ps aux | grep lighttpd
 $ pidof lighttpd

Comment puis-je tuer deux ou plusieurs PID?
--------------------------------------------

La syntaxe est la suivante pour tuer deux ou plusieurs PID, comme l'exige peut être utilisé en une seule commande:

.. code-block:: bash

 kill  pid1 pid2 pid3
 kill -15  pid1 pid2 pid3
 kill -9  pid1 pid2 pid3
 kill  -9 3546 5557 4242

Dites bonjour à tuer tous commande
------------------------------------

Ce est une seule commande Linux. de tuer les processus par nom. Donc pas besoin de trouver les PID en utilisant le «processus pidof" ou "ps aux | grep de processus de la commande. Ne pas utiliser killall commande sur les systèmes d'exploitation Unix. Ce est une commande spécifique à Linux.

La syntaxe est

.. code-block:: bash

 killall Process-Name-Here

Pour tuer le serveur lighttpd, entrez:

.. code-block:: bash
 
 # killall -15 lighttpd

OU
.. code-block:: bash

 # killall -9 lighttpd

Pour tuer le processus navigateur web Firefox, entrez:

.. code-block:: bash

 # killall -9 firefox-bin

Comme je l'ai dit plus tôt, le tuer tous commande sur le système UNIX fait autre chose. Il tue tous les processus et le processus non seulement spécifique. Ne utilisez pas de tuer tous sur le système UNIX.

avantages
------------

* L'utilisateur peut tuer un processus en utilisant différents paramètres selon leurs besoins. Par exemple: en utilisant l'ID, le niveau du 
  processus, il peut être spécifié à tuer.
