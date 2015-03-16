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
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):

 Creating /tmp/ptconfigure-temp-script-37090112192.sh
 chmod 755 /tmp/ptconfigure-temp-script-37090112192.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-37090112192.sh Permissions
 Executing /tmp/ptconfigure-temp-script-37090112192.sh
 --2015-03-16 15:52:21--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.167, 131.103.20.168
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.167|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: unspecified [application/zip]
 Saving to: ‘6c383e2868bd.zip’

    [          <=>                                                                                          ] 2,06,54,011 2.98KB/s   in 12m 14s

 2015-03-16 16:04:59 (27.5 KB/s) - ‘6c383e2868bd.zip’ saved [20654011]

 /tmp/oraclejdk: Scheme missing.
 FINISHED --2015-03-16 16:04:59--
 Total wall clock time: 12m 39s
 Downloaded: 1 files, 20M in 12m 14s (27.5 KB/s)
  End-of-central-directory signature not found.  Either this file is not
  a zipfile, or it constitutes one disk of a multi-part archive.  In the
  latter case the central directory and zipfile comment will be found on
  the last disk(s) of this archive.
 unzip:  cannot find zipfile directory in one of /tmp/oraclejdk.zip or
        /tmp/oraclejdk.zip.zip, and cannot find /tmp/oraclejdk.zip.ZIP, period.
 /tmp/ptconfigure-temp-script-37090112192.sh: 6: cd: can't cd to /tmp/oraclejdk
 mv: cannot stat ‘/tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz’: No such file or directory
 tar: jdk-7u60-linux-x64.tar.gz: Cannot open: No such file or directory
 tar: Error is not recoverable: exiting now
 mkdir: missing operand
 Try 'mkdir --help' for more information.
 cp: missing destination file operand after ‘/tmp/oraclejdk/jdk1.7.0_60/*’
 Try 'cp --help' for more information.
 chmod: missing operand after ‘a+x’
 Try 'chmod --help' for more information.
 update-alternatives: error: alternative path /bin/java doesn't exist
 update-alternatives: error: alternative path /bin/javac doesn't exist
 update-alternatives: error: alternative path /bin/javaws doesn't exist
 update-alternatives: error: alternative /bin/java for java not registered; not setting
 update-alternatives: error: alternative /bin/javac for javac not registered; not setting
 update-alternatives: error: alternative /bin/javaws for javaws not registered; not setting
 Archive:  /tmp/oraclejdk.zip
 Temp File /tmp/ptconfigure-temp-script-37090112192.sh Removed
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
