======
Xvfb
======

synopsis
------------

Ce module facilite l'installation du xvfb, qui est connu comme solution populaire de la machine virtuelle. Le module fournit une solution pour le travail dans une machine virtuelle. xvfb connu sous le nom X virtual frame buffer est un serveur d'affichage mise en œuvre du protocole de serveur d'affichage X11. Contrairement à d'autres serveurs d'affichage Xvfb effectue toutes les opérations graphiques en mémoire sans montrer aucune sortie d'écran. Voyons, comment ce module aide à l'installation du xvfb via apt-get.

Commande Aide
--------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de xvfb. Les listes de commande d'aide sur les alternatives aux paramètres du module de xvfb. Il décrit également la syntaxe pour l'installation de module de xvfb La commande d'aide pour le module de xvfb est représentée ci-dessous.

.. code-block:: bash

		ptconfigure Xvfb help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu module de xvfb.

.. code-block:: bash

 kevell@corp:/# ptconfigure Xvfb help
 ******************************


  This command allows you to install Xvfb, the popular Virtual Machine Solution.

  Xvfb, xvfb

        - install
        Installs Xvfb through apt-get
        example: ptconfigure xvfb install

 ------------------------------
 End Help
 ******************************



installation
----------------

La commande utilisée pour installer le xvfb à la machine des utilisateurs est illustré ci-dessous.

.. code-block:: bash

		ptconfigure xvfb install

Après avoir saisi la commande ci-dessus, les opérations suivantes se produit comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +-----------------------+-------------------------------------------------+------------+-------------------------------------------------+
 | paramètres            | autres paramètres                               | Option     | commentaires                                    |
 +=======================+=================================================+============+=================================================+
 |Install Xvfb? (Y/N)    | aulieude Xvfb, xvfb peut également être utilisé | Y(Yes)     | Si l'utilisateur souhaite procéder le processus |
 |                       |                                                 |            | d'installation qu'ils peuvent entrée comme Y.   |
 +-----------------------+-------------------------------------------------+------------+-------------------------------------------------+
 |Install Xvfb? (Y/N)    | aulieude Xvfb, xvfb peut également être utilisé | N(No)      | Si l'utilisateur souhaite quitter le processus  |
 |                       |                                                 |            | d'installation qu'ils peuvent entrée comme N.|  |
 +-----------------------+-------------------------------------------------+------------+-------------------------------------------------+


Si l'utilisateur procède le processus d'installation, pendant l'exécution de l'installation, le processus suivant se produit:

* Lit listes de paquets.
* Construit l'arbre des dépendances.
* Lit les informations d'état.
* Liste des nouveaux paquets installés.
* Nombre de fichiers mis à niveau, nouvellement installés, retirés, pas mis à niveau.

Enfin, le statut sont clairement signalé et en ajoutant package xvfb de l'emballeur Apt sont exécutées correctement. La capture d'écran ci-dessous vous montre sur le processus d'installation xvfb.

Si le module de xvfb existe déjà dans la machine de l'utilisateur, il affichera un message que le paquet xvfb de l'emballeur Apt est déjà installé. La capture d'écran qui suit est un bon exemple pour ceux type de messages.


.. code-block:: bash

 kevell@corp:/# ptconfigure xvfb install
 Install Xvfb? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! Xvfb !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  xvfb
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 747 kB of archives.
 After this operation, 2,191 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main xvfb amd64 2:1.15.1-0ubuntu2.6 [747 kB]
 Fetched 747 kB in 36s (20.6 kB/s)
 Selecting previously unselected package xvfb.
 (Reading database ... 211203 files and directories currently installed.)
 Preparing to unpack .../xvfb_2%3a1.15.1-0ubuntu2.6_amd64.deb ...
 Unpacking xvfb (2:1.15.1-0ubuntu2.6) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xvfb (2:1.15.1-0ubuntu2.6) ...
 [Pharaoh Logging] Adding Package xvfb from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xvfb: Success
 ------------------------------
 Installer Finished
 ******************************





Avantages
-----------

* Les paramètres utilisés pour déclarer commande d'aide, l'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Il est bien de choses à faire à la fois Cent OS et ainsi que dans Ubuntu.
* Si le paquet de xvfb existe déjà dans la machine de l'utilisateur, il ne sera pas écrasements, au lieu de cela, il affiche un message comme il  en existe déjà.

Xvfb est principalement utilisé pour le test:

* Etant donné qu'il part du code avec le serveur X réel, il peut être utilisé pour tester les parties du code qui ne sont pas liées au matériel   spécifique.
* Il peut être utilisé pour tester des clients dans diverses conditions qui nécessiteraient autrement une gamme de matériel différent; par 
  exemple, il peut être
  utilisé pour tester si les clients fonctionnent correctement à des profondeurs ou tailles d'écran qui sont rarement pris en charge par le 
  matériel.
* Contexte fonctionnement de clients. (Le programme de xwd ou un programme similaire pour capturer une capture d'écran peuvent être utilisés 
  pour voir réellement le résultat)
* Programmes de course qui nécessitent un serveur X d'être actif, même quand ils ne l'utilisent pas. (par exemple Clover rapports html)

