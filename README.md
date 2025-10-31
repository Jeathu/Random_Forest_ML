# 🌳 Classification avec Random Forest

Ce projet implémente des modèles de **Random Forest** pour résoudre des problèmes de classification supervisée, en utilisant deux jeux de données populaires : **Iris** et **CIFAR-10**.

## 📁 Structure du projet

- `iris_with_forest.ipynb` : Notebook principal contenant les deux exercices
- `README.md` : Documentation du projet
- `iris.csv` : Jeu de données Iris (à inclure si non présent dans le notebook)

## 🎯 Objectifs

### Exercice 1 : Classification avec Forêts Aléatoires (Iris)
- Classification des fleurs Iris en 3 espèces
- Utilisation de Random Forest avec paramètres par défaut
- Évaluation des performances et optimisation des hyperparamètres

### Exercice 2 : Optimisation des Forêts Aléatoires (CIFAR-10)
- Classification d'images CIFAR-10 (10 classes)
- Prétraitement des données avec PyTorch
- Recherche d'hyperparamètres optimaux via GridSearch

## 📊 Résultats

### Exercice 1 - Iris
- **Accuracy** : 98%
- **Matrice de confusion** : Excellente séparation des classes
- **Rapport de classification** :
  - Setosa : 100% precision/recall
  - Versicolor : 94% precision, 100% recall
  - Virginica : 100% precision, 94% recall

### Exercice 2 - CIFAR-10
- **Accuracy validation** : 47% (modèle de base)
- **Accuracy test** : 47% (après optimisation)
- **Meilleurs paramètres** : 
  - `n_estimators` : 100
  - `max_depth` : None
  - `min_samples_split` : 2
  - `min_samples_leaf` : 1

## 🛠️ Technologies utilisées

- **Python 3.x**
- **Bibliothèques principales** :
  - `pandas`, `numpy` : Manipulation des données
  - `scikit-learn` : Machine Learning
  - `matplotlib`, `seaborn` : Visualisations
  - `torch`, `torchvision` : Traitement d'images CIFAR-10

## 📋 Méthodologie

### 1. Préparation des données
- Chargement et exploration des jeux de données
- Split train/test/validation
- Normalisation et prétraitement

### 2. Modélisation
- Implémentation de `RandomForestClassifier`
- Entraînement et évaluation
- Optimisation des hyperparamètres

### 3. Évaluation
- Métriques : accuracy, matrice de confusion, rapport de classification
- Validation croisée
- Recherche par grille (GridSearchCV)

## 🔧 Installation et exécution

1. **Cloner le repository** :
```bash
git clone [votre-repo-url]
cd [nom-du-repo]
