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

4.  Visualisation des données


    1. Types de techniques de visualisation utilisées
    2. Utilisation de matplotlib


5.  Système de recommandation
    1. Stockage et gestion des préférences et du profil de l'utilisateur
    2. Utilisation d'algorithmes de recommandation

6.  Tests


    1. Présence de tests fonctionnels
    2. Présence de tests utilisateurs

7.  Rapport


    1. Clarté de la présentation
    2. Présence d'une introduction et d'une conclusion claires, architecture
        des diagrammes, un résumé des différentes tâches réalisées et des limites
    3. Bibliographie
