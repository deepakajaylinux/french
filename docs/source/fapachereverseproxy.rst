=============================
ApacheReverseProxyModules 
=============================

synopsis
-----------

Ce module vise à installer les fonctions de la bibliothèque. Lors de l'installation des fonctions de la bibliothèque, il va vérifier la disponibilité des fonctions de la bibliothèque déjà existants. Il aide à gérer et configurer les paramètres de l'application. L'utilisateur peut spécifier les valeurs par défaut pour les paramètres d'application.

Commande Aide
----------------

Les guides de la commande d'aide l'utilisateur obtiennent au courant des usages, ainsi que les options et les actions qui peuvent être effectuées. Il énumère les aboutissants des paramètres alternatifs

Le codage de faire usage de commande d'aide sous Apache Module proxy inverse, est donné comme suit

.. code-block:: bash

	ptconfigure ApacheReverseProxyModules help

la capture d'écran ci-dessous vous donne une représentation imagée d'utilisation de la commande d'aide.

.. code-block:: bash

          Kevell@corp/# ptconfigure ApacheReverseProxyModules help
	  ******************************


	  This command is part of Core and provides you  with a method by which you can configure Application Settings.
	  You can configure default application settings, ie: mysql admin user, host, pass

	  ApacheReverseProxyModules, apache-reverse-proxy-modules, apache-proxy-mods, apacheproxymodules, apache-lb-mods,
	  apache-load-balancer-modules

          - install
	        Installs Load Balancer/Reverse Proxy Apache Modules
        	example: ptconfigure apache-lb-mods install

	  ------------------------------
          End Help
	  ****************************



installation
---------------

Si l'utilisateur souhaite installer le module proxy apache inverse à leur système, ils peuvent saisir la commande ci-dessous,

.. code-block:: bash

		ptconfigure ApacheReverseProxyModules install

Option
---------

.. cssclass:: table-bordered


 +--------------------------+-----------------------------------------------+-----------------+-------------------------------------------+
 | paramètres               | paramètre alternatif                          | requis          | commentaire                               |
 +==========================+===============================================+=================+===========================================+
 |Install ApacheReverse     | au lieu de Reverse Proxy Apache Module the    | Yes             | Si les entrées de l'utilisateur que Y,    |
 |ProxyModules (Y/N)        | user peut utiliser                            |                 | le module proxy inverse Apache sera       |  
 |                          | apache-reverse-proxy-modules,                 |                 | installé.                                 |
 |                          | apache-proxy-mods, apacheproxymodules,        |                 |                                           |
 |                          | apache-lb-mods, apache-load-balancer-modules  |                 |                                           |
 +--------------------------+-----------------------------------------------+-----------------+-------------------------------------------+
 |Install ApacheReverse     | au lieu de Reverse Proxy Apache Module the    | No              | Si les entrées de l'utilisateur que le N, |
 |ProxyModules (Y/N)        | user peut utiliser                            |                 | le processus se arrêter de l'installation |
 |                          | apache-reverse-proxy-modules,                 |                 |                                           |
 |                          | apache-proxy-mods, apacheproxymodules,        |                 |                                           |
 |                          | apache-lb-mods, apache-load-balancer-modules| |                 |                                           |
 +--------------------------+-----------------------------------------------+-----------------+-------------------------------------------+

   

Lors de l'installation des modules proxy inverse, il sera lit la liste des paquets, des informations d'état, construit l'arbre des dépendances. Si tous les paquets sont manquants, les nouveaux paquets seront installés. Explique la capture d'écran ci-dessous volonté le processus d'installation graphique.

