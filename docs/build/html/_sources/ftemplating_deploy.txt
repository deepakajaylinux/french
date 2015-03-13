==============
Templating
==============


synopsis
---------------

Le gabarit terme lorsqu'il est utilisé dans le contexte de format de fichier ptdeploy se réfère à une caractéristique commune de nombreuses applications logicielles qui définissent un format de fichier non exécutable unique, conçu spécifiquement pour cette application particulière .

Formats de Templating sont ceux dont le dossier indique que le type de fichier est conçu comme un point de départ très élevé à partir duquel créer autre fichiers .

Ces types de fichiers sont généralement installés fichier de template avec de nouvelles valeurs . Il convient de travailler avec Ubuntu et CentOS .

Commande Aide
------------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules de modèle. La commande help répertorie les autres paramètres de templates sous module de ptdeploy . Il décrit également la syntaxe pour détecter la machine de l' utilisateur. La commande d'aide de templates est illustré ci-dessous .

.. code-block:: bash

	ptdeploy templating help


La capture d'écran ci-dessous explique la création de template .


.. code-block:: bash

 kevell@corp:/# ptdeploy templating help
 ******************************


  This command allows you to install a templated file with new values.

  Templating, templating, template

        - install
        Installs a template
        example: ptconfigure template install

 ------------------------------
 End Help
 ******************************


installation
----------------

Dans un contexte de ptdeploy , les templates se réfère à la création d'une image virtuelle unique de la machine en tant que système d'exploitation invité , puis en l'enregistrant comme un outil pour de multiples machines virtuelles en cours d'exécution . La technique est utilisée pour installer à la fois dans la gestion de la virtualisation et le cloud computing , et est commun dans de grands entrepôts de serveur . La commande suivante permet à l'utilisateur d'installer gabarits .

.. code-block:: bash

	ptdeploy templating install

La capture d'écran suivante guide l'utilisateur à installer.


.. code-block:: bash

 kevell@corp:/# ptdeploy templating install

 Install Templating Functionality? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *         Templating !        *
 *******************************
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Templating: Success

 ------------------------------
 Installer Finished
 ******************************



option
------------

.. cssclass:: table-bordered

 +-----------------------------------+-------------------------+----------+--------------------------------------------------+
 | paramètres	       		     | Autres paramètres       | options  | commentaires				     |
 +===================================+=========================+==========+==================================================+
 |Install templating functionality?  | Templating, templating, | Yes	  | Templating peut être installé sous ptdeploy .    |
 |                                   | template                |          |                                                  |
 +-----------------------------------+-------------------------+----------+--------------------------------------------------+
 |Install templating functionality?  | Templating, templating, | No	  | Il peut quitter l'écran			     |
 |                                   | template|               |          |                                                  |
 +-----------------------------------+-------------------------+----------+--------------------------------------------------+



avantages
-----------------

* Modèle de traitement est utilisé dans différents contextes pour différents buts.
* L'objectif spécifique est habituellement subordonnée à l'application logicielle ou le modèle en cours d'utilisation .
* non sensible
* Costumes de travailler avec Ubuntu et CentOS .
* Version mise à jour avec de nouvelles valeurs est possible .
