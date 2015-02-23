================
JenkinsPlugins
================

Synopsis
-------------

Jenkins est populaire pour construire serveur. Jenins est un outil d'intégration continue source écrit en Java. Jenkins fournit des services d'intégration continue pour le développement logiciel.

Plugins ont été libérés pour Jenkins qui se étendent son utilisation pour des projets écrits dans des langues autres que Java. Les plugins sont disponibles pour l'intégration Jenkins avec la plupart des systèmes de contrôle de version et de grandes bases de données. De nombreux outils de construction sont pris en charge par l'intermédiaire de leurs plugins respectifs. Les plugins peuvent aussi changer la façon dont Jenkins ressemble ou ajouter de nouvelles fonctionnalités. Construit peuvent générer des rapports de test dans différents formats pris en charge par les plugins (soutien JUnit est actuellement livré) et Jenkins peut afficher les rapports et de générer des tendances et de les rendre dans l'interface graphique.

Commande Aide
-----------------

Cette commande permet de déterminer l'utilisation d'un module JenkinsPlugins. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
             
   		ptconfigure JenkinsPlugins help


 kevell@corp:/# ptconfigure JenkinsPlugins help
 ******************************


  This command allows you to install a bunch of plugins that we recommend for
  PHP builds in Jenkins.

  JenkinsPlugins, jenkinsplugins, jenkins-plugins, jenkins-plugs

        - install
        Installs the latest version of Jenkins Plugins for PHP recommended by Golden Contact
        example: ptconfigure jenkins-plugins install

 ------------------------------
 End Help
 ******************************





installation
----------------

  Cette commande vous permet d'installer un tas de plugins que nous recommandons pour PHP construit dans Jenkins. Si l'utilisateur doit installer le module Jenkins dans la machine, la commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
		ptconfigure JenkinsPlugins install


Est listé ci-dessous la capture d'écran de la commande ci-dessus,

.. code-block:: bash

 

 kevell@corp:/# ptconfigure JenkinsPlugins install
 Install Jenkins Plugins? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Jenkns Plgs!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-80223312434.sh
 chmod 755 /tmp/ptconfigure-temp-script-80223312434.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-80223312434.sh Permissions
 Executing /tmp/ptconfigure-temp-script-80223312434.sh
 Cloning into 'jplugins'...
 remote: Counting objects: 39, done.
 remote: Total 39 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (39/39), done.
 Checking connectivity... done.
 chown: invalid user: ‘jenkins’
 jenkins: unrecognized service
 Temp File /tmp/ptconfigure-temp-script-80223312434.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JenkinsPlugins: Success
 ------------------------------
 Installer Finished
 ******************************



options
-----------

.. cssclass:: table-bordered

 +------------------------+----------------------------------------------+-----------+---------------------------------------------------+
 | Paramètres             | Alternative paramètres                       | Option    | Commentaires                                      |
 +========================+==============================================+===========+===================================================+
 |ptconfigure             | Soit des quatre paramètre alternatif peut    | Y(Yes)    | Une fois que l'utilisateur fournit l'option,      |
 |JenkinsPlugins Install  | être utilisé dans la commande -              |           | système démarre processus d'installation          |
 |                        | JenkinsPlugins, jenkinsplugins,              |           |                                                   |
 |                        | jenkins-plugins, jenkins-plugs               |           |                                                   |
 |                        | eg: ptconfigure jenkins-plugins installer    |           |                                                   |
 +------------------------+----------------------------------------------+-----------+---------------------------------------------------+
 |ptconfigure             | Soit des quatre paramètre alternatif peut    | N(No)     | Une fois que l'utilisateur fournit l'option,      |
 |JenkinsPlugins Install  | être utilisé dans la commande -              |           | système arrête processus d'installation           |
 |                        | JenkinsPlugins, jenkinsplugins,              |           |                                                   |
 |                        | jenkins-plugins, jenkins-plugs               |           |                                                   |
 |                        | eg: ptconfigure jenkins-plugins installer|   |           |                                                   |
 +------------------------+----------------------------------------------+-----------+---------------------------------------------------+
                          

avantages
--------------

* Le plugin vous donnera un rapport sur combien chaque plugin sera utilisé dans tous vos travaux. Par conséquent, il analysera l'extension 
  utilisée points de chaque travail.
* Ce plugin vous donne la possibilité d'analyser l'utilisation de vos plugins installés.
* Sensibilité non de cas
* Eh bien-to-do dans Ubuntu et CentOS.

