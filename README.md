# 🧠 Prédiction de Maladies Cardiaques — Projet de Machine Learning

## 🎯 Objectif
Ce projet vise à prédire la présence de maladies cardiaques à partir du **jeu de données UCI Heart Disease**.  
Plusieurs algorithmes de Machine Learning ont été comparés afin d’identifier le modèle le plus performant pour la détection précoce des pathologies cardiaques.

## 🧩 Contenu du projet
- **M_L.ipynb** : Notebook Jupyter complet (préparation, entraînement, évaluation).
- **Machine_Learning_N_L.pdf** : Rapport détaillé de l’analyse et des résultats.

## ⚙️ Technologies utilisées
- Python (pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, keras)
- Machine Learning : Régression Logistique, GLM, Random Forest, XGBoost, Réseau de Neurones
- Visualisation : Matplotlib / Seaborn

## 📊 Résultats clés
| Modèle | F1-score | AUC |
|:--------|:----------:|:------:|
| Régression Logistique | 0.76 | 0.78 |
| Random Forest (optimisé) | 0.86 | 0.92 |
| Réseau de Neurones | 0.82 | 0.90 |
| XGBoost | **0.88** | **0.92** |

👉 **XGBoost** offre la meilleure performance globale, combinant robustesse, stabilité et précision.
