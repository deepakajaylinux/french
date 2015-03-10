===========
Host name
===========

synopsis
---------------

Puisque les adresses IP sont plutôt difficiles à retenir (et ne sont pas particulièrement descriptive), l'Internet permet également à l'utilisateur de spécifier un ordinateur par un nom plutôt qu'une chaîne numérique. Toute cette chaîne est connu comme le nom d'hôte de l'ER de comput. Il ya deux options sont disponibles. Montrer et le changement. En utilisant ce module, l'utilisateur peut afficher ou modifier le nom d'hôte.

Commande Aide
-----------------------

Cette commande peut fonctionner sur les objectifs et les commandes disponibles dans le module de nom d'hôte. Il explique également la commande pour modifier hôte module de nom. Avant de modifier le nom d'hôte, l'utilisateur lire cette commande d'aide explique sa fonction.

.. code-block:: bash
         
                ptconfigure hostname help

La capture d'écran suivante peut apporter à l'esprit il.

.. code-block:: bash

 kevell@corp:/# ptconfigure hostname help

 ******************************


  This command allows you to view or modify hostname

  Hostname, hostname

        - change
        Change the system hostname
        example: ptconfigure hostname change --hostname="my-laptop"

        - show
        Show the system hostname
        example: ptconfigure hostname show

 ------------------------------
 End Help
 ******************************



changement
----------------

Les noms d'hôtes sont généralement utilisés dans une capacité administrative et peuvent apparaître dans les listes d'ordinateurs du navigateur, les listes de Active Directory, adresse IP aux résolutions de nom d'hôte, têtes de courriers électroniques, etc. Lorsque l'utilisateur veut changer le nom d'hôte, peut utiliser la commande suivante.

.. code-block:: bash
           
                ptconfigure hostname change –hostname=”kevellcorp”

De la commande ci-dessus le nouveau nom d'hôte peut entrer.

spectacle
-------------------

Ce module est un processus perceptible pour afficher le nom d'hôte sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash
         
                ptconfigure hostname show

Après clé dans la commande, il montre le nom d'hôte.

option
------------
.. cssclass:: table-bordered

 +---------------------------+-------------------------------------+------------+-----------------------------------------------+
 | Paramètres                | Alternative paramètres              | Option     | Commentaires                                  |
 +===========================+=====================================+============+===============================================+
 |ptconfigure hostname       | au lieu de Hostname nous pouvons    | Show       | Système commence à montrer le processus de    |
 |                           | utiliser Hostname,hostname          |            | nom d'hôte sous ptconfigure                   |
 +---------------------------+-------------------------------------+------------+-----------------------------------------------+
 |ptconfigure hostname       | au lieu de Hostname nous pouvons    | Change     | Système commence à changer le processus de    |
 |change –hostname=”Name”    | utiliser Hostname,hostname          |            | nom d'hôte sous ptconfigure|                  |
 +---------------------------+-------------------------------------+------------+-----------------------------------------------+


avantages
-------------

* Les noms d'hôtes peuvent être des noms simples constitués d'un seul mot ou une phrase, ou ils peuvent être structuré.
* Les noms d'hôtes peut être non-sensible.
* Nom d'hôte peut voir et modifié facilement.
