**Project Overview**

This project aims to predict worldwide box office revenue for movies using machine learning techniques. By analyzing factors like production budget, runtime, IMDb ratings, and audience votes, we can estimate a movie’s potential earnings.

**Repository Contents**

- **Predicting Movie Box Office Revenue.ipynb** – Main notebook for data processing, model training, and evaluation.
- **README.md** – Documentation for the project, including methodology and results.
- **movie_statistic_dataset.csv** – The dataset used in this analysis.

**Libraries Used**

- `pandas` – Data manipulation
- `numpy` – Numerical operations
- `matplotlib` & `seaborn` – Data visualization
- `scikit-learn` – Machine learning models and evaluation

**Methodology**

This project follows the **CRISP-DM** process:

1. **Exploratory Data Analysis (EDA)**
   - Histograms to understand feature distributions.
   - Correlation heatmaps to identify relationships.
   - Outlier removal for better predictions.

2. **Feature Engineering & Data Processing**
   - Log transformation for highly skewed variables (`budget`, `revenue`, `votes`).
   - Feature selection focusing on key numerical attributes.
   
3. **Model Training & Evaluation**
   - **Linear Regression** (Baseline model) → `R² = 0.68`
   - **Random Forest Regressor** (Improved model) → `R² = 0.72`
   - **Hyperparameter Tuning (GridSearchCV)** → `R² = 0.73`
   
4. **Prediction Scenario**
   - Predicted a new movie’s revenue using the trained model.
   - **Example Movie:** $200M budget, 130 min runtime, 7.5 IMDb rating, 500K votes.
   - **Prediction:** **$565.9M worldwide revenue**.

**Key Findings**

- **Budget and audience engagement are major predictors** of box office success.
- **Random Forest outperformed Linear Regression**, capturing nonlinear relationships better.
- **Genre-based revenue analysis could be a next step** for improvement.

**Acknowledgments**

- **Dataset Source:** [The Ultimate Film Statistics Dataset](https://www.kaggle.com/datasets/alessandrolobello/the-ultimate-film-statistics-dataset-for-ml) from Kaggle.
- **Libraries:** `scikit-learn`, `pandas`, `seaborn`, and others for analysis.

🔗 **To view the full analysis and insights, check out my Medium post:** [Predicting Movie Box Office Revenue](https://medium.com/@dh.aloraini/predicting-movie-box-office-revenue-a-data-science-approach-248c8d402036).
