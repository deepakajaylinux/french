============
Sudonopass
============

synopsis
---------------

Sudonopass utilisé pour exécuter une commande particulière avec les permissions root. La chose intéressante est que lorsque le sudo de l'utilisation de l'utilisateur pour une commande particulière, le système demande à l'utilisateur le mot de passe actuel usera € ™. Une fois que l'utilisateur d'entrer le mot de passe, la commande se exécute avec les privilèges root. Ce est apte à travailler avec Ubuntu et Cent OS.

Commande Aide
-----------------------

Cette commande d'aide à guider l'utilisateur sur module de sudonopass. Ceci est approprié pour tous les types d'utilisateurs professionnels. La commande d'aide montre une courte liste des commandes intégrées dans le module de sudonopass. La capture d'écran ci-dessous énumère il.

.. code-block:: bash

	kevell@corp:/# ptconfigure SudoNoPass help
	******************************


	 This command allows you to add an entry to the system sudo file that will
	 allow your user to have passwordless sudo. This is required for
	 quite a few of the  builds provided by Golden Contact, as
	 will perform test execution, software installs and more, silently.

	 SudoNoPass, sudonopass, sudo-nopass, sudo-passwordless

        - install
        Installs the sudo without password entry
        example: ptconfigure sudo-nopass install

	------------------------------
	End Help
	******************************

installation
------------------

Utilisez ce module à installer sudonopass sur les paquets de système Ubuntu Linux.

.. code-block:: bash

          ptconfigure sudonopass install

Install sudonopass? (Y / N)

Lorsque l'utilisateur donne entrée, que oui il va installer automatiquement configurer l'accès de passe root pour tout le monde. La capture d'écran suivante expliquer.

.. code-block:: bash

	kevell@corp:/# ptconfigure sudo-nopass install
	Install Sudo w/o Pass for User? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         Sudo NoPass!        *
	*******************************
	Enter User To Install As:
	Kevells
	The following will be written to /etc/sudoers
	Please check if it looks wrong
	You may not be able to use Sudo if it is incorrect!!!
	Kevells ALL=NOPASSWD: ALL
	Is this okay? (Y/N) 
	y
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	SudoNoPass: Success
	------------------------------
	Installer Finished
	******************************

Option
------------

.. cssclass:: table-bordered

 +-------------------------------+--------------+--------------------------------------------------------------+
 | Paramètres                    | option       | sortie                                                       |
 +===============================+==============+==============================================================+
 |Install sudonopass?(Y/N)       | Yes          | Il est sudonopass installer sous ptconfigure                 |
 +-------------------------------+--------------+--------------------------------------------------------------+
 |Install sudonopass?(Y/N)       | No           | Vous finirez|                                                |
 +-------------------------------+--------------+--------------------------------------------------------------+



avantages
------------

* Sudonopass fait en sorte que les privilèges root sont là pour une commande spécifique (ou pour une durée déterminée) et non pour la session 
  complète qui peut entraîner une mauvaise utilisation accidentelle des privilèges root.
* L'utilisateur peut utiliser sudonopass même accorder des privilèges limités à un utilisateur. Ce est utile lorsque l'utilisateur ne veulent 
  pas d'un utilisateur d'avoir le contrôle de tous les pouvoirs profondes tout en faisant un sudonopass.
* Le meilleur avantage est que sudonopass nécessite de usera € ™ propre mot de passe de connexion plutôt que mot de passe root. Cela aide à 
  garder mot de passe root privé et il ne est pas nécessaire de le changer, même quand un utilisateur (sudoer) laisse.
* Ce fichier fournit des informations sur les commandes qui ont été exécutent en utilisant sudo et leur temps d'exécution. Cela permet de garder  l'administrateur race des utilisateurs, même de confiance

