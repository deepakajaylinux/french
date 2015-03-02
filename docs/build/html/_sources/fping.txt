==========
Ping
==========

synopsis
-----------

Comme un verbe, PING signifie «d'attirer l'attention de» ou «pour vérifier la présence d'une« autre partie en ligne. PING (Packet INternet Groper) Module utilisé pour tester la connectivité du système. PING utilisé pour envoyer des données de réseau pour, et recevoir des données de réseau à partir, un autre ordinateur sur un réseau. PING fréquemment utilisé pour tester, si un autre système est accessible sur un réseau, et si oui, combien de temps il faut pour que les données qui doivent être échangées.

Commande Aide
---------------

Cette commande permet de déterminer l'utilisation de module de PING. Cette commande aider à comprendre les options à utiliser avec commande PING. Cette commande va guider l'utilisateur final de connaître l'utilisation de différentes options et la syntaxe de ces options. Ci-dessous sont donnés la commande et la capture d'écran de la même.

.. code-block:: bash

	ptconfigure ping help

 kevell@corp:/# ptconfigure ping help

 ******************************


  This command allows you to test the status of ports

  Ping, ping

        - once
        ping a target once
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2

        - ten
        ping a target ten times
        example: ptconfigure ping ten --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2

        - until-responding
        ping a target for a set amount of time until it responds
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2
            --max-wait=100 # no seconds in total to keep trying, will guess 60

 ------------------------------
 End Help
 ******************************



options
-----------

Module PING ont trois options différentes, qui extraient des données que par l'option utilisée dans les commandes. Tableau ci-dessous explique la meme

.. cssclass:: table-bordered

 +------------------+-----------------------+--------------------------+----------------------------------------------------+
 | options          | Autres paramètres     | commandes                | fonctions                                          |
 +==================+=======================+==========================+====================================================+
 |Once              | Ping, ping            | ptconfigure ping once    | Nous ping une cible une fois. Une fois l'option    |
 |                  |                       | – yes –guess –target=    | permet de récupérer les données une seule fois     |
 |                  |                       | google.com – interval=5  |                                                    |
 +------------------+-----------------------+--------------------------+----------------------------------------------------+
 |Ten               | Ping, ping            | ptconfigure ping ten –   | Dix données de traction d'options pour dix fois,   |
 |                  |                       | yes –guess –target=      | ayant intervalle de temps que cinq secondes        |
 |                  |                       | google.com – interval=5  | [attend secondes avant d'envoyer le paquet suivant |
 +------------------+-----------------------+--------------------------+----------------------------------------------------+
 |Until-responding  | Ping, ping            | ptconfigure ping once    | nous ping la cible pour un montant fixé de temps   |
 |                  |                       | – yes –guess target=     | Jusqu'à il répond ayant intervalle de temps que 5  |
 |                  |                       | google.com – interval=5  | secondes et 100 secondes max pour essayer de la    |
 |                  |                       | wait=100                 | cible.|                                            |
 +------------------+-----------------------+--------------------------+----------------------------------------------------+


Remarque:

* Intervalle - Nombre de secondes d'attente entre chaque demande

* Max-attente - Nombre de secondes au total pour continuer à essayer

* Intervalle et Max-attente fréquence de temps peuvent être décidées par l'utilisateur que par l'exigence



Une fois l'option
-------------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping once --yes --guess --target=www.google.com

 [Pharaoh Logging] Ping Latency is 34 ms
 ******************************


 Ping Modifications:
 --------------------------------------------
 
 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************


dix Option
-------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping ten --yes --guess --target=www.google.com 

 [Pharaoh Logging] Ping Latency is 36 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 36 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************


Jusqu'à répondre
-----------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping once -- yes --guess --target=google.com -- interval=5 -- max-wait=100

 [Pharaoh Logging] Ping Latency is 37 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************


avantages
------------


PING permet à l'utilisateur de vérifier une adresse IP existence particulière et peut accepter la demande. Commande PING est la meilleure façon de tester la connectivité entre deux noeuds. Qu'il se agisse du réseau local (LAN) ou Wide Area Network (WAN).
