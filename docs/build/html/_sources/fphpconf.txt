============
phpconf
============


synopsis
---------

Ce module aide à l'installation et ainsi que la gestion de la configuration de PHP. L'utilisateur peut cadrer leur configuration selon leurs besoins au moment de l'exécution de l'installation.


Commande Aide
-------------

La commande help guide l'utilisateur à travailler avec cette config php. Il précise également la commande utilisée pour l'installation. La commande help liste également les autres paramètres qui peuvent être utilisés. La commande utilisée pour l'aide l'option sous la config php est donnée ci-dessous.

.. code-block:: bash

	ptconfigure PHPConf help

La capture d'écran ci-dessous montre que donnée représentation picturale concernant l'utilisation de l'aide en php config.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  PHPConf, php-configure, php-configuration, php-conf, phpconf

        - install
        Installs a configuration for PHP
        example: ptconfigure phpconf install

 ------------------------------
 End Help
 ******************************


installation
-------------

Installation de la configuration de PHP est plus bénéfique pour les utilisateurs car ils peuvent encadrer la configuration selon leurs besoins. La commande utilisée pour l'installation est donnée ci-dessous:

.. code-block:: bash

		ptconfigure PHPConf install

Après avoir saisi la commande comme indiqué ci-dessus les opérations suivantes se produit, comme indiqué dans la forme de tableaux.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf install
 Install PHP Conf? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Conf!        *
 *******************************
 Set non-default value for user_ini.filename? Default is .user.ini (Y/N)
 y
 What value for user_ini.filename?

 Set non-default value for user_ini.cache_ttl? Default is 300 (Y/N)
 
 Set non-default value for engine? Default is On (Y/N)

 Set non-default value for short_open_tag? Default is On (Y/N)

 Set non-default value for asp_tags? Default is Off (Y/N)

 Set non-default value for precision? Default is 14 (Y/N)

 Set non-default value for y2k_compliance? Default is On (Y/N)

 Set non-default value for output_buffering? Default is 4096 (Y/N)

 Set non-default value for output_handler? Default is  (Y/N)

 Set non-default value for zlib.output_compression? Default is Off (Y/N)

 Set non-default value for zlib.output_compression_level? Default is -1 (Y/N)

 Set non-default value for zlib.output_handler? Default is  (Y/N)

 Set non-default value for implicit_flush? Default is Off (Y/N)

 Set non-default value for unserialize_callback_func? Default is  (Y/N)

 Set non-default value for serialize_precision? Default is 17 (Y/N)

 Set non-default value for allow_call_time_pass_reference? Default is Off (Y/N)

 Set non-default value for safe_mode? Default is Off (Y/N)

 Set non-default value for safe_mode_gid? Default is Off (Y/N)

 Set non-default value for safe_mode_exec_dir? Default is  (Y/N)

 Set non-default value for safe_mode_allowed_env_vars? Default is PHP_ (Y/N)

 Set non-default value for safe_mode_protected_env_vars? Default is LD_LIBRARY_PATH (Y/N)

 Set non-default value for open_basedir? Default is  (Y/N)

 Set non-default value for disable_functions? Default is pcntl_alarm,pcntl_fork,pcntl_waitpid,pcntl_wait,pcntl_wifexited,pcntl_wifstopped,pcntl_wifsignaled,pcntl_wexitstatus,pcntl_wtermsig,pcntl_wstopsig,pcntl_signal,pcntl_signal_dispatch,pcntl_get_last_error,pcntl_strerror,pcntl_sigpr ocmask,pcntl_sigwaitinfo,pcntl_sigtimedwait,pcntl_exec,pcntl_getpriority,pcntl_setpriority, (Y/N)

 Set non-default value for disable_classes? Default is  (Y/N)

 Set non-default value for ignore_user_abort? Default is On (Y/N)

 Set non-default value for realpath_cache_size? Default is 16k (Y/N)

 Set non-default value for realpath_cache_ttl? Default is 120 (Y/N)

 Set non-default value for zend.enable_gc? Default is On (Y/N)

 Set non-default value for expose_php? Default is On (Y/N)

 Set non-default value for max_execution_time? Default is 30 (Y/N)

 Set non-default value for max_input_time? Default is 60 (Y/N)

 Set non-default value for max_input_nesting_level? Default is 64 (Y/N)

 Set non-default value for max_input_vars? Default is 1000 (Y/N)

 Set non-default value for memory_limit? Default is 128M (Y/N)



 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPConf: Success
 ------------------------------
 Installer Finished
 ******************************


