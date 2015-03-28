============
SshKeyStore 
============

Synopsis
-------------

SSH ou shell sécurisé, est un protocole crypté utilisé pour administrer et de communiquer avec les serveurs. Lorsque vous travaillez avec un serveur Linux, les chances sont, vous passerez la plupart de votre temps dans une session de terminal connecté à votre serveur via SSH.

clés SSH sont un moyen d'identifier les ordinateurs de confiance, sans impliquer les mots de passe. clés SSH offrent un moyen sécurisé de se connecter à un serveur basé sur Unix Linux et.

Serveur OpenSSH prend en charge différents schémas d'authentification. Les deux plus populaires sont comme suit:

1. l'authentification basée sur les mots de passe
2. La clé publique d'authentification basée. Ce est une méthode de sécurité alternative à l'utilisation des mots de passe. Cette méthode est 
   recommandée sur un VPS, nuage, serveur dédié ou même à domicile.

Dans clé publique méthode basée vous pouvez vous connecter à des hôtes distants et serveur, et transférer des fichiers à eux, sans utiliser vos mots de passe. Ce module vous permet de trouver des informations d'identification pour une clé sur une machine.

Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation de module de sshkeystore. L'utilisateur viendra à savoir sur la manière différente / format à exécuter ce module. Cette commande guide l'utilisateur final de connaître le but de cette commande. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash
        
        ptconfigure sshkeystore help


Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeyStore help
 ******************************

  This command allows you to find credentials for a key on a machine

  SshKeyStore, sshkeystore, ssh-key-store

        - find
        Add an SSH Public Key to an account
        example: ptconfigure ssh-key-store find --key=daveylad
        example: ptconfigure ssh-key-store find --key=daveylad --prefer=user

 ------------------------------
 End Help
 ******************************

trouver
--------

Lorsque l'utilisateur a besoin d'ajouter une clé publique SSH à un compte, la commande ci-dessous donnée exécuter le processus.

.. code-block:: bash
        
	        ptconfigure ssh-key-store find --key=daveylad


.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-key-store find --key=id_rsa
 [Pharaoh Logging] Trying keystore keys
 Enter User home directory:
 /
 [Pharaoh Logging] User key not found at //.ssh/id_rsa
 Enter User home directory:
 /
 [Pharaoh Logging] Other User key not found at //.ssh/id_rsa
 [Pharaoh Logging] Root key found at /root/.ssh/id_rsa
 ******************************


 SshHarden Modifications:
 --------------------------------------------

 Ssh Key Store: Success
 /root/.ssh/id_rsa

 ------------------------------
 SshHarden Mods Finished
 ******************************




Alternative Paramètre
--------------------------------

Il ya deux autres paramètres qui peuvent être utilisés dans la ligne de commande.

SshKeyStore, sshkeystore, ssh-key-store 

Example: ptconfigure sshkeystore help /ptconfigure ssh-key-store help

Avantages
--------------

* La clé SSH privée (la partie qui peut être mot de passe protégé), ne est jamais exposé sur le réseau. Le mot de passe ne est utilisé que pour   décrypter la clé sur la machine locale. Cela signifie que brutale en réseau forçant ne sera pas possible contre le mot de passe.
* La clé privée est maintenue dans un répertoire restreint. Le client SSH ne reconnaîtra pas les clés privées qui ne sont pas conservés dans 
  restreinte répertoires. La clé elle-même doit également avoir autorisations restreintes (lire et écrire ne est disponible que pour le 
  propriétaire). Cela signifie que les autres les utilisateurs du système ne puisse espionner.
* Tout attaquant espoir de casser le mot de passe de clé privée SSH doit déjà avoir accès au système. Cela signifie qu'ils auront déjà
  accès à votre compte d'utilisateur ou le compte root. Si vous êtes dans cette position, le mot de passe peut empêcher l'attaquant de 
  immédiatement connectant à vos autres serveurs. Cela devrait vous donner le temps de créer et de mettre en œuvre une nouvelle paire de clés 
  SSH et supprimer l'accès à partir de la clé compromise.

