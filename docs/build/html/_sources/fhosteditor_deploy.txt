======================
Host Editor
======================

Synopsis
------------------

Ce module prend en charge pour manipuler l'éditeur de l'hôte virtuel Apache sous ptdeploy. Il peut fonctionner de deux façons. Ils sont ajouter et supprimer. Éditeur de serveur virtuel est un outil de PHP écrit de faire ajout des hôtes virtuels d'apache un jeu d'enfant. Éditeur de serveur virtuel permettra à l'utilisateur d'ajouter, modifier ou supprimer les informations d'hôte virtuel sur le serveur Web de l'utilisateur. Il est commode de travailler avec Ubuntu et cent OS.  Nous allons voir comment l'apache Vhost éditeur peut fonctionner sous ptdeploy.


Commande Aide
-----------------------

Cette commande help guide l'utilisateur pour créer un hosteditor. La commande help pour Hosteditor est illustrée ci-dessous.

.. code-block:: bash

	ptdeploy Hosteditor help

Après les entrées la commande ci-dessus, il commence de fonctionnement pour ajouter un éditeur de l'hôte virtuel. Il catéchèse les fonctions dans les captures d'écran.

.. code-block:: bash

 kevell@corp:/# ptdeploy HostEditor help 

 ****************************** 

  This command is part of Default Modules and handles Host File Management Functions. 

  HostEditor, hosteditor, he, hostEditor 

          - add 
          add a Host File entry 
          example: ptdeploy hosteditor add 
          example: ptdeploy hosteditor add --yes 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1 
              --host-name=dave.com 

          - rm 
          remove a Host File entry 
          example: ptdeploy hosteditor rm 
          example: ptdeploy hosteditor rm --yes 
              --host-ip=127.0.0.1 # guess will ignore this, and remove any entry matching the host name 
              --host-name=dave.com 

 ------------------------------ 
 End Help 
 ****************************** 



Alternative Paramètre
-----------------------------------

Les autres paramètres qui peuvent être définis dans les déclarations sont les suivants :

HostEditor, hosteditor, he, hostEditor 


Add
-------

Ceci facilite l'utilisateur pour créer un hôte de l'éditeur. L'utilisateur peut entrer le fait d'accorder à leur souhait.

.. code-block:: bash

		sudo ptdeploy hosteditor add

Après l'entrée dans la commande ci-dessus, l'utilisateur peut compléter le processus suivant.

.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor add 

 Do you want to add a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 
 
 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          karuna 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block::  bash

 kevell@corp:/# ptdeploy hosteditor add --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 kumar 
 ****************************** 

 1Host Editor Finished 
 ****************************** 




supprimer
--------------

La commande de terminal pour la suppression des hosteditor est rm. Le format général de cette commande est rm. RM supprime un hôte si vous spécifiez un chemin d'accès correct pour elle et si vous n'avez pas, puis il affiche un message d'erreur et passez à l'hôte suivant.

La commande suivante permet de supprimer le serveur virtuel.

.. code-block:: bash
   
		sudo ptdeploy hosteditor rm

La capture d'écran suivante peut expliquer ses fonctions.

.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor rm 

 Do you want to remove a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 

 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          nithin 
 127.0.0.1          kumar 
 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy hosteditor rm --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 nithin 
 ****************************** 
 
 1Host Editor Finished 
 ****************************** 


avantages
---------------

 * Multi utilisateur peut accéder à la fois.
 * L'utilisateur peut ajouter ou supprimer des hôtes.
 * Respect de la casse non.
