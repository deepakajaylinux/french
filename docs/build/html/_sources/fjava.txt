=====	
JAVA
=====

synopsis
------------

Ce module aide à l'installation de la version d'Oracle Java JDK 1.7. Il facilite également la configuration java, javac, javaws avec la nouvelle version d'oracle.

Commande Aide
---------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de java. La commande help répertorie les alternatives aux paramètres du module Java. Il décrit également la syntaxe pour l'installation de Java JDK 1.7. La commande d'aide pour le module Java est représentée ci-dessous.

.. code-block:: bash

		ptconfigure Java help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu module de java.

.. code-block:: bash

 kevell@corp:/# ptconfigure java help
 ******************************


 This command allows you to install Java JDK 1.7 .

 Java, java, java17

        - install
        Installs a version of Oracle Java JDK 1.7. It will also configure java,
        javac and javaws to be provided by the new Oracle version.
        example: ptconfigure java17 install

 ------------------------------
 End Help
 ******************************



installation
----------------

Installation de la version java oracle de JDK 1.7 à la machine de l'utilisateur peut être fait en utilisant simplement la commande comme indiqué ci-dessous.

.. code-block:: bash
	
		ptconfigure Java install

Après avoir saisi la commande ci-dessus, le processus suivant se produit comme indiqué dans le format tabulaire.


.. cssclass:: table-bordered


 +----------------------------+------------------------------------------+------------+-----------------------------------------------+
 | Paramètres                 | Alternative paramètres                   | Option     | Commentaires                                  |
 +============================+==========================================+============+===============================================+
 |Install The Oracle Java     | au lieu de Oracle Java JDK 1.7 The       | Y(Yes)     | If the user wish to proceed the installation  |
 |JDK 1.7? (Y/N)              | alternatives can aussi Following be      |            | process they can input as Y.                  |
 |                            | used:Java, java, java17                  |            |                                               |
 +----------------------------+------------------------------------------+------------+-----------------------------------------------+
 |Install The Oracle Java     | au lieu de Oracle Java JDK 1.7 The       | N(No)      | If the user wish to quit the installation     |
 |JDK 1.7? (Y/N)              | alternatives can aussi Following be      |            | process they can input as N.                  |
 |                            | used:Java, java, java17|                 |            |                                               |
 +----------------------------+------------------------------------------+------------+-----------------------------------------------+


avantages
------------

* Les paramètres utilisés dans les opérations d'aide et d'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Configuration java, javac, javaws peut être fait avec l'aide de la nouvelle version d'oracle.
