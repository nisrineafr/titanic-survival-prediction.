# Titanic Survival Prediction
Titanic Survival Prediction - Ce projet utilise plusieurs algorithmes de machine learning (Régression Logistique, SVM, KNN, XGBoost, Random Forest) pour prédire la survie des passagers du Titanic. Il inclut le prétraitement des données, l'entraînement des modèles et la comparaison des performances.
## Introduction
Ce projet utilise des modèles de Machine Learning pour prédire la survie des passagers du Titanic en fonction de différentes caractéristiques (âge, sexe, classe de voyage, etc.). L'objectif est de comparer plusieurs modèles et de sélectionner celui offrant la meilleure performance.
## Données
Le dataset utilisé contient des informations sur les passagers, comme l'âge, le sexe, la classe du billet et le tarif payé. Ces données ont été nettoyées et prétraitées avant d'entraîner les modèles.
## Modèles Testés
Nous avons testé plusieurs modèles :
- **Régression Logistique**
- **SVM**
- **KNN**
- **XGBoost**
- **Random Forest**
## Résultats
Le tableau ci-dessous résume les performances des modèles :
| Modèle                  | Accuracy | Précision | Recall | F1-Score | ROC-AUC |
|-------------------------|----------|-----------|--------|----------|---------|
| **Régression Logistique**  | 0.8101   | 0.7778    | 0.7568 | 0.7671   | 0.8816  |
| **SVM**                    | 0.7765   | 0.7125    | 0.7703 | 0.7403   | 0.8693  |
| **KNN**                    | 0.6313   | 0.6667    | 0.2162 | 0.3265   | 0.6260  |
| **XGBoost**                | 0.8212   | 0.8088    | 0.7432 | 0.7746   | 0.8907  |
| **Random Forest**          | 0.8380   | 0.8358    | 0.7568 | 0.7943   | 0.8877  |
Le **Random Forest** est le modèle le plus performant avec une **accuracy de 83.80%** et un **F1-score de 79.43%**.
## Prédictions sur de nouvelles données
Le modèle Random Forest a été utilisé pour prédire la survie des passagers sur un dataset test (`test.csv`). Les prédictions sont enregistrées dans un fichier `predictions_random_forest.csv`.
## Exécution du Projet
**Installation des dépendances :**
```bash
pip install pandas numpy scikit-learn xgboost seaborn matplotlib
