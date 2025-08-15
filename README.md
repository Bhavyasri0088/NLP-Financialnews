# Indian Financial News — NLP Project

This project focuses on **Natural Language Processing (NLP) for Indian Financial News**. We aim to preprocess, analyze, and classify financial news headlines/articles from Indian sources using various machine learning (ML) algorithms. The workflow covers data cleaning, feature extraction, NLP techniques, model training, and evaluation.

---

## Project Overview

- **Objective:**  
  Build and evaluate classifiers to predict sentiment or category from Indian financial news articles/headlines.
- **Tasks Covered:**  
  - Data loading, cleaning, and merging  
  - Text preprocessing (tokenization, lemmatization, removing stopwords)  
  - Feature engineering (TF-IDF, vectorization)  
  - Model training (Logistic Regression, Random Forest, XGBoost, Naive Bayes)  
  - Model evaluation (classification report, confusion matrix, ROC-AUC)  
  - Model persistence (saving with pickle/joblib)  
  - EDA and visualization (matplotlib, seaborn)

---

## Data Dictionary

| Column         | Description                              |
|----------------|------------------------------------------|
| `headline`     | News headline text                       |
| `article`      | Full news article text (if available)    |
| `date`         | Date of publication                      |
| `sentiment`    | Label: sentiment/category (target)       |
| `source`       | (Optional) News source                   |

> **Note:** Please adjust column names to match your actual dataset.

---

## File Structure

```
NLP-Financialnews/
│
├── IndianFinancialNews_merged_final.ipynb   # Main notebook with full workflow
├── [data files]/                           # Place your CSV/data files here
├── models/                                # Saved models/vectorizers (if any)
├── README.md                              # This file
```

---

## Setup & Installation

1. **Clone the repo and navigate to the project directory:**
   ```bash
   git clone https://github.com/Bhavyasri0088/NLP-Financialnews.git
   cd NLP-Financialnews
   ```

2. **Create a virtual environment & activate:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # for Linux/Mac
   venv\Scripts\activate     # for Windows
   ```

3. **Install required packages:**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn nltk spacy xgboost joblib
   ```

4. **Download NLTK data (if running for the first time):**
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   nltk.download('wordnet')
   ```

---

## How to Run

1. **Place your data files in the project directory** (adjust paths if needed).
2. **Open and run the notebook:**
   - Use Jupyter Notebook, JupyterLab, or VS Code.
   - Run all cells from top to bottom.
3. **Adjust any file paths as needed** in code cells referencing data or output files.
4. **Models and vectorizers** may be saved in the `models/` directory for reuse.

---

## Key Technologies

- **Pandas, NumPy:** Data loading, cleaning, manipulation
- **NLTK:** Tokenization, stopwords, lemmatization
- **Scikit-learn:** ML models, feature extraction, evaluation
- **XGBoost:** Gradient boosting classifier
- **Matplotlib, Seaborn:** Visualization
- **Pickle/Joblib:** Model persistence

---

## Reproducibility

- Set random seeds where possible for reproducible results.
- Keep a requirements.txt for exact versions (optional).
- Save trained models/vectorizers for consistent inference.

---

## Authors

Goddati.Bhavyasri

## contact
goddatibhavya@gmail.com

For questions, open an issue or contact goddatibhavya@gmail.com

```
