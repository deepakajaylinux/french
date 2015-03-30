nify
=========

Synopsis
------------------

Minify est l'élimination des caractères inutiles à partir du code source. Mini, lorsqu'il est utilisé comme un préfixe, signifie petit. Le but de rapetisser est de rendre le code source "petit" et améliorer les performances.

Le terme rapetisser est souvent associée à des langages interprétés scénarisées, tels que PHP, qui sont déployés et transmis sur Internet. Code qui a été minified en remplaçant pistes d'espaces par un seul espace, par exemple, est plus léger et prend moins de temps pour un navigateur à charger. Rapetisser outils populaires pour le développement Web comprennent Compresseur et ubuntu compilateur. Minify convient de travailler avec Ubuntu et cent OS.

commande Aide
-----------------------

Minify rend le développement de package une brise: Conceptuellement, rapetisser est similaire à la compression. Contrairement code qui a été comprimé, cependant, le code qui a minified peut encore être travaillé avec sans nécessiter l'étape supplémentaire de décompression. Minified code source peut également être utilisé comme une sorte de faux-fuyants, si l'obscurcissement terme peut être distinguée comme une forme de fausse cryptographie tandis qu'un exemple de code minified peut être inversée en utilisant un imprimeur.

La commande d'aide suivant guide l'utilisateur à gérer rapetisser.

.. code-block:: bash

                ptconfigure minify help

Cette capture d'écran montre la commande help utilization

.. code-block:: bash

 kevell@corp:/# ptconfigure minify help

 ******************************


  This command allows you to update Minify.

  Minify, minify

        - install
        Installs the latest version of minify
        example: ptconfigure minify install

 ------------------------------
 End Help
 ******************************
       
installation
------------------

Il fonctionne avec les conventions existantes pour la structure du code, en ajoutant des outils efficaces pour soutenir le cycle de développement de codage. Avec rapetisser, l'élaboration d'un codage devient si facile que ce sera la configuration par défaut de l'utilisateur lorsque l'utilisateur est en train d'écrire une quantité importante de code. Cette commande utilisé pour installer rapetisser est la suivante,

.. code-block:: bash

                ptconfigure minify install

La capture d'écran ci-dessous explique.

.. code-block:: bash


 kevell@corp:/# ptconfigure minify install 
 Install Minify? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Minify!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  libmemcached10 pear-channels php5-xdebug 
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
  java-wrappers libjargs-java 
 Suggested packages: 
  libjargs-java-doc 
 The following NEW packages will be installed: 
  java-wrappers libjargs-java yui-compressor 
 0 upgraded, 3 newly installed, 0 to remove and 34 not upgraded. 
 Need to get 587 kB of archives. 
 After this operation, 776 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main java-wrappers all 0.1.27 [9,908 B] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main libjargs-java all 1.0.0-4 [14.3 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main yui-compressor all 2.4.7-1 [563 kB] 
 Fetched 587 kB in 41s (14.2 kB/s) 
 Selecting previously unselected package java-wrappers. 
 (Reading database ... 362717 files and directories currently installed.) 
 Preparing to unpack .../java-wrappers_0.1.27_all.deb ... 
 Unpacking java-wrappers (0.1.27) ... 
 Selecting previously unselected package libjargs-java. 
 Preparing to unpack .../libjargs-java_1.0.0-4_all.deb ... 
 Unpacking libjargs-java (1.0.0-4) ... 
 Selecting previously unselected package yui-compressor. 
 Preparing to unpack .../yui-compressor_2.4.7-1_all.deb ... 
 Unpacking yui-compressor (2.4.7-1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up java-wrappers (0.1.27) ... 
 Setting up libjargs-java (1.0.0-4) ... 
 Setting up yui-compressor (2.4.7-1) ... 
 [Pharaoh Logging] Adding Package yui-compressor from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Minify: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


option
----------

Minify code source est particulièrement utile pour langages interprétés et transmis déployées sur Internet, car elle réduit la quantité de données qui doit être transféré.

.. cssclass:: table-bordered

 +---------------------------+-------------------------------------------+---------------+----------------------------------------+
 | paramètres                | Alternative Paramètre                     | options       | commentaires                           |
 +===========================+===========================================+===============+========================================+
 |Install minify?(Y/N)       | Au lieu d'utiliser minify nous pouvons    | Y             | il se installe minifysous ptconfigure  |
 |                           | utiliser Minify                           |               |                                        |
 +---------------------------+-------------------------------------------+---------------+----------------------------------------+
 |Install minify?(Y/N)       | Au lieu d'utiliser minify nous pouvons    | N             | La sortie du système d'installation    |
 |                           | utiliser Minify|                          |               |                                        |
 +---------------------------+-------------------------------------------+---------------+----------------------------------------+


avantages
------------

* Minify communique via PHP codage.
* Minify réconforte avec Ubuntu et cent OS.
* Minify soutient non sensibilité à la casse.
* Minify déduit caractères inutiles à partir du code source.
