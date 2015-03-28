=============
SshHarden 
=============



synopsis
----------

Ce module aide à créer et modifier sshhardens. Le durcir ssh facilite les fonctions de sécurité pour les comptes utilisateurs SSH.

Commande Aide
-------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module SSH de durcir. Les listes de commandes de l'aide sur les autres paramètres de SSH durcir. Il décrit également la syntaxe pour utiliser SSH durcir à Securify. La commande d'aide pour durcir SSH est donnée ci-dessous.

.. code-block:: bash

	ptconfigure SshHarden help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu SSH Harden.

.. code-block:: bash

	Kevell@corp:/# ptconfigure SshHarden help
	
	******************************


        This command allows you to modify create or modify sshhardens

	SshHarden, sshharden, ssh-harden

        - securify
        Add some security to your SSH accounts
        example: ptconfigure ssh-harden securify

	------------------------------
	End Help
	******************************


Securify
-----------

La commande utilisée pour le compte securifying utilisateurs SSH via SSH durcir est indiqué ci-dessous:

.. code-block:: bash

	ptconfigure ssh-harden securify

Après avoir saisi la commande comme indiqué ci-dessus l'installation de ssh durcissement commence comme indiqué dans le format tabulaire.

.. cssclass:: table-bordered

 +---------------------------+-------------------------------------------+-----------+---------------------------------------------------+
 | paramètre                 | Alternative Paramètre                     | Option    | Kommentare                                        |
 +===========================+===========================================+===========+===================================================+
 |Install SshHardening?      | peut également être utilisé au lieu de    | Y(Yes)    | Si l'utilisateur veut le processus d'installation |
 |(Y/N)                      | ssh Durcissement Do alternatives          |           | , vous pouvez aller en entrée Y.                  |
 |                           | suivantes: SshHarden, sshharden,          |           |                                                   |
 |                           | ssh-harden.                               |           |                                                   |
 +---------------------------+-------------------------------------------+-----------+---------------------------------------------------+
 |Install Ssh Hardening?     | peut également être utilisé au lieu de    | N(No)     | Si l'utilisateur veut arrêter le processus        |
 |(Y/N)                      | ssh Durcissement Do alternatives          |           | d'installation, vous pouvez entrer en N. Quitter  |
 |                           | suivantes: SshHarden, sshharden,          |           |                                                   |
 |                           | ssh-harden.|                              |           |                                                   |
 +---------------------------+-------------------------------------------+-----------+---------------------------------------------------+


Si l'utilisateur procède à l'installation de SSH qui permet securifying durcir le compte de ssh d'utilisateurs obtient lancé. Bien que le processus d'exécution se produit, la configuration de sshd se modifie qui interdit ssh root login et ainsi que sshd config est modifié qui interdit mot de passe basé connexion ssh. Enfin, il redémarre le service ssh et afficher les résultats de modifications accomplies Chut Harden. La capture d'écran ci-dessous explique le processus mentionné ci-dessus imagée.

.. code-block:: bash


 kevell@corp:/# ptconfigure sshharden securify
 Install Ssh Hardening? (Y/N) 
 y
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
 [Pharaoh Logging] /etc/ssh/sshd_config modified to disallow root ssh login
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
 [Pharaoh Logging] /etc/ssh/sshd_config modified to disallow password based ssh login
 [Pharaoh Logging] Restarting ssh service
 ssh stop/waiting
 ssh start/running, process 12828
 ******************************


 SshHarden Modifications:
 --------------------------------------------

 Ssh Hardening: Success

 ------------------------------
 SshHarden Mods Finished
 ******************************



avantages
------------

* Cette ssh actes durcir comme un activateur qui permet les fonctions de sécurité des comptes utilisateurs SSH.
* Les paramètres utilisés dans l'aide et securifying, les opérations d'installation ne sont pas sensibles à la casse qui est un avantage 
  supplémentaire par rapport à tout autres.
* Ce module permet de modifier ssh durcir config qui interdit racine connexion ssh, mot de passe basé connexion ssh.
