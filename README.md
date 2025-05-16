# Ames Housing Classification Project

This project uses the [Ames Housing dataset](https://www.kaggle.com/datasets/prevek18/ames-housing-dataset) to predict whether a house is priced **above or below the median sale price** using classification techniques. It involves data preprocessing, exploratory analysis, feature engineering, and model evaluation.

---

## Project Structure

- `project 1.ipynb` – The main Jupyter notebook containing code, analysis, and results.
- `requirements.txt` – List of required Python libraries.
- `readme.md` – This file.

---

## Objective

To build a binary classification model that predicts whether a home’s sale price is **above (`1`) or below (`0`) the median** value, using a combination of numerical and categorical features.

---

## Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (Logistic Regression, Decision Tree, model evaluation)

---

## Key Steps

### 1. **Data Preprocessing**

- Removed features with excessive missing values (1000+).
- Categorical missing values filled with `"Missing"`.
- Numerical missing values filled with median.
- One-hot encoding used for categorical features.

### 2. **Feature Selection**

- Selected features with correlation ≥ 0.35 with the target variable.
- Combined both numerical and encoded categorical features.

### 3. **Modeling**

- Built and evaluated:
  - Logistic Regression
  - Decision Tree (max depth = 5)
- Performance metrics: confusion matrix, accuracy, classification report.
- Cross-validation scores computed for both models.

### 4. **Visualization**

- Heatmap of feature correlations.
- Decision tree plot.
- Bar chart of top logistic regression coefficients.

---

## Results

Both models showed reasonable performance in classifying homes above or below the median value. Logistic regression offered interpretability, while the decision tree provided a visual and rule-based approach.

---

## Acknowledgments

- [Ames Housing Dataset](https://www.kaggle.com/datasets/prevek18/ames-housing-dataset)
- Scikit-learn team for robust machine learning tools.
