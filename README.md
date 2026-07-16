# football-match-outcome-prediction
End-to-end machine learning pipeline for English Premier League match outcome prediction.

#  Football Match Outcome Prediction using Machine Learning

An end-to-end machine learning pipeline for predicting English Premier League match outcomes using historical match statistics and feature engineering.

##  Project Overview

This project predicts the outcome of English Premier League matches (Home Win, Draw, or Away Win) using machine learning models trained on five seasons of historical match data.

The project follows a complete machine learning workflow including data preprocessing, exploratory data analysis, feature engineering, model training, cross-validation, and performance evaluation.

---

##  Dataset

- **Competition:** English Premier League
- **Seasons:** 5 Seasons
- **Target Variable:** Full-Time Result (FTR)
  - Home Win
  - Draw
  - Away Win

- The project uses historical English Premier League match data from **five consecutive seasons**:

  - 2021–22
  - 2022–23
  - 2023–24
  - 2024–25
  - 2025–26

- These datasets were combined into a single dataframe before preprocessing and feature engineering.

---

##  Feature Engineering

The following features were engineered to improve predictive performance:

- Last 5 Match Points
- Last 5 Goals Scored
- Last 5 Goals Conceded
- Goal Difference
- Average Points Per Game
- Home/Away Form
- Rolling Performance Metrics

---

##  Models Used

- Dummy Classifier (Baseline)
- Random Forest Classifier
- XGBoost Classifier

---

##  Model Evaluation

Models were evaluated using **5-Fold Stratified Cross Validation** to obtain reliable performance estimates.

| Model | Mean Accuracy |
|--------|--------------:|
| Baseline | 44.60% |
| Random Forest | **49.74%** |
| XGBoost | 48.41% |

Random Forest achieved the highest average accuracy, while XGBoost demonstrated slightly more consistent performance across folds.

---

##  Repository Structure

```
football-match-outcome-prediction/
│
├── Football_Match_Outcome_Prediction.ipynb
├── requirements.txt
├── README.md
├── 2021-22.csv
├── 2022-23.csv
├── 2023-24.csv
├── 2024-25.csv
└── 2025-26.csv
```

---

##  Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

##  How to Run

1. Clone the repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook.
4. Run all cells sequentially.

---

##  Future Improvements

- Add expected goals (xG) based features
- Time-based validation
- Hyperparameter optimization
- Incorporate bookmaker odds as a benchmark
- Explore deep learning approaches

---

##  Author

**Nikhil Kumar**

B.Tech, Mechatronics and Automation Engineering

Indian Institute of Information Technology (IIIT) Bhagalpur
