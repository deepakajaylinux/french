===========
HAProxy
===========


synopsis
-------------

HAProxy est un logiciel gratuit, solution de haute disponibilité open source, fournir l'équilibrage de charge et de proxy pour les protocoles TCP et HTTP basé sur des applications en répartissant les requêtes entre plusieurs serveurs. A la réputation d'être rapide et efficace (en termes de processeur et de la mémoire).

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'un module HAProxy. L'utilisateur viendra à connaître les différentes façons / format à exécuter ce module. Cette commande va guider l'utilisateur final de savoir quand et comment la commande à utiliser. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
	        ptconfigure HAproxy help


La représentation picturale de la commande ci-dessus est listé ci-dessous,

.. code-block:: bash


 kevell@corp:/# ptconfigure HAProxy help

 *******************************************************


  This module provides installs HA Proxy Server

  HAProxy, ha-proxy, haproxy

        - install
        Installs HA Proxy Server
        example: ptconfigure haproxy install

        - configure
        Configure Load Balancing with HA Proxy Server
        example: ptconfigure haproxy configure

 -------------------------------------------------------
 End Help
 ********************************************************

installation
----------------

Nous pouvons installer HAProxy utilisant le gestionnaire de paquets de la distribution. Lorsque l'utilisateur doit installer le module haproxy dans la machine. La commande ci-dessous donnée exécuter le processus d'installation.

.. code-block:: bash
        
	        ptconfigure HAproxy install

La représentation picturale de la commande ci-dessus est listé ci-dessous,

.. code-block:: bash

 
 kevell@corp:/# ptconfigure haproxy install
 Install HA Proxy Server? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         HA Proxy Server!        *
 *******************************
 [Pharaoh Logging] Package haproxy from the Packager Apt is already installed, so not installing
 HA Proxy Init script config file /etc/default/haproxy added
 [Pharaoh Logging] Restarting haproxy service
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:25] : unknown keyword '1' in 'defaults' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:32] : unknown option 'tcp-check'.
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:34] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:35] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:36] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:37] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:38] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:39] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : Error(s) found in configuration file : /etc/haproxy/haproxy.cfg
 [ALERT] 041/154050 (17460) : Fatal errors found in configuration.
 * Restarting haproxy haproxy
   ...fail!
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 HAProxy: Success
 ------------------------------
 Installer Finished
 ******************************



options
--------

.. cssclass:: table-bordered

 +----------------------------+------------------------------+-------------+----------------------------------------------+
 | Paramètres                 | Alternative paramètres       | Option      | Commentaires                                 |
 +============================+==============================+=============+==============================================+
 |ptconfigure HAProxy Install | HAProxy , ha-proxy, haproxy  | Y           | Le système démarre processus d'installation  |
 +----------------------------+------------------------------+-------------+----------------------------------------------+
 |ptconfigure HAProxy Install | HAProxy , ha-proxy, haproxy  | N           | Système arrête processus d'installation|     |
 +----------------------------+------------------------------+-------------+----------------------------------------------+


 

configuration
--------------------

Cette commande permet de configurer l'équilibrage de charge avec le serveur haproxy. Une fois la commande ci-dessous donnée est exécuté, le système vous offre la valeur par défaut pour chaque section, se il ya des changements à faire, l'utilisateur peut fournir les données.

.. code-block:: bash

                ptconfigure HAproxy configure

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,




.. code-block:: bash


 kevell@corp:/# ptconfigure haproxy configure

 *******************************
 *        Pharaoh Tools        *
 *         HA Proxy Server!    *
 *******************************
 
 What is the environment name you want to balance load to? 
 
 PHP Notice:  Undefined index:  in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 102
 PHP Notice:  Undefined index:  in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 102
 PHP Warning:  Invalid argument supplied for foreach() in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 75
 Set non-default value for global_log? Default is 127.0.0.1 local0 notice (Y/N) 

 Set non-default value for global_maxconn? Default is 20000 (Y/N) 

 Set non-default value for global_user? Default is haproxy (Y/N) 

 Set non-default value for global_group? Default is haproxy (Y/N) 

 Set non-default value for defaults_log? Default is global (Y/N) 

 Set non-default value for defaults_mode? Default is http (Y/N) 

 Set non-default value for defaults_option_string? Default is option dontlognull
    option redispatch (Y/N) 

 Set non-default value for defaults_retries? Default is 3 (Y/N) 

 Set non-default value for defaults_timeout_connect? Default is 5000 (Y/N) 

 Set non-default value for defaults_timeout_client? Default is 10000 (Y/N) 

 Set non-default value for defaults_timeout_server? Default is 10000 (Y/N) 

 Set non-default value for listen_appname? Default is appname (Y/N) 

 Set non-default value for listen_ip_port? Default is 0.0.0.0:80 (Y/N) 

 Set non-default value for listen_mode? Default is http (Y/N) 

 Set non-default value for listen_balance? Default is roundrobin (Y/N) 

 Set non-default value for listen_option_string? Default is option httpclose
    option forwardfor (Y/N) 

 Set non-default value for listen_server_string? Default is  (Y/N) 

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 HA Proxy Server: Success
 ------------------------------
 Installer Finished
 ******************************


avantages
--------------

* Toutes les applications accèdent au cluster via une seule adresse IP. La topologie de la grappe masqué derrière HAProxy de base de données.
* Il est possible d'ajouter ou de supprimer des nœuds de base de données sans modifier les applications.
* Une fois le nombre maximum de connexions de base de données ( MySQL ) atteint , files HAProxy nouvelles connexions supplémentaires . Ce est 
  une belle façon de demandes de connexion de base de données d'étranglement et assure une protection contre les surcharges .
