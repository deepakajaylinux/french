===============
JArticle
===============

synopsis
-------------

Il gère les détails de jarticle. Cela vous permet d'utiliser un Article sous forme de Module. Joomla propose une très large gamme d'options pour la création de différents types de contenu et à la structuration des il sur votre site Internet.

Dans Joomla, un Article est un morceau de contenu comprenant du texte, éventuellement avec des liens vers d'autres ressources (par exemple, images). Articles sont les unités de base de l'information dans le système de contenu et de niveau inférieur dans la hiérarchie de contenu. Chaque Article est dans une seule catégorie. Une catégorie peut être dans une autre catégorie, ce qui en fait un sous catégorie. Il est également possible d'avoir des Articles non classé. Ces articles existent sans être associés à n'importe quelle catégorie.



Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation du module jarticle. L'utilisateur viendra à connaître le différent façons/format d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.


.. code-block:: bash
        
	jrush  jarticle help


.. code-block:: bash

 kevell@corp:/# jrush  jarticle help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla JArticles (Component, Module or Plugin).

  JArticle, jarticle

        - disable
        Deletes a jarticle
        example: jrush jarticle disable

        - enable
        Enables a jarticle
        example: jrush jarticle enable

        - info
        Display the details of a jarticle
        example: jrush jarticle info


 ------------------------------
 End Help
 ****************************************



Enable
----------------

Lorsque l'utilisateur a besoin permettre à un article donné, le dessous étant donné de commande exécutera le processus d'installation.


.. code-block:: bash
        
	jrush jarticle enable ..config file=”bootstrap file path”

Info
------

Si l'utilisateur a besoin de connaître les informations d'un article. Le dessous étant donné de commande vous aidera à


.. code-block:: bash
        
	jrush jarticle info ..config file=”bootstrap file path”


La représentation picturale de la commande ci-dessus est listée ci-dessous,


.. code-block:: bash

 kevell@corp:/# jrush jarticle info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JArticle ID. To enter title/alias/asset-id use --jarticle-title, --jarticle-alias or --jarticle-asset-id parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JArticle Information:
 -------------------------

 Article ID: 2
 Asset ID: 35
 Alias: about-us
 Title: About Us
 Created By: 825
 Created By Alias: Joomla
 State: 1
 ------------------------------
 JArticle Manage Finished
 ****************************************


Disable
----------------

Lorsque l'utilisateur doit désactiver un article particulier, le dessous étant donné de commande exécutera le processus d'installation.


.. code-block:: bash
        
	jrush jarticle disable ..config file=”bootstrap file path”

Alternative Paramètre
----------------------------

Soit du paramètre alternatif deux peut être utilisé dans la commande-

jarticle, JArticle

eg:  jrush jarticle disable/ jrush JArticle disable                                 




avantages
--------------

* Fournir une méthode facultative pour l'organisation de vos articles 
* Il contient du texte et peut contenir des images et autres types de contenu 
* permet d'obtenir des informations sur un article de manière facile 
* peut activer et désactiver un article en une seule étape

