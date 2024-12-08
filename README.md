# GuessTheWinner-DataChallenge
Bienvenue dans le dépôt GitHub du projet Guess The Winner - Data Challenge, développé dans le cadre du data challenge "Football : Can you guess the winner?" organisé par QRT sur la plateforme Challenge Data. Ce défi met les participants au défi de prédire les résultats de matchs de football en exploitant des données historiques détaillées sur les équipes et les joueurs.

## Contexte du Data Challenge
Ce projet fait partie du data challenge "Football : Can you guess the winner?", proposé par QRT sur la plateforme Challenge Data. Ce défi a pour objectif de prédire les résultats des matchs de football dans différentes ligues et régions à partir de données statistiques détaillées.

L'objectif principal est de construire un modèle robuste et généralisable qui peut classer correctement les matchs selon trois résultats possibles :

* Victoire de l'équipe à domicile
*  Match nul
* Victoire de l'équipe à l'extérieur
Les données fournies incluent des statistiques historiques détaillées sur les performances des équipes et des joueurs, offrant une base riche pour appliquer des techniques de machine learning avancées.

## Objectif du Projet
Le défi consiste à résoudre un problème de classification multiclasse, en exploitant deux ensembles de données :

Données des équipes : Incluant des statistiques globales sur les performances des équipes lors des derniers matchs.
Données des joueurs : Incluant des statistiques détaillées sur les performances individuelles des joueurs.
Le but est de construire des modèles prédictifs capables de tirer parti de ces données pour fournir des prédictions fiables et généralisables, quelles que soient les ligues ou les régions.

## Structure du Dépôt
team_data_processing.ipynb : Notebook contenant le traitement des données et l'analyse exploratoire pour les statistiques des équipes.
player_data_processing.ipynb : Notebook dédié au traitement et à l'analyse des données des joueurs.
README.md : Ce fichier contenant la description du projet.
## Méthodologie
### 1. Prétraitement des données
Gestion des valeurs manquantes (imputation par médiane).
Transformation et normalisation des données avec StandardScaler.
Réduction de la dimensionnalité avec PCA.
Gestion des déséquilibres de classe avec SMOTE-Tomek Links.
### 2. Modèles utilisés
Les modèles testés incluent :

* Random Forest
* Gradient Boosting
* XGBoost
* LightGBM
* CatBoost
* K-Nearest Neighbors (KNN)
* Neural Networks
* Logistic Regression
* Ensemble Methods (Stacking, Voting)

### 3. Évaluation
Les modèles ont été évalués principalement avec la métrique Accuracy, définie comme :

##### Accuracy

$$
\text{Accuracy} = \frac{\text{Nombre de prédictions correctes}}{\text{Nombre total de prédictions}}
$$

Où :  
- Le **nombre de prédictions correctes** correspond aux instances correctement classées par le modèle.  
- Le **nombre total de prédictions** est le nombre total d'exemples dans les données évaluées.  
 
### 4. Soumissions
Les meilleurs modèles ont été sélectionnés pour effectuer des prédictions sur les données de test et générer des fichiers de soumission.

Résultats
Le modèle Ensemble Methods a obtenu la meilleure accuracy de 0.478 sur les données de test.
Les performances des autres modèles sont détaillées dans les notebooks.

#### Installation et Exécution
Prérequis: Python 3.8+

Librairies nécessaires : numpy, pandas, scikit-learn, xgboost, lightgbm, catboost, matplotlib, seaborn, shap.

Installation
Clonez ce dépôt :

` git clone https://github.com/samarelayed/GuessTheWinner-DataChallenge.git `

`cd GuessTheWinner-DataChallenge `

Installez les dépendances :

Exécution
Lancez les notebooks dans votre environnement préféré (ex. : Jupyter Notebook, VS Code, Google Colab) pour reproduire les analyses et les résultats.

