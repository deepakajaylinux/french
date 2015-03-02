=========
Php SSH
=========

synopsis
-----------

  PhpSSH est devenu encore plus facile à obtenir en place et fonctionne. Ce qui rend beaucoup plus facile de mise à niveau automatique ptconfigure via PhpSSH. Prenant shell distant,
  pour effectuer différentes tâches est une norme, si l'utilisateur possède la machine serveur de multiples dans une infrastructure.

Commande Aide
-----------------------

Dans cette commande d'aide, l'utilisateur sera discute un tel outil qui a été conçu pour éliminer les failles dans les programmes à distance précédentes shell. ptconfigure sujet d'intérêt pour cette commande ne est autre que la vente sécurisé, mieux connu comme phpSSH. La commande de l'aide comme suit

.. code-block:: bash

                ptconfigure PHPSSH help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide sous PHP SSH.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPSSH help
 ******************************


  This command allows you to install the PHP SSH default Module

  PHPSSH, php-ssh, phpssh

        - install
        Installs the PECL PHP SSH Extension.
        example: ptconfigure phpssh install

 ------------------------------
 End Help
 ******************************



installation
---------------------

Ce est un processus de premier plan à installer le module Phpssh sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash
         
                ptconfigure phpssh install

Après avoir saisi la commande ci-dessus, les étapes suivantes sont impliqués au cours du processus d'installation, comme décrit dans le tableau,

.. cssclass:: table-bordered

 +-----------------------+------------------------------------------+-------------+----------------------------------------------------+
 | Paramètre             | Autres paramètres                        | Options     | Commentaires                                       |
 +=======================+==========================================+=============+====================================================+
 |Install PHP SSH? (Y/N) | Au lieu d'utiliser SSH PHP Nous pouvons  | Y(Yes)      | Si l'utilisateur souhaite procéder le processus    |
 |                       | utiliser PHPSSH, phpssh, php-ssh         |             | d'installation qu'ils peuvent entrée comme Y.      |
 +-----------------------+------------------------------------------+-------------+----------------------------------------------------+
 |Install PHP SSH? (Y/N) | Au lieu d'utiliser SSH PHP Nous pouvons  | N(No)       | Si l'utilisateur souhaite quitter le processus     |
 |                       | utiliser PHPSSH, phpssh, php-ssh         |             | d'installation qu'ils peuvent entrée comme N.|     |
 +-----------------------+------------------------------------------+-------------+----------------------------------------------------+



Si l'utilisateur procède à l'installation, au cours du processus d'installation est décrite dans les listes ci-dessous:


* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste outs les paquets supplémentaires qui installent.
* Liste outs les nouveaux paquets qui installent.
* Détails concernant le nombre de fichiers mis à niveau, nouvellement installés, enlevés et non mis à jour.



La capture d'écran ci-dessous représente graphiquement le processus décrit ci-dessus de l'installation.

.. code-block:: bash


 kevell@corp:/# ptconfigure phpssh install
 Install PHP SSH? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP SSH!        *
 *******************************
 
 Creating config file /etc/php5/mods-available/ssh2.ini with new version
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libssh2-1
 The following NEW packages will be installed:
  libssh2-1 libssh2-php
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 91.0 kB of archives.
 After this operation, 389 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-1 amd64 1.4.3-2 [66.3 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-php amd64 0.12-1build1 [24.7 kB]
 Fetched 91.0 kB in 4s (19.8 kB/s)
 Selecting previously unselected package libssh2-1:amd64.
 (Reading database ... 183000 files and directories currently installed.)
 Preparing to unpack .../libssh2-1_1.4.3-2_amd64.deb ...
 Unpacking libssh2-1:amd64 (1.4.3-2) ...
 Selecting previously unselected package libssh2-php.
 Preparing to unpack .../libssh2-php_0.12-1build1_amd64.deb ...
 Unpacking libssh2-php (0.12-1build1) ...
 Setting up libssh2-1:amd64 (1.4.3-2) ...
 Setting up libssh2-php (0.12-1build1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package libssh2-php from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPSSH: Success
 ------------------------------
 Installer Finished
 ******************************		     


avantages
-----------------

* La première et la plus importante est la vie privée de la communication. Cela signifie que la connexion, ce qui fournit un shell de connexion   à distance, doit être crypté pour éviter les écoutes.
* Il doit y avoir un mécanisme pour vérifier si les données envoyés par l'une des parties ne est pas altérée, ou bricolés. En bref, contrôle 
  d'intégrité est nécessaire.
* Identité de fois sur le serveur et le client doit être fournie à l'autre, d'établir une authentification appropriée.
* Chiffrement et d'authentification mécanismes prévus par PhpSSH améliore la sécurité dans une grande mesure.