Options
--------

.. cssclass:: table-bordered

 +----------------------+-----------------------------------------+-----------+-------------------------------------------------+
 | paramètres           | Autres paramètres                       | requis    | commentaire                                     |
 +======================+=========================================+===========+=================================================+
 |Install PHPConf?      | Au lieu de PHP Conf ces autres noms     | Y(Yes)    | Si l'utilisateur souhaite procéder le processus |
 |(Y/N)                 | peuvent être utilisés: php-configure,   |           | de nstallation qu'ils peuvent entrée comme Y    |
 |                      | php-conf php-configuration, phpconf     |           |                                                 |
 +----------------------+-----------------------------------------+-----------+-------------------------------------------------+
 |Install PHPConf?      | Au lieu de PHP Conf ces autres noms     | N(No)     | Si l'utilisateur souhaite quitter le processus  |
 |(Y/N)                 | peuvent être utilisés:php-configure,    |           | d'installation qu'ils peuvent entrée comme N.   |
 |                      | php-conf php-configuration, phpconf|    |           |                                                 |
 +----------------------+-----------------------------------------+-----------+-------------------------------------------------+


Si l'utilisateur procède le processus d'installation, pendant l'exécution de l'installation, le module spécifie la valeur par défaut de configuration et se enquiert également à l'utilisateur de mentionner les valeurs par défaut, pour la configuration selon leurs besoins. Les spécifications pour la configuration lors de l'installation est listé ci-dessous:

* Rapport user_ini.filename
* Valeur pour user_ini.cache_ttl?
* Valeur pour le moteur.
* Valeur pour short_open_tag.
* Valeur pour asp_tags.
* La valeur de précision.
* Valeur pour y2k_compliance.
* Valeur pour output_buffering.
* Valeur pour output_handler.
* Valeur pour zlib.output_compression.
* Valeur pour zlib.output_compression_level.
* Valeur pour zlib.output_handler.
* Valeur pour implicit_flush.
* Valeur pour unserialize_callback_func.
* La valeur de précision de serialize.
* Valeur pour allow_call_time_pass_reference.
* Valeur pour safe_mode.
* Valeur pour safe_mode_gid.
* Valeur pour safe_mode_exec_dir?
* Valeur pour safe_mode_allowed_env_vars.
* Valeur pour open_basedir.
* Valeur pour désactiver des fonctions.
* Valeur pour disable_classes?
* Valeur pour ignore_user_abort
* Valeur pour realpath_cache_size?
* Valeur pour realpath_cache_ttl.
* Valeur pour zend.enable_gc.
* Valeur pour expose_php.
* Valeur pour max_execution_time.
* Valeur pour max_input_time.
* Valeur pour max_input_nesting_level.
* Valeur pour max_input_vars.
* Valeur pour memory_limits.

Après avoir regardé les valeurs par défaut pour les fonctions de configuration, l'utilisateur peut décider de leurs actions. Se ils sont boisé avec des valeurs par défaut qu'ils peuvent entrée comme N. Se ils ont besoin de spécifier les valeurs de configuration qu'ils peuvent entrée comme Y. La capture d'écran comme le montre ci-dessous explique le processus décrit ci-dessus visuellement.


Avantages
-----------

* Les paramètres utilisés pour définir l'installation et la commande d'aide ne est pas sensible à la casse.
* Les utilisateurs peuvent encadrer les fonctions de configuration au moment de l'exécution de l'installation.
* Il fonctionne bien à la fois sur Cent OS et Windows.
