============
PHPEclipse
============

Synopsis
-------------

PHPEclipse est un ensemble de plug-ins pour le cadre Eclipse qui fournit IDE intégré pour les développeurs PHP. Eclipse et PHPEclipse sont écrit en Java, et se déroulera sur tous les environnements graphiques de bureau. PHPEclipse est un logiciel Open Source, librement disponible sous la licence Common Public.

La plate-forme Eclipse fournit aux utilisateurs un paradigme d'interface utilisateur cohérente. Un IDE de développement de logiciels est une des applications de bureau plus complexes plupart d'entre nous sont susceptibles d'utiliser, et ainsi le temps nécessaire à un développeur pour devenir efficace avec un IDE particulier peut être important. Eclipse ne réduit pas cette fois, mais il ne fournit une approche cohérente de l'interface qui ne doit pas être appris une fois dans le but de développer efficacement avec un large éventail de langues et outils de programmation. Dans le cadre de cette approche, Eclipse fournit une documentation détaillée et des tutoriels sur toute sa fonctionnalité générique, permettant aux projets de plugins, comme PHPEclipse, se concentrer uniquement sur leurs domaines spécifiques à leur domaine. En apprenant à utiliser Eclipse comme une plate-forme de développement, ou d'apprendre à développer vos propres outils de plug-in pour Eclipse, vous acquérez une compétence utile et flexible.

Commande Aide
--------------

Cette commande permet de déterminer l'utilisation d'un module PHPEclipse. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure PHPeclipse help

La représentation picturale de la commande ci-dessus est illustré ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPEclipse help

 ******************************


  This command allows you to update PHPEclipse.

  phpeclipse, PHPEclipse, PHP-Eclipse

        - install
        Installs the latest version of PHPEclipse
        example: ptconfigure phpeclipse install

 ------------------------------
 End Help
 ******************************


installation
----------------

Cette commande aide à l'installation de la dernière version de PHPEclipse dans le système. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
	        ptconfigure PHPEclipse install


Options
-----------                               


.. cssclass:: table-bordered

 +-----------------------+----------------------------------------------------+-------------+----------------------------------------------+ 
 | paramaters            | paramètre alternatif                               | Options     | commentaires                                 |
 +=======================+====================================================+=============+==============================================+
 |ptconfigure PHPEclipse | Il ya trois paramètres alternatifs qui peuvent     | Y           | Le système démarre processus d'installation  |
 |Install?(Y/N)          | être utilisés en ligne de commande. PHP-Eclipse,   |             |                                              |
 |                       | PHPEclipse, phpeclipse Par exemple :               |             |                                              |
 |                       | ptconfigure PHPEclipse install,                    |             |                                              |
 |                       | ptconfigure PHP-Eclipse install                    |             |                                              |
 +-----------------------+----------------------------------------------------+-------------+----------------------------------------------+
 |ptconfigure PHPEclipse | Il ya trois paramètres alternatifs qui peuvent     | N           | Système arrête processus d'installation      |
 |Install?(Y/N)          | être utilisés en ligne de commande. PHP-Eclipse,   |             |                                              |
 |                       | PHPEclipse, phpeclipse Par exemple :               |             |                                              |
 |                       | ptconfigure PHPEclipse install,                    |             |                                              |
 |                       | ptconfigure PHP-Eclipse install|                   |             |                                              |
 +-----------------------+----------------------------------------------------+-------------+----------------------------------------------+


avantages
--------------

* PHP, HTML, XML et CSS coloration syntaxique
* La complétion de code
* Web intégré navigateur aperçu
* Commande intégrée des serveurs Apache et MySQL
