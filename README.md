# 📊 Bank Marketing - Prédiction de souscription

Ce projet vise à prédire si un client souscrira à un dépôt à terme à partir de données issues de campagnes de télémarketing d’une banque portugaise.

## 🧠 Objectif
Utiliser des modèles de machine learning (KNN et arbre de décision) pour prédire la variable cible `y` :
- `yes` : le client a souscrit
- `no` : le client n’a pas souscrit

## 🗃️ Données
Le dataset utilisé est `bank-additional-full.csv`, issu de l’article :
> Moro, Cortez & Rita (2014) – *A Data-Driven Approach to Predict the Success of Bank Telemarketing*

Il contient 41 188 lignes et 21 colonnes (20 features + cible `y`).

## ⚙️ Étapes principales
- Exploration des données
- Analyse de la variable cible
- Prétraitement (encodage, normalisation)
- Détection du déséquilibre de classes
- Modélisation : KNN, arbre de décision
- Évaluation avec des métriques adaptées (Recall, F1-score, AUC)

## 🛠️ Outils utilisés
- Python (pandas, matplotlib, seaborn, scikit-learn, Jupyter)
- Git & GitHub

## 📁 Fichiers importants
- `bank_marketing_knn_tree.ipynb` : notebook principal
- `requirements.txt` : dépendances Python

## ✍️ Auteur
Projet réalisé dans le cadre d’un cours d’intelligence artificielle – Licence 3.
