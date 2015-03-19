==================
Amazon CloudFront
==================

synopsis
-------------

Amazon CloudFront est un service de livraison de contenu web. Il s'intègre aux autres produits Amazon Web Services pour donner aux développeurs et aux entreprises un moyen simple de diffuser des contenus aux utilisateurs finaux avec une latence faible, les vitesses de transfert de données élevé et aucun engagement d'exigences minimales d'utilisation.


Amazon CloudFront permet d'offrir à votre site Web entier, y compris le contenu interactif, en continu, statique et dynamique à l'aide d'un réseau mondial de centres de bord. Demandes de votre contenu sont alors acheminés automatiquement vers l'endroit le plus proche du bord, contenu est livré avec le meilleur rendement possible. Amazon CloudFront est optimisé pour fonctionner avec les autres Services Web Amazon, Amazon Simple Storage Service (Amazon S3), Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Load Balancing et Amazon Route 53. Amazon CloudFront fonctionne également parfaitement avec n'importe quel serveur d'origine non-AWS, qui stocke les versions originales et définitives de vos fichiers. Comme les autres produits Amazon Web Services, il n'y a pas de contrats à long terme ou engagements d'utilisation mensuels minimums pour utiliser Amazon CloudFront – vous payez uniquement pour autant ou aussi peu de contenu que vous livrez en fait via le service de livraison de contenu.



Commande Aide
----------------------

Cette commande permet de déterminer l'utilisation d'Amazon CloudFront. L'utilisateur viendra à connaître la façon/format différent d'exécuter ce module. Cette commande guide l'utilisateur pour connaître le but de cette commande. Voici donnés sont le commandement et la capture d'écran de la même chose.


.. code-block:: bash


Alternative Paramètre
------------------------------       

Il y a trois paramètres de substitution qui peuvent être utilisés en ligne de commande.


AWSEC2, awsec2, aws-ec2


avantages
--------------

Console de gestion : Amazon CloudFront travaille avec l'AWS Management Console. Présent sur le web, pointer-cliquer, interface utilisateur graphique vous permet de gérer Amazon CloudFront sans écrire de code du tout.


Contenu dynamique : Utilisation Amazon CloudFront pour livrer l'intégralité de votre contenu, y compris les parties dynamiques de votre site qui changent pour chaque utilisateur final.


Support pour POST/PUT et autres méthodes HTTP: utilisation CloudFront d'accélérer les données téléchargées des utilisateurs finaux.


SSL personnalisé : Utiliser votre propre nom de domaine et votre propre certificat SSL pour fournir du contenu via HTTPS.

Invalidation : Retirer les copies d'un fichier de tous les endroits de bord Amazon CloudFront.


Soutien Wildcard CNAME : Mapper un nom de domaine générique à votre réseau de distribution Amazon CloudFront.


Support des Apex : Les visiteurs de votre site Web peuvent désormais accéder votre site à l'apex de la zone (ou « domaine racine »). Par exemple, votre site est accessible comme exemple.com plutôt que www.example.com.


Réponses d'erreur personnalisées : Configurer comment CloudFront gère les réponses d'erreur pour votre site Web.


