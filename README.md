# Projet-Titanic: Apprentissage automatique à partir d’une catastrophe
Ecrit par: Salem LUKAU MAKIESE<br>
Département MIASHS, UFR 6 Informatique, Mathématique et Statistique Université Paul Valéry, Montpellier 3

# Introduction
## Contexte du Projet
Au cours de notre premier semestre de Master MIASHS, nous avons entrepris un projet
qui englobe l’ensemble des compétences acquises. Ce document synthétise le travail réalisé
durant ce semestre, en mettant l’accent sur l’élaboration d’un algorithme de prédiction.
Notre travail s’est déroulé sur la plateforme Kaggle, où nous avons utilisé l’apprentissage
automatique pour étudier une tragédie historique : le naufrage du Titanic. Le Titanic,
souvent qualifié d’“insubmersible”, a coulé lors de son voyage inaugural le 15 avril 1912
après avoir percuté un iceberg, entraînant la mort de 1502 des 2224 passagers et membres
d’équipage à bord. <br>
Dans ce cadre, nous avons cherché à développer un modèle prédictif pour répondre à la
question : “Quels types de personnes étaient les plus susceptibles de survivre ?” Pour cela,
nous avons utilisé les données des passagers (nom, âge, sexe, etc.). Nous avons disposé de
deux ensembles de données similaires. Le premier, “train.csv”, comprenait les détails d’un
sous-ensemble de passagers à bord (891 pour être précis) et indiquait s’ils
avaient survécu ou non. Le second, “test.csv” (voir figure 22), contenait des informations
similaires mais sans révéler le sort des passagers. Il était de notre responsabilité de prédire
ces résultats.<br>
En exploitant les modèles que nous avons découverts dans les données, nous avons prédit
si les 418 autres passagers à bord (trouvés dans “test.csv”) ont survécu. L’ensemble d’entraînement a 
été utilisé pour construire nos modèles d’apprentissage automatique. Pour cet
ensemble, nous avons fourni le résultat (ou “vérité de terrain”) pour chaque passager. Notre
modèle a été basé sur des “caractéristiques” telles que le sexe et la classe des passagers.
L’ensemble de test a été utilisé pour évaluer la performance de notre modèle. Pour chaque
passager dans l’ensemble de test, nous avons utilisé le modèle que nous avons formé pour
prédire s’ils ont survécu ou non au naufrage du Titanic.<br>
Enfin, nous avons inclus “gendersubmission.csv”, un ensemble de prédictions qui suppose
que toutes les femmes ont survécu. Cela nous a permis d’avoir un exemple de ce à quoi un
fichier de soumission devrait ressembler, de comprendre la structure de la soumission et de
comparer notre modèle à une hypothèse de base.
## Dictionnaires de données
Les variables sont des indicateurs clés dans notre ensemble de données. Elles nous donnent des informations précieuses sur le statut socio-économique (pclass), l’âge (age), les relations familiales (sibsp et parch) des individus. Chaque variable a une signification spécifique et une valeur qui contribue à notre compréhension globale des données. Il est important
de noter que certaines variables peuvent avoir des valeurs fractionnées ou estimées, et que
certaines relations familiales peuvent ne pas être représentées.

| Variable         | Définition          |   Clé                           |
| ---------        | ---------            | ---------                       |
| survival         | Survie               | 0 = Non, 1 = Oui               |
| pclass           | Classe du billet       | 1 = 1ère, 2 = 2ème, 3 =3ème  |
| sex   | Sexe   | female = Femme, male =Homme   |
| Age   | Âge en années   | Pas de clé   |
| sibsp   | Nombre de frères/sœurs/époux à bord du Titanic  | Pas de clé   |
| parch   | Nombre de parents/enfants à bord du Titanic   | Pas de clé   |
| ticket   | Numéro du billet   | Pas de clé   |
| fare   | Tarif du passager   |  Pas de clé  |
| cabin   | Numéro de la cabine   |  Pas de clé  |
| embarked   | Port d’embarquement   | C = Cherbourg, Q= Queenstown, S =Southampton    |

# Analyse Exploratoire des Données (AED)
L’Analyse Exploratoire des Données constitue une phase cruciale de tout projet en science des données ou en apprentissage automatique. Elle nous offre l’opportunité d’appréhender la nature intrinsèque des données que nous manipulons.
## Analyse Préliminaire et Nettoyage des Données
Avant de nous immerger dans l’analyse des données, il est impératif de saisir les informations fondamentales relatives à notre jeu de données. Cela englobe la compréhension du
nombre de caractéristiques, du type de ces caractéristiques (numériques, catégoriques), ainsi
que de la présence éventuelle de valeurs manquantes.
Comme l’illustre la figure ci-dessous, notre jeu de données englobe 891 passagers. Néanmoins, certaines variables, telles que l’âge et le port d’embarquement, renferment des valeurs
manquantes que nous devrons traiter. De surcroît, les variables “Name”, “Ticket” et “Cabin”
seront éliminées de nos jeux de données, car elles ne contribuent pas significativement à notre
analyse.
## Encodage et Gestion des Valeurs Manquantes
Nous sommes confrontés à des variables catégorielles, telles que “Sex” et “Embarked”,
qui nécessitent une conversion en valeurs numériques pour être exploitées. Par exemple, les
valeurs distinctes de “Sex”, à savoir “male” et “female”, ont été codées en 0 et 1 respectivement. Un processus analogue a été appliqué à la colonne “Embarked”

## Visualisations de Données
Nous avons effectué quelques visualisations

# Examen de Divers Modèles
Nous avons procédé à l’exploration de quatre modèles distincts. L’objectif principal de
cette démarche est de mettre en parallèle leurs performances respectives pour identifier le
modèle qui se révèle être le plus efficace.

# Conclusion
Ce projet, axé sur la classification binaire du naufrage tragique du Titanic, a permis une exploration approfondie des techniques d’apprentissage automatique appliquées à des données historiques. Nous avons franchi plusieurs étapes cruciales, notamment une préparation minutieuse des données, une exploration de divers modèles et une évaluation rigoureuse de leur performance.<br>

En somme, ce projet a mis en lumière le potentiel des techniques d’apprentissage automatique dans le domaine de la classification binaire. En continuant à affiner et à développer ces approches, il est possible d’obtenir des modèles encore plus performants, ouvrant ainsi la voie à des applications futures et à une meilleure compréhension des mécanismes sous-jacents aux événements historiques tels que le naufrage du Titanic. Cela souligne l’importance et la pertinence de l’apprentissage automatique dans l’analyse et la compréhension des événements historiques.

