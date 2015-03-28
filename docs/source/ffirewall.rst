===========
Firewall
===========

synopsis
--------------

Un pare-feu est un système de sécurité réseau qui contrôle le trafic réseau entrant et sortant sur la base d'un ensemble de règles appliquées. Pare-feu existent à la fois en tant que solution de logiciel et un dispositif matériel.

Commande Aide
------------------------

Cette commande d'aide aider l'utilisateur à propos de Ptconfigure. Il guide l'autorisation de l'utilisateur.
L'utilisateur peut faire la modification selon souhait. Image Aide guidera l'utilisateur. Disons visualiser.

.. code-block:: bash

  ptconfigure Firewall help

Est listé ci-dessous la capture d'écran pour la commande ci-dessus,

.. code-block:: bash

 kevell@corp:/# ptconfigure Firewall help
 ******************************
 This command allows you to modify create or modify firewalls

  Firewall, firewall

        - enable
        Enable system firewall
        example: ptconfigure firewall enable

        - disable
        Disable system firewall
        example: ptconfigure firewall disable

        - allow
        Allow a Firewall rule
        example: ptconfigure firewall allow --firewall-rule="ssh/tcp"

        - deny
        Deny a Firewall rule. Allow connection attempts to be ignored and time out.
        example: ptconfigure firewall deny --firewall-rule="ssh/tcp"

        - reject
        Reject a Firewall rule. Terminate connections attempts with an error to the connector.
        example: ptconfigure firewall reject --firewall-rule="ssh/tcp"

        - limit
        Limit a Firewall rule. ufw will deny connections if an IP address has attempted
        to initiate 6 or more connections in the last 30 seconds.
        example: ptconfigure firewall limit --firewall-rule="ssh/tcp"

        - delete
        Delete a Firewall rule.
        example: ptconfigure firewall delete --firewall-rule="ssh/tcp"

        - insert
        Insert a Firewall rule.
        example: ptconfigure firewall insert --firewall-rule="ssh/tcp"

        - reset
        Reset a Firewall rule.
        example: ptconfigure firewall reset --firewall-rule="ssh/tcp"

        - default
        Set default policy, should be allow, deny, or reject
        example: ptconfigure firewall default --policy="deny"

 ------------------------------
 End Help
 ******************************

options
---------

Règles de pare-feu peuvent être personnalisés selon vos besoins, les exigences et les niveaux de menace de sécurité. L'utilisateur peut créer ou désactiver des règles de pare-feu basé sur des conditions telles que:

.. cssclass:: table-bordered

 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 | Paramètres        | Fonction                                      | Commentaire                                                     |
 +===================+===============================================+=================================================================+
 |IP address         | Bloquant une adresse IP ou d'une certaine     |                                                                 |
 |                   | plage d'adresses IP, ce qui vous pensez sont  |                                                                 |
 |                   | des prédateurs                                |                                                                 |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Enable             | Activer le pare-feu du système                | ptconfigure firewall enable                                     |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Disable            | Désactiver le pare-feu du système             | ptconfigure firewall disable                                    |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Allow              | Autoriser règle de pare-feu                   | ptconfigure firewall allow –firewall-rule=”ssh/tcp”             |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Deny               | Autoriser tentative de connexion à être       | ptconfigure firewall deny –firewall-rule=”ssh/tcp”              |
 |                   | ignoré et le temps                            |                                                                 |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Reject             | Terminate tentatives de connexion avec une    | ptconfigure firewall reject –firewall-rule=”ssh/tcp”            |
 |                   | erreur au connecteur                          |                                                                 |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Limit              | Ufw refusera les connexions si une adresse    | ptconfigure firewall limit –firewall-rule=”ssh/tcp”             |
 |                   | IP a initié six ou tenté plus de connexion    |                                                                 |
 |                   | dans les 30 dernières secondes.               |                                                                 |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Delete             | Supprimer une règle de pare-feu               | ptconfigure firewall delete –firewall-rule=”ssh/tcp”            |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Insert             | Insérez une règle de pare-feu                 | ptconfigure firewall insert –firewall-rule=”ssh/tcp”            |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |Reset              | Réinitialiser une règle de pare-feu           | ptconfigure firewall reset –firewall-rule=”ssh/tcp”             |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+
 |default            | La politique par défaut, devrait être allow,  | ptconfigure firewall default – policy=”deny”                    |
 |                   | deny ou rejeter.|                             |                                                                 |
 +-------------------+-----------------------------------------------+-----------------------------------------------------------------+

La représentation picturale de la commande allow, deny , rejet et réinitialisation est listé ci-dessous ,

.. code-block:: bash

 kevell@corp:/# ptconfigure firewall allow --firewall-rule="ssh/tcp"

 Rules updated
 Rules updated (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall deny --firewall-rule="ssh/tcp"


 Skipping adding existing rule
 Skipping adding existing rule (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall reject --firewall-rule="ssh/tcp"

 Rules updated
 Rules updated (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptconfigure firewall reset --firewall-rule="ssh/tcp"

 Resetting all rules to installed defaults. Proceed with operation (y|n)? Backing up 'user.rules' to '/lib/ufw/user.rules.20150324_190113'
 Backing up 'after.rules' to '/etc/ufw/after.rules.20150324_190113'
 Backing up 'after6.rules' to '/etc/ufw/after6.rules.20150324_190113'
 Backing up 'before6.rules' to '/etc/ufw/before6.rules.20150324_190113'
 Backing up 'user6.rules' to '/lib/ufw/user6.rules.20150324_190113'
 Backing up 'before.rules' to '/etc/ufw/before.rules.20150324_190113'
 
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************





avantages
------------

* Le pare-feu empêche les accès non au système via une connexion réseau en identifiant et en empêchant la communication sur les ports risqués.
* Système de communiquer sur de nombreux ports reconnus, et le pare-feu aura tendance à permettre à ces sans demander ou alerter l'utilisateur.
* Les pare-feu peuvent également détecter l'activité «suspecte» de l'extérieur.
* L'utilisateur peut définir leur règle selon leur souhait.

