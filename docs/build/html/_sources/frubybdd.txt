=========
RubyBDD
=========

synopsis
------------------

Ruby comportement Driven Development (BDD) vous donne le meilleur de Test Driven Development, Domain Driven Design, et les techniques de planification axé essai d'acceptation, afin que l'utilisateur peut installer Ruby BDD pour de meilleurs logiciels avec l'auto-documentation, les tests exécutables qui apportent aux utilisateurs et développeurs ensemble avec un langage Php. Il réconforte avec Ubuntu et Cent OS.

Commande Aide
------------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans les modules Ruby BDD. La commande help répertorie les autres paramètres de Ruby Bdd le cadre du module de ptconfigure. Il décrit également la syntaxe pour l'installation de la updation de l'utilisateur. La commande d'aide pour Ruby Bdd est illustré ci-dessous.

.. code-block:: bash

		ptconfigure Ruby Bdd help

La capture d'écran ci-dessous montre l'effort plein de Ruby Bdd.

.. code-block:: bash

 kevell@corp:/# ptconfigure RubyBDD help

 ******************************


  This command allows you to install Ruby RVM.

  RubyBDD, rubybdd, ruby-bdd

        - install
        Installs Ruby BDD Gems
        example: ptconfigure ruby-bdd install

 ------------------------------
 End Help
 ******************************


installation
-------------------

L'installation comprend l'installation de Ruby Bdd nécessaire pour faire l'installation dans une version mise à jour. Ce est un processus manifeste pour installer le module Ruby Bdd sous ptconfigure en utilisant simplement la commande ci-dessous,

.. code-block:: bash

	ptconfigure Ruby Bdd Install

Après dynamiser la commande il catéchiser entrée.

Lorsque l'entrée de l'utilisateur que oui automatiquement installera Ruby Bdd avec la vérification du système. Si pas quitter l'installation. La capture d'écran ci-dessous le démontre.


.. code-block:: bash

 kevell@corp:/# ptconfigure ruby-bdd install

 Install Ruby BDD? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          !Ruby BDD!!        *
 *******************************
 ERROR:  Error installing cucumber:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:1:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/gherkin-2.12.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/gherkin-2.12.2/ext/gherkin_lexer_ar/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package cucumber from the Packager Gem did not execute correctly
 ERROR:  Error installing capybara:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:4:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2/ext/nokogiri/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package capybara from the Packager Gem did not execute correctly
 ERROR:  While executing gem ... (Gem::DependencyError)
     Unable to resolve dependencies: calabash-android requires rubyzip (~> 0.9.9); xamarin-test-cloud requires rubyzip (~> 1.1)
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 [Pharaoh Logging] Adding Package calabash from the Packager Gem did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 RubyBDD: Success
 ------------------------------
 Installer Finished
 ******************************

Option
---------------


.. cssclass:: table-bordered

 +----------------------------+---------------------------------------------+-----------+--------------------------------------------+
 | paramètres                 | paramètre alternatif                        | option    | commentaire                                |
 +============================+=============================================+===========+============================================+
 |Install RubyBdd?(Y/N)       | Au lieu d'utiliser RubyBdd nous pouvons     | Y         | Il va installer RubyBdd sous ptconfigure   |
 |                            | utiliser ruby-bdd, rubybdd                  |           | outils Pharaon                             |
 +----------------------------+---------------------------------------------+-----------+--------------------------------------------+
 |Install RubyBdd?(Y/N)       | Au lieu d'utiliser RubyBdd nous pouvons     | N         | La sortie du système d'installation        |
 |                            | utiliser ruby-bdd, rubybdd|                 |           |                                            |
 +----------------------------+---------------------------------------------+-----------+--------------------------------------------+


avantages
----------------


* Rubybdd est bien de choses à faire dans Ubuntu et CentOS
* Rubybdd soutient non sensibilité à la casse
* Rubybdd est flexible
* Un autre grand avantage d'avoir BDD sont le développement piloté par - l'utilisateur peut mettre à jour en dernière version de rubybdd, et 
  niveau de correctif, rubis.
* Rubybdd utilisé pour l'installation
