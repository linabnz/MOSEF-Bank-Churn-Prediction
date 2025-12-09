# 🏆 MOSEF Bank Churn Prediction - Kaggle Challenge

Welcome to the **MOSEF Bank Churn Prediction** project, completed as part of a Kaggle challenge.  
This project showcases advanced machine learning techniques to predict bank customer churn with exceptional accuracy.

We use preprocessing techniques, feature engineering, and an ensemble model based on stacking (CatBoost, XGBoost, LightGBM) to achieve optimal performance measured by AUC.

---

## Project Structure

- **`notebook.ipynb`**: The main notebook containing all steps, from data preparation to submission file generation.
- **`resultats/`**: Folder where submission files are stored.

---

## Features

### 1. **Data Preprocessing**
- Handling missing values, outliers, and encoding categorical variables.
- Transformation and creation of new features:
  - Log transformation of skewed variables.
  - Custom feature interactions (e.g., `Tenure_NumOfProducts`, `Balance/EstimatedSalary`).

### 2. **Exploratory Data Analysis**
- Visualization of numerical and categorical variables.
- Distribution analysis and relationship with the target variable (`Exited`).

### 3. **Modeling**
- **Base models**: CatBoost, XGBoost, LightGBM.
- **Stacking Ensemble**: Combines base learners with a meta-model (XGBoost or CatBoost) for improved performance.
- **Cross-validation**: Stratified K-Fold for robust evaluation.

### 4. **Evaluation**
- AUC scores for each fold and generation of ROC curves.
- Average ROC curve for easier interpretation of model performance.

### 5. **Submission**
- Predictions generated on the test set and saved as CSV submission files.

---

## Installation

### Prerequisites
1. **Create a virtual environment:**

   ```bash
   python -m venv env```

2. **Activate the virtual environment:**
```bash
   env\Scripts\activate
   ```
3. **Install dependencies:**
```bash
pip install -r requirements.txt
```


## Results

### Key Performance:
- **Average AUC across folds.**.
- Detailed ROC curves for each fold and a mean ROC curve.

## Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/linabnz/MOSEF-Bank-Churn-Prediction.git
   
### Open the Jupyter notebook:

```bash
jupyter notebook notebook.ipynb
```
### Run all cells to:
- Preprocess the data.
- Train the models.
- Evaluate performance.
- Generate predictions for the submission file (stored in resultats/).

### Contributors:
- [Sharon Chemmama](https://github.com/Sharon2607)
- [Lina Benzemma](https://github.com/linabnz)



