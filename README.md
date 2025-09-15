#  SyriaTel Customer Churn Prediction

##  Contexte
SyriaTel, un opérateur télécom, souhaite réduire les pertes financières liées à l’attrition des clients (**churn**).  
L’objectif est de construire un **modèle de classification binaire** permettant de prédire si un client risque de résilier prochainement.

---

##  Objectifs du projet
- Identifier les clients les plus à risque de churn  
- Détecter les variables clés qui influencent l’attrition  
- Fournir des recommandations business pour améliorer la fidélisation  
- Proposer un pipeline reproductible pour l’entreprise  

---

##  Dataset
- **Source** : [Kaggle – SyriaTel Customer Churn](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset)  
- **Nombre d’observations** : 3333 clients  
- **Variables clés** :  
  - `Churn` (cible binaire : Yes/No)  
  - `International plan`  
  - `Customer service calls`  
  - `Total day minutes`, `Total eve minutes`, etc.  

---

##  Méthodologie
1. **Préparation des données** : nettoyage, encodage, scaling  
2. **Analyse exploratoire (EDA)** : distribution du churn, corrélations, outliers  
3. **Modélisation** : Logistic Regression, RandomForest, XGBoost  
4. **Évaluation** : Accuracy, Precision, Recall, F1-score, matrice de confusion  
5. **Interprétation** : feature importance et recommandations  

---

## Résultats
- **Meilleur modèle** : RandomForestClassifier  
- **F1-score** : ~0.87  
- **Insights clés** :  
  - Les clients avec un **International plan** ont un risque élevé de churn  
  - Le nombre élevé de **Customer service calls** est fortement corrélé au churn  
  - Les minutes de jour influencent aussi la probabilité de churn  

---

##  Recommandations business
- Renforcer la qualité du **service client** (les clients qui appellent beaucoup sont plus à risque)  
- Revoir la tarification et les conditions de l’**International plan**  
- Lancer un programme de **fidélisation proactive** pour les clients identifiés comme à risque (>60%)  
- Monitorer en continu les métriques de churn  

---
