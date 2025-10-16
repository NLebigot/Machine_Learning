Prédiction de maladies cardiaques par Machine Learning
Objectif

Ce projet vise à développer un modèle de machine learning capable de prédire la présence d’une maladie cardiaque chez un patient à partir de données médicales. L’enjeu est de détecter précocement les patients à risque afin d’améliorer leur prise en charge. Pour cela, plusieurs algorithmes ont été entraînés et comparés (régression logistique, GLM, Random Forest, Random Forest optimisée, réseau de neurones, XGBoost) afin d’identifier le modèle le plus performant.

Données

Le jeu de données provient de la base UCI Heart Disease, qui compile des informations cliniques de patients (âge, sexe, type de douleur thoracique, pression artérielle, cholestérol, etc.). Chaque entrée représente un patient, et la variable cible HeartDisease indique si ce patient souffre d’une maladie cardiaque (1 = oui, 0 = non).

Méthodologie

La méthodologie a mobilisé plusieurs compétences : nettoyage des données (traitement des valeurs manquantes et des anomalies), analyse exploratoire (visualisation des distributions, corrélations) et sélection de variables pertinentes pour la modélisation. Différents modèles ont ensuite été entraînés, avec optimisation des hyperparamètres (ex. GridSearchCV pour la Random Forest) et évaluation des performances via validation croisée et métriques (matrices de confusion, F1-score, AUC), puis visualisation des résultats (courbes ROC, comparatif des modèles).

Technologies

Développement réalisé en Python (Jupyter Notebook) avec les bibliothèques Pandas, NumPy, Scikit-learn, Statsmodels, TensorFlow/Keras, XGBoost et les outils de visualisation Matplotlib/Seaborn.

Résultats clés

Comparaison des performances des modèles (F1-score en validation croisée et AUC ROC).
Le graphique ci-dessus compare le F1-score et l’AUC des différents modèles. XGBoost ressort comme le meilleur modèle avec un F1-score de 0,88 et une AUC de 0,92. Il est suivi de près par le réseau de neurones (F1 ≈ 0,85, AUC 0,90) et la Random Forest optimisée (F1 0,86, AUC 0,92), aux performances presque équivalentes. En comparaison, les modèles linéaires (régression logistique et GLM) se révèlent moins performants (F1 ~0,75–0,79, AUC ~0,78).

👉 **XGBoost** offre la meilleure performance globale, combinant robustesse, stabilité et précision.
