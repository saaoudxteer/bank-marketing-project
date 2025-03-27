# 📊 Bank Marketing - Prédiction de souscription

Ce projet vise à prédire si un client va **souscrire à un dépôt à terme** à partir de données issues de **campagnes de télémarketing** d’une banque portugaise. Il est inspiré de l’article de référence de **Moro, Cortez & Rita (2014)**.

---

## 🎯 Objectif
Développer un modèle de **classification supervisée** pour prédire la variable cible `y` :
- `yes` : le client a souscrit à l’offre
- `no` : le client n’a pas souscrit

---

## 📁 Données utilisées
- **Fichier** : `bank-additional-full.csv`
- **Source** : Article scientifique  
  > Moro, Cortez & Rita (2014) – *A Data-Driven Approach to Predict the Success of Bank Telemarketing*  
- **Taille** : 41 188 observations, 20 variables explicatives + 1 variable cible

---

## ⚙️ Pipeline du projet

### 1. 📊 Exploration & compréhension des données
- Analyse de la distribution des variables
- Détection des valeurs manquantes ou “unknown”
- Visualisations : histogrammes, camembert, boxplots, heatmap

### 2. 🧹 Prétraitement
- Encodage des variables catégorielles (`get_dummies`)
- Transformation logarithmique des variables asymétriques (`duration`, `campaign`)
- Normalisation des variables numériques
- Sélection des variables les plus corrélées avec la cible
- Suppression des variables redondantes ou fortement corrélées

### 3. ⚠️ Déséquilibre des classes
- `yes` = ~11%, `no` = ~89%
- Application de la méthode **SMOTE** pour équilibrer les classes

### 4. 🧠 Modélisation
- **KNN (K-Nearest Neighbors)** avec choix optimal de `k` basé sur l’accuracy
- **Arbre de Décision**, avec et sans optimisation
- **Random Forest** avec **GridSearchCV** pour ajuster les hyperparamètres
- **XGBoost** en cours de test pour comparaison avancée

### 5. 📈 Évaluation
- Précision, rappel, F1-score
- **AUC-ROC** pour évaluer la capacité de discrimination
- Visualisation des comparaisons avec des **graphiques de performance**

---

## 🔧 Technologies utilisées

| Outil | Description |
|-------|-------------|
| Python | Langage principal |
| pandas / numpy | Manipulation des données |
| seaborn / matplotlib | Visualisation |
| scikit-learn | Prétraitement + modèles |
| imbalanced-learn | Méthode SMOTE |
| xgboost | Gradient boosting performant |
| Jupyter | Développement interactif |
| VS Code | Environnement de développement |
| Git & GitHub | Suivi de version |

---



