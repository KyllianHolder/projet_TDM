# projet_TDM

Rapport

Votre tâche finale consiste à préparer un rapport de 4 pages sur le projet en format PDF, qui détaille les points suivants :

Sources des données de vos images et leur licence.
Taille de vos données.
Informations que vous avez décidé de stocker pour chaque image.
Informations concernant les préférences de l'utilisateur
Les modèles d'exploration de données et/ou d'apprentissage machine que vous avez utilisés avec les métriques obtenues.
l'auto-évaluation de votre travail.
Remarques concernant les séances pratiques, les exercices et les possibilités d'amélioration.
Conclusion
Note : Veuillez n'ajouter aucun programme (ou code) dans ce rapport.

Intro :

Le but de notre projet est de créer un algorithme de recommandation des images en fonctions des préférences de l'utilisateur. Ce système de recommandation sert de filtrage de l'information visant à présenter la meilleure image qui serait susceptibles d'intéresser l'utilisateur.

1.  Collecte de données

Nos images sont sous licence libre et proviennent de Kaggle, qui est une plateforme web organisant des compétitions en science des données appartenant à Google. Sur cette plateforme, les entreprises proposent des problèmes en science des données et offrent un prix aux datalogistes obtenant les meilleures performances.

Nous avons téléchargé ca data set de 100 images et avons crée un repository sur GitHub, nous clonons via une commande git les images, qui arrivent ensuite directement dans un dossier situé sur notre projet d'algoritheme de recommandation.

On enregistre les métadonnées de chaque images dans un ou plusieurs fichiers JSON, les préférences sont triées selon les carristiques suivantes :
- tailles 
- le format de l'image (.jpeg, .png, etc.)
- couleurs 
- l'orientation de l'image (paysage, portrait, carré, etc.)

Pour leurs stockages, nous enregistrons les images dans des dossiers et nous stockons les métadonnées dans un fichier .json

2.  Étiquetage et annotation

Pour collecter ces données, nous demandont à l'utilisateur de classer une collection d'images en fonction de sa préférence. Pour cela, nous avons une base de centaines d'images et nous en tiront dix aléatoirement.

Pour effectuer cette recommandation, une question va lui être posé, lui demandant s'il aime ou non l'image que nous lui proposont, il fait cela dix fois, et nous analysons les caractéristiques des images qu'il a choisit.
Lorsque cette analyse est effectué, à la fin nous lui montront une image choisit selon notre algorithme, qui ressort une image qu'il serait susceptible d'apprecier.
   
3.  Analyses de données

Pour analyser les données, nous utilisons l'implémentation Kmeans, qui consiste à regrouper les éléments de notre jeu de donnée en groupes, appelés clusters. Le but est de faire ressortir les patterns cachés dans la donnée en regroupant les éléments qui se « ressemblent ». 
Nous récuperons une sélection d'informations sur laquelle va se baser notre système de filtrage en 3 étapes :
1) On receuille l'information
2) On bâti une matrice contenant l'information
3) On extrait à partir de cette matrice une suggestion d'image


4.  Visualisation des données

Nous avons fait un profil de like, calculer qu'une seule fois, mais à l'avenir nous souhaiterons rajouter un systeme qui nou spermettrait de liker les photos en continuité et d'adapter ce profil utilisateur en fonction de ses likes en fonctions de ses gouts, cela permettrait d'être plus précis.

    1. Types de techniques de visualisation utilisées
    2. Utilisation de matplotlib


5.  Système de recommandation

Notre système de recommandation actuel permet de proposer une image selon les gouts préalablement étudé de l'utilisateur. Pour le moment, nous n'avons pas crée de profil d'utilisateur à prorprement parlé, mais plutot un profil de like, l'utilisateur choisit d'aimer ou non une image lui étant proposé.

Quant au filtrage, on utilise un filtrage collaboratif mais basé sur le contenu. En effet, ce système qu'on utilise à pour but de faire des prévisions sur les goûts explicites de nos utilisateurs. C'est-à-dire que ce sera à notre utilisateur de donner son opinion, sur les propositions d'images qui lui est accessible. 
Cette méthode est notament utilsé par le celebre service de streaming Netflix, car ce site permet de donner son avis sur des produits.

Cette méthode présente deux avantages :

On peut facilement reconstruire l'historique d'un individu
On évite d'agréger des informations qui ne correspondent pas à un unique utilisateur (plusieurs personnes sur un même poste ou une personne agissant pour le compte d'autrui)
Son principal défaut étant que les informations recueillies peuvent contenir un biais dit de déclaration.


Pour le stockage et la gestion des préférences et du profil de l'utilisateur, on utilise un dictionnaire.
    
La limite de notre proposition est qu'on prend en compte tous les paramètres pour la recommandation, mais on définit pas le paramètre le plus important pour l'utilisateur, cela reste un axe d'amélioration qu'on souhaiterait produire avant de commencer la partie 2. 


6.  Tests

    1. Présence de tests fonctionnels
    2. Présence de tests utilisateurs

7.  Rapport

    1. Clarté de la présentation
    2. Présence d'une introduction et d'une conclusion claires, architecture
        des diagrammes, un résumé des différentes tâches réalisées et des limites
    3. Bibliographie
