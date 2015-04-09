============
Encryption
============

Synopsis
------------

Ce module permet aux utilisateurs de crypter ou décrypter un fichier.

Le cryptage est le processus de codage des messages ou des informations d'une manière telle que seules les parties autorisées peuvent le lire. Le cryptage ne est pas en soi empêcher l'interception, mais nie le contenu du message à l'intercepteur. Dans un schéma de chiffrement, le message ou l'information, dénommé clair, cryptées en utilisant un algorithme de chiffrement, générant texte chiffré qui ne peut être lu si décrypté. Pour des raisons techniques, une méthode de cryptage utilise habituellement une clé pseudo-aléatoire générée par un algorithme. Il est en principe possible de décrypter le message sans posséder la clé, mais, pour un schéma de chiffrement bien conçu, de grandes ressources de calcul et de compétences sont nécessaires. Un destinataire autorisé peut facilement déchiffrer le message avec la clé fournie par l'expéditeur à des destinataires, mais ne pas intercepteurs non autorisées.

Voyons comment utiliser ce module dans chiffrer et déchiffrer un fichier ou d'une chaîne.


Commande Aide
-------------------

La commande d'aide est un manuel d'utilisation brève qui aide les utilisateurs à la manipulation de ce module. Elle spécifie les paramètres alternatifs qui peuvent être utilisés dans la déclaration. Il précise également les fonctions possibles en vertu du présent module de chiffrement, avec la syntaxe pour les utiliser. La commande utilisée pour déclarer option d'aide est indiqué ci-dessous,

.. code-block:: bash

	ptconfigure encryption help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu de chiffrement.

.. code-block:: bash



 kevell@corp:/# ptconfigure encryption help

 ******************************


 This command allows you to encrypt or decrypt a file.  

 Encryption, encrypt  

 - install        
	Encrypts a file or string        
 	example: sudo ptconfigure encryption install --yes --unencrypted-data=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion        
	 --encryption-target-file=/tmp/encrypted --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions=""                
	 --encryption-file-owner="" --encryption-file-group=""                

 - uninstall        
	Decrypts an encrypted file or string        
	example: sudo ptconfigure encryption uninstall --yes --encrypted-data=/tmp/encrypted        
	 --encryption-target-file=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion --encryption-key=/root/.ptconfigure/SSH/key                	 --encryption-file-permissions="" --encryption-file-owner="" --encryption-file-group=""                

 ------------------------------
 End Help
 ******************************



installer
-----------


Cette fonction permet aux utilisateurs de crypter un fichier ou une chaîne en utilisant simplement la commande comme indiqué ci-dessous,

.. code-block:: bash

	 sudo ptconfigure encryption install --yes --unencrypted-data=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion
 	--encryption-target-file=/tmp/encrypted --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions=""                
	 --encryption-file-owner="" --encryption-file-group=""                

Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les domaines suivants dans le format de la syntaxe mentionné ci-dessus,

* Fichier cible de cryptage
* Clé de chiffrement
* Clé SSH
* Autorisation de fichier de chiffrement
* Propriétaire du fichier de chiffrement
* Groupe de fichiers de cryptage


.. code-block:: bash

 kevell@corp# ptconfigure encryption install
 Install Encryption Functionality? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Encryption !        *
 *******************************
 [Pharaoh Logging] Package php5-mcrypt from the Packager Apt is already installed, so not installing
 Enter either a filepath or raw data to encrypt
 /home/kevell/Desktop/test
 Enter output file path:
 /home/kevell/Desktop/tester
 Enter Encryption Key
 123
 Enter permissions for output file (Empty is okay):
 
 Enter Owner for output file (Empty is okay):

 Enter Group for output file (Empty is okay):

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Encryption: Success
 ------------------------------
 Installer Finished
 ******************************

Désinstaller
-----------------

Cette fonction permet aux utilisateurs de déchiffrer un fichier ou d'une chaîne cryptée. Ceci peut être réalisé en utilisant la commande ci-dessous,

.. code-block:: bash

	sudo ptconfigure encryption uninstall --yes --encrypted-data=/tmp/encrypted
	 --encryption-target-file=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion --encryption-key=/root/.ptconfigure/SSH/key                	 --encryption-file-permissions="" --encryption-file-owner="" --encryption-file-group=""                


Pour mettre en œuvre cette fonction, l'utilisateur doit indiquer les domaines suivants dans le format de la syntaxe mentionné ci-dessus,

* Fichier cible de cryptage
* Clé de chiffrement
* Clé SSH
* Autorisation de fichier de chiffrement
* Propriétaire du fichier de chiffrement
* Groupe de fichiers de cryptage


.. code-block:: bash

 kevell@corp:/# ptconfigure encryption uninstall
 Uninstall Encryption Functionality? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Encryption !        *
 *******************************
 [Pharaoh Logging] Package php5-mcrypt from the Packager Apt is already installed, so not installing
 Enter either a filepath or raw data to decrypt
 /home/kevell/Desktop/tester
 Enter output file path:
 /home/kevell/Desktop/testing
 Enter Encryption Key
 123
 Enter permissions for output file (Empty is okay):
 
 Enter Owner for output file (Empty is okay):

 Enter Group for output file (Empty is okay):

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 Encryption: Success
 ------------------------------
 Installer Finished
 ******************************


Autres paramètres
-------------------


Les autres paramètres de ce module, chacun pouvant être utilisés dans la déclaration est,

* Encryption
* encrypt

avantages
---------

* Les paramètres utilisés dans les opérations d'aide et de cryptage et de décryptage de l'ONU ne sont pas sensibles à la casse qui est un 
  avantage supplémentaire alors comparés à d'autres.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce est un mode sécurisé, car seule personne autorisée peut les utiliser.
