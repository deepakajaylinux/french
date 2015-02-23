=======
Jmeter
=======

synopsis
------------

Ce module traite de l'installation du jmeter avec la version mise à jour. JMeter peut être utilisé comme un outil de test unitaire pour les connexions de base de données JDBC, FTP, LDAP, les services Web, JMS, HTTP, les connexions TCP génériques et les processus autochtones OS. Voyons comment ce module permet à l'utilisateur dans l'installation et l'utilisation du Jmeter.

Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module Jmeter. Il énumère les autres paramètres du module de jmeter. Il décrit également la syntaxe pour l'installation du module de jmeter. La commande d'aide pour le module de jmeter est représentée ci-dessous.

.. code-block:: bash

		ptconfigure Jmeter help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu Jmeter.

.. code-block:: bash

 kevell@corp:/# ptconfigure Jmeter help

 ******************************


  This command allows you to update Jmeter.

  Jmeter, jmeter

        - install
        Installs the latest version of Jmeter
        example: ptconfigure jmeter install

 ------------------------------
 End Help
 ******************************


installation
----------------

La commande utilisée pour installer le jmeter dans la machine des utilisateurs est indiqué ci-dessous:

.. code-block:: bash

		ptconfigure jmeter install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered


 +----------------------+-----------------------------------------+-----------+--------------------------------------------------+
 | Paramètres           | Alternative paramètres                  | Option    | Commentaires                                     |
 +======================+=========================================+===========+==================================================+
 |Install Jmeter? (Y/N) | Au lieu de jmeter, nous pouvons         | Y(Yes)    | Si l'utilisateur souhaite procéder le processus  |
 |                      | utiliser Jmeter également.              |           | d'installation qu'ils peuvent entrée comme Y.    |
 +----------------------+-----------------------------------------+-----------+--------------------------------------------------+
 |Install Jmeter? (Y/N) | Au lieu de jmeter, nous pouvons         | N(No)     | Si l'utilisateur souhaite quitter le processus   |
 |                      | utiliser Jmeter également.              |           | d'installation qu'ils peuvent entrée comme N.|   |
 +----------------------+-----------------------------------------+-----------+--------------------------------------------------+


Si l'utilisateur procède à l'installation, au cours du processus d'installation est décrite dans les listes ci-dessous:


* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les paquets qui sont automatiquement installés.
* Liste outs les nouveaux paquets qui installent.
* Détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.
* Lit les listes de paquets et affiche la liste des paquets qui sont déjà installé.


Représente imagée L'écran suivant le processus décrit ci-dessus de l'installation.


.. code-block:: bash



avantages
------------

* Les paramètres utilisés dans l'aide et l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en rapport aux 
  autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce module de volonté installe le Jmeter dans la version mise à jour.
* Si le module existe déjà dans la machine de l'utilisateur, il affiche un message comme il est déjà existant.
* JMeter soutient paramétrage variable affirmations (de validation de réponse), par les cookies de fil, les variables de configuration et une 
  variété derapports.
* Développeurs hors site peuvent facilement étendre JMeter avec plugins personnalisés.

