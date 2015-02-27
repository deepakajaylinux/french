==========
Git lab
==========

synopsis
------------

GitLab est incroyablement puissante plate-forme de collaboration de code open source, gestionnaire de dépôt git, Issue Tracker et le code examinateur. Il se intègre avec des traqueurs, les services d'intégration continue et a un support Active Directory phénoménale. Il installe redis serveur et fonctions de la bibliothèque aussi. Ce est gérable dans Ubuntu et CentOS.

HelpCommand
------------------------

Aide commande comprend un vaste système d'aide basée sur la console, qui rappelle de pages de manuel dans Ubuntu. Les rubriques d'aide comprennent l'aide pour installer les dépendances, et les bibliothèques Redis serveur. Simple d'écrire les commandes sans arguments.

.. code-block:: bash

		ptconfigure gitlab help

Les captures d'écran suivantes explique clairement ses fonctions.

.. code-block:: bash


 kevell@corp:/# ptconfigure gitlab help
 ******************************


  This command allows you to install a full Git Lab installation on to a server
  The dependencies for GitLab are also installed.

  GitLab, gitlab, git-lab

        - install
        Installs the latest version of GitLab on a system
        example: ptconfigure gitlab install

 ------------------------------
 End Help
 ******************************

installation
---------------------

    L'installation comprend la fourniture ou la connexion aux services nécessaires pour rendre l'équipement installé prêt à fonctionner. Ce est un processus révélé à installer le module de laboratoire git sous Ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

		ptconfigure gitlab install

Après dynamiser la commande il catéchiser entrée.

L'entrée de l'utilisateur que oui il va installer automatiquement gitlab avec la vérification du système. La capture d'écran suivante démontre.

options
----------

.. cssclass:: table-bordered

 +-------------------------+-------------------------------------------+--------------+------------------------------------------+
 | paramètres              | Autres Paramètres                         | options      | commentaires                             |
 +=========================+===========================================+==============+==========================================+
 |Install gitlab?(Y/N)     | Au lieu d'utiliser gitlab nous pouvons    | Y(Yes)       | Il va installer git et un ensemble de    |
 |                         | utiliser Gitlab, gitlab, git-lab          |              | gitlab commune sous ptconfigure.         |
 +-------------------------+-------------------------------------------+--------------+------------------------------------------+
 |Install gitlab?(Y/N)     | Au lieu d'utiliser gitlab nous pouvons    | N(No)        | La sortie du système d'installation      |
 |                         | utiliser Gitlab, gitlab, git-lab|         |              |                                          | 
 +-------------------------+-------------------------------------------+--------------+------------------------------------------+


avantages
----------------

* Gitlab suit le contenu plutôt que sur les fichiers
* Branches sont légers, et la fusion est un processus simple
* Permet un processus de développement plus rationnel déconnecté
* Dépôts sont de plus petite taille et sont stockés dans un seul répertoire .git
* Permet pour les opérations de rassemblement avancées, et l'utilisation de ranger lorsque l'on travaille à travers des sections gênants.
* Développé pour les systèmes Ubuntu, mais existe soutien communautaire pour les autres distributions comme Arch, CentOS, Fedora, Gentoo ou
* Nécessite une version et les composants spécifié pour fonctionner
