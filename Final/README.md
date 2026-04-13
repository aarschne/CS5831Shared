#  Allergen Detection Using Machine Learning

This repository contains a complete machine learning pipeline for detecting allergens in food products using nutritional and ingredient-level data. The project includes exploratory data analysis, classification modeling, and association analysis.

---

## Repository Structure

```
.
├── EDA.ipynb
├── Classification.ipynb
├── Associations.ipynb
├── Associationsnew.ipynb
├── CS5831FinalClassification.yaml
├── Data/
└── Archive/
```

---

##  Notebooks

### `EDA.ipynb`
- Performs **exploratory data analysis**
- Investigates:
  - Feature distributions
  - Skewness
  - Correlations
- Includes visualizations to better understand the dataset

---

### `Classification.ipynb`
- Trains and evaluates multiple classification models for allergen detection
- Models included:
  - Linear Discriminant Analysis (LDA)
  - Quadratic Discriminant Analysis (QDA)
  - Regularized LDA
  - XGBoost
  - TabNet
  - LightGBM
- Focuses on model performance and comparison

---

### `Associations.ipynb` / `Associationsnew.ipynb`
- Uses LDA models for each allergen
- Extracts **feature importance**
- Identifies relationships between features and specific allergens
- Helps interpret which variables are most influential

---

## Directories

### `Data/`
- Contains all datasets used in the notebooks
- Includes CSV files required for modeling and analysis

### `Archive/`
- Stores older or experimental notebooks
- Not required for main workflow, but kept for reference

---

## Environment Setup

The file `CS5831FinalClassification.yaml` defines the conda environment used for this project.

### Create the environment:
```bash
conda env create -f CS5831FinalClassification.yaml
conda activate CS5831FinalClassification
```

---

## Workflow Overview

1. Run `EDA.ipynb` to understand the data  
2. Use `Classification.ipynb` to train and evaluate models  
3. Run `Associations.ipynb` to interpret feature importance and relationships  

---

## Notes

- The project emphasizes **recall** as a key metric due to the safety-critical nature of allergen detection
- Feature importance analysis is used to improve interpretability
- Multiple modeling approaches are compared to ensure robust performance

---

## Author

Aaron Schneberger
