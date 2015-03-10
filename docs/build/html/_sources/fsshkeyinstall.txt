===============
SshKeyInstall
===============

synopsis
----------------

Clé SSH Installer utilisé pour installer la clé ssh pour un nouvel utilisateur. Une authentification est plus sécurisée que l'authentification par mot de passe. Ceci est particulièrement important si le système est visible sur Internet. Avec l'authentification par clé publique, l'entité d'authentification a une clé publique et une clé privée. Chaque clé est un grand nombre de propriétés mathématiques spéciales. Il est adapté avec Ubuntu et CentOS.

Commande Aide
-------------------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le SSHKEY installer le module. Il énumère les alternatives aux paramètres du module Sshkeyinstall. Il décrit également la syntaxe pour l'installation du module Sshkeyinstall. La commande d'aide pour le module Sshkeyinstall est représentée ci-dessous.

.. code-block:: bash
 
		ptconfigure Sshkeyinstall help


La syntaxe pour déclarer la commande d'aide est non sensible à la casse qui est un avantage supplémentaire. Visualiser l'utilisateur sur la commande d'aide en vertu Sshkeyinstall La capture d'écran suivante.

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeyInstall help

 ******************************


  This command allows you to install an SSH Public key for a user

  SshKeyInstall, sshkeyinstall, ssh-key-install

        - public-key
        Add an SSH Public Key to an account
        example: ptconfigure ssh-key-install public-key
        example: ptconfigure ssh-key-install public-key --yes --public-key-data="zzzzz"
        example: ptconfigure ssh-key-install public-key --yes --public-key-file="id_rsa.pub" --user-name=dave

 ------------------------------
 End Help
 ******************************


installation
------------------

L'installation comprend l'installation de Sshkeyinstall nécessaire pour faire l'installation dans une version mise à jour. Ce est un processus manifeste pour installer le module Sshkeyinstall sous ptconfigure Sshkeyinstall en utilisant simplement la commande ci-dessous

.. code-block:: bash

 		ptconfigure  Sshkeyinstall  public-key

Après dynamiser la commande il catéchiser entrée.

 Lorsque l'entrée d'utilisateur comme il sera automatiquement oui installer Sshkeyinstall avec vérification du système. Si pas quitter l'installation. La capture d'écran suivante demonstSshkeyinstallte Sshkeyinstall il.


 options
--------------

.. cssclass:: table-bordered


 +-------------------------------+--------------------------------------------+---------------+------------------------------------------+
 | paramètre                     | Alternative Paramètre                      | Option        | Kommentare                               |
 +===============================+============================================+===============+==========================================+
 |Install Sshkeyinstall?(Y/N)    | Au lieu d'utiliser SshKeyInstall nous      | Y             | Il est installé sous Sshkeyinstall       |
 |                               | pouvons utiliser Sshkeyinstall,            |               | ptconfigure dans  Pharaoh tools          |
 |                               | ssh-key-installer                          |               |                                          |
 +-------------------------------+--------------------------------------------+---------------+------------------------------------------+
 |Install Sshkeyinstall?(Y/N)    | Au lieu d'utiliser SshKeyInstall nous      | N             | La sortie du système d'installation      |
 |                               | pouvons utiliser Sshkeyinstall,            |               |                                          |
 |                               | ssh-key-installer|                         |               |                                          |
 +-------------------------------+--------------------------------------------+---------------+------------------------------------------+


avantages
----------------

* Sshkeyinstall est bien de choses à faire dans Ubuntu et CentOS
* Sshkeyinstall peut hold-up non sensibilité à la casse
* Sshkeyinstall est flexible
* Sshkeyinstall utilisé installer sshkey
* Sshkeyinstall soutient la sécurité
