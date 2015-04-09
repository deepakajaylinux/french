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


.. code-block:: bash

 kevell@corp:/# ptconfigure java17 install
 Install The Oracle Java JDK 1.7? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):
 /opt
 Creating /tmp/ptconfigure-temp-script-96883431452.sh
 chmod 755 /tmp/ptconfigure-temp-script-96883431452.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-96883431452.sh Permissions
 Executing /tmp/ptconfigure-temp-script-96883431452.sh
 --2015-04-09 16:27:08--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.168, 131.103.20.167
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.168|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 141966331 (135M) [application/zip]
 Saving to: Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢

 100%[====================================================================================================>] 14,19,66,331  110KB/s   in 12m 36s

 2015-04-09 16:39:46 (183 KB/s) - Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢ saved [141966331/141966331]

 Archive:  /tmp/oraclejdk.zip
 6c383e2868bd47e56385921e11ec155ac54faa13
   creating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/
  inflating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz  
 update-alternatives: using /opt/bin/java to provide /usr/bin/java (java) in auto mode
 update-alternatives: using /opt/bin/javac to provide /usr/bin/javac (javac) in auto mode 
 update-alternatives: using /opt/bin/javaws to provide /usr/bin/javaws (javaws) in auto mode
 Temp File /tmp/ptconfigure-temp-script-96883431452.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 Java: Success
 ------------------------------
 Installer Finished
 ******************************


avantages
------------

* Les paramètres utilisés dans les opérations d'aide et d'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Configuration java, javac, javaws peut être fait avec l'aide de la nouvelle version d'oracle.