.. code-block:: bash


 kevell@corp:/#: ptconfigure ApacheReverseProxyModules install
 Install Apache Rev. Proxy Modules? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Proxy Mods!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libapache2-mod-proxy-html
 0 upgraded, 1 newly installed, 0 to remove and 229 not upgraded.
 Need to get 1,464 B of archives.
 After this operation, 22.5 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libapache2-mod-proxy-html amd64 1:2.4.7-1ubuntu4.1 [1,464 B]
 Fetched 1,464 B in 1s (1,323 B/s)
 Selecting previously unselected package libapache2-mod-proxy-html.
 (Reading database ... 181545 files and directories currently installed.)
 Preparing to unpack .../libapache2-mod-proxy-html_1%3a2.4.7-1ubuntu4.1_amd64.deb ...
 Unpacking libapache2-mod-proxy-html (1:2.4.7-1ubuntu4.1) ...
 Setting up libapache2-mod-proxy-html (1:2.4.7-1ubuntu4.1) ...
 [Pharaoh Logging] Adding Package libapache2-mod-proxy-html from the Packager Apt executed correctly
 [Pharaoh Logging] Package libxml2-dev from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-49127207421.sh
 chmod 755 /tmp/ptconfigure-temp-script-49127207421.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-49127207421.sh Permissions
 Executing /tmp/ptconfigure-temp-script-49127207421.sh
 Considering dependency proxy_balancer for lbmethod_byrequests:
 Considering dependency proxy for proxy_balancer:
 Enabling module proxy.
 Considering dependency alias for proxy_balancer:
 Module alias already enabled
 Considering dependency slotmem_shm for proxy_balancer:
 Enabling module slotmem_shm.
 Enabling module proxy_balancer.
 Enabling module lbmethod_byrequests.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-49127207421.sh Removed
 Creating /tmp/ptconfigure-temp-script-12740464083.sh
 chmod 755 /tmp/ptconfigure-temp-script-12740464083.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-12740464083.sh Permissions
 Executing /tmp/ptconfigure-temp-script-12740464083.sh
 Module proxy already enabled
 Temp File /tmp/ptconfigure-temp-script-12740464083.sh Removed
 Creating /tmp/ptconfigure-temp-script-61839737362.sh
 chmod 755 /tmp/ptconfigure-temp-script-61839737362.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-61839737362.sh Permissions
 Executing /tmp/ptconfigure-temp-script-61839737362.sh
 Considering dependency proxy for proxy_http:
 Module proxy already enabled
 Enabling module proxy_http.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-61839737362.sh Removed
 Creating /tmp/ptconfigure-temp-script-22752304452.sh
 chmod 755 /tmp/ptconfigure-temp-script-22752304452.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-22752304452.sh Permissions
 Executing /tmp/ptconfigure-temp-script-22752304452.sh
 ERROR: Module mod_proxy_http does not exist!
 Temp File /tmp/ptconfigure-temp-script-22752304452.sh Removed
 Creating /tmp/ptconfigure-temp-script-19250932602.sh
 chmod 755 /tmp/ptconfigure-temp-script-19250932602.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-19250932602.sh Permissions
 Executing /tmp/ptconfigure-temp-script-19250932602.sh
 Considering dependency proxy for proxy_ftp:
 Module proxy already enabled
 Enabling module proxy_ftp.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-19250932602.sh Removed
 Creating /tmp/ptconfigure-temp-script-38556602379.sh
 chmod 755 /tmp/ptconfigure-temp-script-38556602379.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-38556602379.sh Permissions
 Executing /tmp/ptconfigure-temp-script-38556602379.sh
 Considering dependency proxy for proxy_connect:
 Module proxy already enabled
 Enabling module proxy_connect.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-38556602379.sh Removed
 Creating /tmp/ptconfigure-temp-script-85272088847.sh
 chmod 755 /tmp/ptconfigure-temp-script-85272088847.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-85272088847.sh Permissions
 Executing /tmp/ptconfigure-temp-script-85272088847.sh
 Considering dependency proxy for proxy_ajp:
 Module proxy already enabled
 Enabling module proxy_ajp.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-85272088847.sh Removed
 Creating /tmp/ptconfigure-temp-script-31029043648.sh
 chmod 755 /tmp/ptconfigure-temp-script-31029043648.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-31029043648.sh Permissions
 Executing /tmp/ptconfigure-temp-script-31029043648.sh
 Considering dependency proxy for proxy_wstunnel:
 Module proxy already enabled
 Enabling module proxy_wstunnel.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-31029043648.sh Removed
 Creating /tmp/ptconfigure-temp-script-2400353229.sh
 chmod 755 /tmp/ptconfigure-temp-script-2400353229.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-2400353229.sh Permissions
 Executing /tmp/ptconfigure-temp-script-2400353229.sh
 Considering dependency proxy for proxy_balancer:
 Module proxy already enabled
 Considering dependency alias for proxy_balancer:
 Module alias already enabled
 Considering dependency slotmem_shm for proxy_balancer:
 Module slotmem_shm already enabled
 Module proxy_balancer already enabled
 Temp File /tmp/ptconfigure-temp-script-2400353229.sh Removed
 Creating /tmp/ptconfigure-temp-script-88564779807.sh
 chmod 755 /tmp/ptconfigure-temp-script-88564779807.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-88564779807.sh Permissions
 Executing /tmp/ptconfigure-temp-script-88564779807.sh
 Enabling module cache.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-88564779807.sh Removed
 Creating /tmp/ptconfigure-temp-script-68936090528.sh
 chmod 755 /tmp/ptconfigure-temp-script-68936090528.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-68936090528.sh Permissions
 Executing /tmp/ptconfigure-temp-script-68936090528.sh
 Enabling module headers.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-68936090528.sh Removed
 [Pharaoh Logging] Restarting apache2 service
 Output of config test was:
 apache2: Syntax error on line 214 of /etc/apache2/apache2.conf: Could not open configuration file /etc/apache2/httpd.conf: No such file or dir ectory.
 Action 'configtest' failed.
 The Apache error log may have more information.
 * Restarting web server apache2
   ...fail!
 * The apache2 configtest failed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 ApacheReverseProxyModules: Success
 ------------------------------
 Installer Finished
 ******************************




Avantages pour les utilisateurs
------------------------------------------

* Il affiche la liste des paquets disponibles, et à son tour installe les paquets manquants et nécessaires.
* Les avants de proxy inverse vers une destination fixe le compte de clients arbitraires.
* Il sera incorpore le contenu qui est hébergée par un serveur dans un site plus grand.
* Il aide à la configuration des paramètres d'applications.
* Il est bien de choses à faire dans Cent OS et ainsi que dans ubuntu.

