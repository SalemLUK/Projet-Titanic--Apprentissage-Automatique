# Projet-Titanic: Apprentissage automatique à partir d’une catastrophe
# Introduction
# Contexte du Projet
Au cours de notre premier semestre de Master MIASHS, nous avons entrepris un projet
qui englobe l’ensemble des compétences acquises. Ce document synthétise le travail réalisé
durant ce semestre, en mettant l’accent sur l’élaboration d’un algorithme de prédiction.
Notre travail s’est déroulé sur la plateforme Kaggle, où nous avons utilisé l’apprentissage
automatique pour étudier une tragédie historique : le naufrage du Titanic. Le Titanic,
souvent qualifié d’“insubmersible”, a coulé lors de son voyage inaugural le 15 avril 1912
après avoir percuté un iceberg, entraînant la mort de 1502 des 2224 passagers et membres
d’équipage à bord.
Dans ce cadre, nous avons cherché à développer un modèle prédictif pour répondre à la
question : “Quels types de personnes étaient les plus susceptibles de survivre ?” Pour cela,
nous avons utilisé les données des passagers (nom, âge, sexe, etc.). Nous avons disposé de
deux ensembles de données similaires. Le premier, “train.csv”, comprenait les détails d’un
sous-ensemble de passagers à bord (891 pour être précis, voir figure 21) et indiquait s’ils
avaient survécu ou non. Le second, “test.csv” (voir figure 22), contenait des informations
similaires mais sans révéler le sort des passagers. Il était de notre responsabilité de prédire
ces résultats.
En exploitant les modèles que nous avons découverts dans les données, nous avons prédit
si les 418 autres passagers à bord (trouvés dans “test.csv”) ont survécu. L’ensemble d’entraînement a 
été utilisé pour construire nos modèles d’apprentissage automatique. Pour cet
ensemble, nous avons fourni le résultat (ou “vérité de terrain”) pour chaque passager. Notre
modèle a été basé sur des “caractéristiques” telles que le sexe et la classe des passagers.
L’ensemble de test a été utilisé pour évaluer la performance de notre modèle. Pour chaque
passager dans l’ensemble de test, nous avons utilisé le modèle que nous avons formé pour
prédire s’ils ont survécu ou non au naufrage du Titanic.
Enfin, nous avons inclus “gendersubmission.csv”, un ensemble de prédictions qui suppose
que toutes les femmes ont survécu. Cela nous a permis d’avoir un exemple de ce à quoi un
fichier de soumission devrait ressembler, de comprendre la structure de la soumission et de
comparer notre modèle à une hypothèse de base.
