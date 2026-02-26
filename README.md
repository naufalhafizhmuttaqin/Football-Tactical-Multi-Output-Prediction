# Football Tactical Multi-Output Prediction

## Project Overview
This project aims to build a **Multi-Output Machine Learning Model** to predict football tactical decisions, including:

- Home Team Strategy
- Away Team Strategy
- Home Team Formation
- Away Team Formation

The model uses **Random Forest Classifier** wrapped with `MultiOutputClassifier` to simultaneously predict multiple tactical outputs.

This project demonstrates an end-to-end data science workflow:
> Data Understanding → EDA → Preprocessing → Modeling → Evaluation → Tactical Recommendation

---

## Problem Statement

Football tactical decisions such as formation and strategy significantly impact match outcomes.  
This project attempts to:

- Learn tactical patterns from historical match data
- Predict tactical setup for both teams
- Provide data-driven tactical recommendations

---

## Dataset

The dummy dataset contains:

- Team information (home & away)
- Opponent style
- Tactical decisions (strategy & formation)
- Match result (removed during modeling)

Target variables (multi-output):

- `home_strategy_used`
- `away_strategy_used`
- `home_formation_used`
- `away_formation_used`

---

## Tech Stack

- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn

---

## Exploratory Data Analysis (EDA)

- Distribution analysis of strategies and formations
- Class balance visualization
- Statistical summary of dataset

---

## Data Preprocessing

- One-hot encoding for opponent styles
- Label encoding for target variables
- Train-test split (80:20)
- Removal of irrelevant column (`result`)

---

## Model Architecture

Base Model: Random Forest
