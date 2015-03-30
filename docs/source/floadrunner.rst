==============
Loadrunner
==============

synopsis
----------

HP LoadRunner est un produit automatisé de performance et de test de l'automatisation de Hewlett-Packard pour les tests application de la charge : examiner le comportement et les performances du système , tout en générant charge réelle . LoadRunner prend en charge divers outils de développement , des technologies et des protocoles de communication . 

Commande Aide
--------------

La commande help guide les utilisateurs au sujet de l'objet et ainsi que sur les options qui sont inclus dans le module de LoadRunner . Il décrit également la syntaxe pour l'installation du module de LoadRunner . La commande d'aide pour loadrunner est représentée ci-dessous .


.. code-block:: bash

	ptconfigure Loadrunner help

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure Loadrunner help 
 ****************************** 


  This command allows you to install HardyCssRegression from a GC Repo. 

  Loadrunner 

        - install 
        Installs the latest GC Repo version of Loadrunner 
        example: ptconfigure Loadrunner install 

 ------------------------------ 
 End Help 
 ******************************   



installation
--------------

La commande utilisée pour l'installation du module de LoadRunner sur le terminal est listé ci-dessous ,

.. code-block:: bash

	ptconfigure loadrunner install 

La représentation picturale de la commande ci-dessus est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure loadrunner install 
 Install Loadrunner? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Loadrunner !         * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-32374780925.sh 
 chmod 755 /tmp/ptconfigure-temp-script-32374780925.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-32374780925.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-32374780925.sh 
 mkdir: cannot create directory â€˜loadrunnerâ€™: File exists 
 Cloning into 'loadrunner'... 
 remote: Counting objects: 1284, done. 
 remote: Total 1284 (delta 0), reused 0 (delta 0), pack-reused 1284 
 Receiving objects: 100% (1284/1284), 5.63 MiB | 21.00 KiB/s, done. 
 Resolving deltas: 100% (592/592), done. 
 Checking connectivity... done. 
 Temp File /tmp/ptconfigure-temp-script-32374780925.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Loadrunner: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


avantages
----------

* Pas besoin de l'installer sur le serveur en cours de test . Il utilise moniteurs indigènes . Ex : Perfmon pour fenêtres ou rstatd démon
  pour Unix
* Utilise ANSI C que le langue1 de programmation par défaut et d'autres langages comme Java et VB .
* Excellent suivi et interface d'analyse où vous pouvez voir les rapports facile à comprendre graphiques colorés et graphiques .
  Prend en charge la plupart des protocols2 .
* Rend correlation3 beaucoup plus facile . Nous allons creuser dans la corrélation par une série de messages plus tard.
* Scénario de Nice GUI généré par un enregistrement en un clic , bien sûr, vous ne devez modifier le script en fonction de vos besoins .
