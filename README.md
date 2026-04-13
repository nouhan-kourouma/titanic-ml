# Titanic — Comparaison de modèles ML

## Objectif
Prédire la survie des passagers du Titanic en comparant 5 algorithmes de classification.

## Modèles comparés
- Logistic Regression
- Random Forest
- XGBoost
- SVM (RBF)
- KNN

## Résultats (CV 5-fold)
| Modèle | CV AUC |
|---|---|
| XGBoost | 0.881 |
| Random Forest | 0.879 |
| SVM (RBF) | 0.870 |
| Logistic Regression | 0.869 |
| KNN | 0.865 |

## Pipeline
1. EDA (distributions, corrélations, interactions)
2. Feature Engineering (Title, FamilySize, IsAlone, HasCabin)
3. Modélisation avec pipeline sklearn (imputation + scaling)
4. Évaluation : Cross-validation, AUC-ROC, matrice de confusion

## Structure
- `notebooks/` — notebook principal
- `data/` — données non committées https://www.kaggle.com/datasets/amineipad/titanic-dataset