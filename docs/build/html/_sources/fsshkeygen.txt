============
SshKeygen
============


synopsis
----------

Ce est une aide pour générer la valeur de la clé. Ce module est d'avoir deux types de clés. Ils sont dsa, rsa. dsa valeur de bit clé est 1024 et la valeur du bit clé de rsa est plus que 768. Alors seulement il peut fonctionner. Il est à portée de main dans la tâche avec Ubuntu et cent OS.

Commande Aide
-------------

Cette commande d'aide explique à propos de l'installation d'un module particulier. La commande d'aide est facile à utiliser par l'utilisateur final. La commande suivante guidé l'utilisateur de l'installation.

.. code-block:: bash
		
		ptconfigure Sshkeygen  help

Après avoir donné la commande, la commande affiche la liste des options d'aide. Les captures d'écran suivantes donneront effet visuel pour l'utilisation de ce module.

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeygen help
 ******************************


  This command allows you to install an SSH Key Pair.

  SshKeygen, ssh-keygen, sshkeygen

        - install
        Installs a new SSH Key
        example: ptconfigure ssh-keygen install
        example: ptconfigure ssh-keygen install --yes --bits=4096 --type=rsa --path="/home/dave/.ssh/id_rsa" --comment="Daves"

        - uninstall
        Removes an SSH Key
        example: ptconfigure ssh-keygen uninstall

 ------------------------------
 End Help
 ******************************



installation
-------------

Installation ne est pas un processus difficile à installer ce module sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

		ptconfigure sshkeygen install


Après avoir saisi les entrées des clés SSH gen sera installé avec succès. Les captures d'écran suivantes donneront effet visuel pour l'utilisation de ce module.

.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-keygen install
 Install SSH Key Generation? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         sshkeygen!        *
 *******************************
 Enter number of bits for SSH Key (multiple of 1024):
 1024
 Choose Key type (rsa/dsa)
 (0) rsa 
 (1) dsa 
 1
 Enter path to store private key (public key will be same with .pub):
 /root/SSH/abcd
 Plain text comment appended to public key. None is fine
 kevell
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 SshKeygen: Success
 ------------------------------
 Installer Finished
 ******************************



Options
---------


.. cssclass:: table-bordered

 +--------------------------+--------------------------+-------------+------------------------------------------------------------+
 | paramètres               | (Par défaut) annuaire    | Option      | commentaires                                               |
 +==========================+==========================+=============+============================================================+
 |Install Key Generation    | Yes                      |             | Il va installer la génération clé sous ptconfigure         |
 +--------------------------+--------------------------+-------------+------------------------------------------------------------+
 |Install Key Generation    | No                       |             | L'utilisateur dispose d'une sortie.                        |
 +--------------------------+--------------------------+-------------+------------------------------------------------------------+
 |Choose key type           | rsa                      | 0           | Il va installer la génération clé parmi type de clé        |
 |                          |                          |             | sélectionné                                                |
 +--------------------------+--------------------------+-------------+------------------------------------------------------------+
 |Choose key type           | dsa                      | 1           | Il va installer la génération clé parmi type de clé        |
 |                          |                          |             | sélectionné                                                |
 +--------------------------+--------------------------+-------------+------------------------------------------------------------+
 |path                      | /root/ssh/filename       | -           | Il permettra de créer le fichier avec la clé publique et   |
 |                          |                          |             | privée                                                     |
 +--------------------------+--------------------------+-------------+------------------------------------------------------------+
 |Command appended in file  | yes                      |             | L'utilisateur doit ajouter                                 |
 +--------------------------+--------------------------+-------------+------------------------------------------------------------+
 |Command appended in file  | No                       |             | Abandonné par doc|                                         |
 +--------------------------+--------------------------+-------------+------------------------------------------------------------+





avantages
-----------

Nous pouvons travailler à partir endroit éloigné. L'utilisateur doit charger le système de chemin. Génération automatique est possible. Nous pouvons ajouter le fichier lorsque vous avez besoin. Nous pouvons partager les touches sans mot de passe. Non sensible à la casse.
