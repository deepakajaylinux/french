==========
Jetty
==========

Synopsis
-------------

Jetty fournit un serveur Web et le conteneur javax.servlet, plus de soutien pour SPDY, WebSocket, OSGi, JMX, JNDI, JAAS et beaucoup d'autres l'intégration. Ces composants sont open source et disponible pour un usage commercial et distribution.Jetty est utilisé dans une grande variété de projets et de produits, à la fois dans le développement et la production. Jetty peut être facilement intégré dans les appareils, les outils, les cadres, les serveurs d'applications et les clusters.

Jetty est un HTTP basé sur Java (Web) serveur pure et conteneur de servlets Java. Bien que les serveurs Web sont généralement associées à la signification de documents à des personnes, Ponton est maintenant souvent utilisé pour la machine aux communications de la machine, généralement dans des cadres de logiciels plus importants. Jetty est développé comme un projet libre et open source dans le cadre de la Fondation Eclipse. Le serveur Web est utilisé dans des produits tels que Apache ActiveMQ, Alfresco, Apache Geronimo, Apache Maven, Spark Apache, Google App Engine, Eclipse, FUSE, Streaming API et Zimbra de Twitter. Jetty est également le serveur dans les projets open source tels que Lift, Eucalyptus, Red5, Hadoop et I2P. Jetty supporte la dernière API Java Servlet (avec l'appui JSP) ainsi que les protocoles SPDY et WebSocket.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de jetée. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure jetty help

La représentation picturale de la commande ci-dessus est illustré ci-dessous,

.. code-block:: bash

 kevell@corp:/# ptconfigure Jetty help

 ******************************


  This command allows you to install Jetty, the popular Web Server.

  Jetty, jetty

        - install
        Installs Jetty.  
        example: ptconfigure jetty install

 ------------------------------
 End Help
 ******************************


installation
----------------


Cette commande aide à l'installation de la jetée dans le système. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
	        ptconfigure jetty install


Options
-----------                               

.. cssclass:: table-bordered

 
 +-----------------------+----------------------------------------------------+-------------+--------------------------------------+
 | Paramètres            | Alternative paramètres                             | Option      | Commentaires                         |
 +=======================+====================================================+=============+======================================+
 |ptconfigure jetty      | Il ya deux autres paramètres qui peuvent être      | Y(Yes)      | Le système démarre processus         |
 |Install                | utilisés en ligne de commande. Jetty , jetty       |             | d'installation                       |
 |                       | Eg: ptconfigure jetty install ptconfigure          |             |                                      |
 |                       | Jetty install                                      |             |                                      |
 +-----------------------+----------------------------------------------------+-------------+--------------------------------------+
 |ptconfigure jetty      | Il ya deux autres paramètres qui peuvent être      | N(No)       | Système arrête processus             | 
 |Install                | utilisés en ligne de commande. Jetty , jetty       |             | d'installation                       |
 |                       | Eg: ptconfigure jetty install ptconfigure          |             |                                      |
 |                       | Jetty install|                                     |             |                                      |
 +-----------------------+----------------------------------------------------+-------------+--------------------------------------+


avantages
--------------

* Complet et basée sur des normes
* Flexible et extensible
* Faible encombrement
* exportable
* asynchrone
* Enterprise évolutive
* Double sous licence Apache et Eclipse
