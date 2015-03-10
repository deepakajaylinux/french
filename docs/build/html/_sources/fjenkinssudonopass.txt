==================
JenkinsSudoNoPass
==================

synopsis
------------

Jenkins est un serveur de build populaire. Jenkins fournit des services d'intégration continue pour le développement logiciel. Jenkinssudonopass tolère l'utilisateur d'adjoindre une entrée dans le fichier sudo système. Cela a mis en place les utilisateurs Jenkins à fonctionner avec des passward. Ceci est approprié pour Ubuntu et
CentOS.

Commande Aide
-----------------------

La commande d'aide à gérer les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de jenkinssudonopass. Les listes de commandes de l'aide sur les autres paramètres de jenkinssudonopass. Il décrit également la syntaxe pour utiliser jenkinssudonopass à Securify. La commande d'aide pour jenkinssudonopass est donnée ci-dessous.

.. code-block:: bash

		ptconfigure Jenkinssudonopass help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu jenkinssudonopass.

.. code-block:: bash

 kevell@corp:/# ptconfigure JenkinsSudoNoPass help
 ******************************


  This command allows you to add an entry to the system sudo file that will
  allow your Jenkins user to have passwordless sudo. This is required for
  quite a few of the Jenkins builds provided by Golden Contact, as Jenkins
  will perform test execution, software installs and more, silently.

  JenkinsSudoNoPass, jenkinssudonopass, jenkins-sudo-nopass, jenkins-sudo-passwordless

        - install
        Installs the Jenkins sudo without password entry
        example: ptconfigure jenkins-sudo-nopass install

 ------------------------------
 End Help
 ******************************



installation
-----------------

Cette commande autorise à installer Jenkins sudo sans saisie de mot de passe. Lorsque l'utilisateur veut installer jenkinssudonopass la commande suivante guide l'utilisateur à installer.

.. code-block:: bash

                ptconfigure Jenkinssudonopass install

Après avoir tapé cette commande, le système demande à l'utilisateur le souhaite. L'autre processus explique l'installation grâce à la capture d'écran.

.. code-block:: bash

 kevell@corp:/# ptconfigure jenkinssudonopass install
 Install Sudo w/o Pass for Jenkins User? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Jenk Sudo Ps        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-2682022801.sh
 chmod 755 /tmp/ptconfigure-temp-script-2682022801.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-2682022801.sh Permissions
 Executing /tmp/ptconfigure-temp-script-2682022801.sh
 The following will be written to /etc/sudoers
 Please check if it looks wrong
 It may break your system if wrong !!!
 jenkins ALL=NOPASSWD: ALL
 Temp File /tmp/ptconfigure-temp-script-2682022801.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JenkinsSudoNoPass: Success
 ------------------------------
 Installer Finished
 ******************************

options
--------------

.. cssclass:: table-bordered


 +-----------------------+-----------------------------------------------------+-------------+------------------------------------------+
 | Paramètres            | Alternative paramètres                              | Option      | Commentaires                             |
 +=======================+=====================================================+=============+==========================================+
 |Install sudo w/o for   | En dépit de jenkinssudonopass, les alternatives     | Y(Yes)      | Si l'utilisateur souhaite procéder le    |
 |Jenkins user? (Y/N)    | suivantes peuvent également être utilisés:          |             | processus d'installation qu'ils peuvent  |
 |                       | JenkinsSudoNoPass , jenkinssudonopass,              |             | entrée comme Y.                          |
 |                       | jenkins-sudo-nopass, jenkins-sudo-passwordless      |             |                                          |
 +-----------------------+-----------------------------------------------------+-------------+------------------------------------------+
 |Install sudo w/o for   | En dépit de jenkinssudonopass, les alternatives     | N(No)       | Si l'utilisateur souhaite quitter le     |
 |Jenkins user? (Y/N)    | suivantes peuvent également être utilisés:          |             | processus d'installation qu'ils peuvent  |
 |                       | JenkinsSudoNoPass , jenkinssudonopass,              |             | entrée comme N.                          |
 |                       | jenkins-sudo-nopass, jenkins-sudo-passwordless|     |             |                                          |
 +-----------------------+-----------------------------------------------------+-------------+------------------------------------------+


avantages
------------

* Open source de processus d'intégration continue.
* Jenkinssudonopass est une automatisation construit.
* Par script construit et de remédier aux problèmes d'erreur humaine, les ordinateurs sont de mieux en mieux à l'exécution de tâches 
  répétitives.
* Jenkinssudonopass besoin de passer du temps sur leurs déploiements
* Polyvalence et la flexibilité.






