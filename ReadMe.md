# 🏆 MOSEF Bank Churn Prediction - Kaggle Challenge

Bienvenue dans le projet **MOSEF Bank Churn Prediction**, réalisé dans le cadre d'un challenge Kaggle. Ce projet met en avant des techniques avancées de machine learning pour prédire le churn des clients bancaires avec une précision exceptionnelle.


Nous utilisons des techniques de preprocessing, d'ingénierie des variables et un modèle d'ensemble basé sur le stacking (CatBoost, XGBoost, LightGBM) pour atteindre une performance optimale mesurée par l'AUC.

---

## 📂 Structure du Projet

- **`notebook.ipynb`** : Le notebook principal contenant toutes les étapes, de la préparation des données à la génération des fichiers de soumission.
- **`resultats/`** : Dossier où sont enregistrés les fichiers submissions.

---

## 🛠 Fonctionnalités

### 1. **Prétraitement des Données**
- Gestion des valeurs manquantes, des outliers, et encodage des variables catégorielles.
- Transformation et création de nouvelles variables :
  - Transformation logarithmique des variables biaisées.
  - Interactions personnalisées entre les variables (e.g., `Tenure_NumOfProducts`, `Balance/EstimatedSalary`).

### 2. **Analyse Exploratoire**
- Visualisation des variables numériques et catégorielles.
- Analyse des distributions et des relations avec la variable cible (`Exited`).

### 3. **Modélisation**
- **Modèles de base** : CatBoost, XGBoost, LightGBM.
- **Ensemble Stacking** : Combine les modèles de base avec un méta-modèle (XGBoost ou CatBoost) pour améliorer la performance.
- **Validation croisée** : Utilisation de Stratified K-Fold pour une évaluation robuste.

### 4. **Évaluation**
- Calcul des scores AUC pour chaque pli et génération des courbes ROC.
- Courbe ROC moyenne pour une meilleure visualisation des performances.

### 5. **Soumission**
- Génération des prédictions sur les données de test et sauvegarde des résultats au format CSV.

---

## 🔧 Installation

### Prérequis
1. **Créez un environnement virtuel :**

   ```bash
   python -m venv env```

2. **Activation du venv :**
```bash
   env\Scripts\activate
   ```
3. **Installation du requirement :**
```bash
pip install -r requirements.txt
```


## 📈 Résultats

### Performances clés :
- **AUC moyenne sur les plis**.
- Courbes ROC détaillées pour chaque pli et une courbe moyenne.

## 📜 Utilisation

1. **Clonez ce dépôt :**

   ```bash
   git clone https://github.com/linabnz/MOSEF-Bank-Churn-Prediction.git
   
### Ouvrez le notebook Jupyter :

```bash
jupyter notebook notebook.ipynb
```
### Exécutez toutes les cellules pour :
- Prétraiter les données.
- Entraîner les modèles.
- Évaluer les performances.
- Générer les prédictions pour le fichier de soumission (enregistré dans **`resultats/`**).


### Contributeurs :
- [Sharon Chemmama](https://github.com/Sharon2607)
- [Lina Benzemma](https://github.com/linabnz)



