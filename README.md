# Titanic-survival-classification

🚢 Project Overview

This project predicts whether a passenger survived the Titanic disaster based on demographic and travel-related features such as age, sex, passenger class, fare, and family size.

I built multiple classification models and compared their performance using metrics like Accuracy, Precision/Recall/F1-score, and AUC-ROC Curve.

📘 Dataset

Source: Kaggle – Titanic: Machine Learning from Disaster

File used: train.csv

Samples: 891

Target Variable:

Survived (0 = No, 1 = Yes)

🧹 Data Cleaning & Preprocessing

Filled missing values:

Age → median

Embarked → mode

Dropped:

PassengerId

Name

Ticket

Cabin (too many missing values)

Created new features:

FamilySize = SibSp + Parch + 1

IsAlone = 1 if FamilySize == 1 else 0

One-Hot Encoding applied to:

Sex

Embarked

Pclass (if needed)

📊 Exploratory Data Analysis

Key visualizations include:

Survival rate by gender

Correlation heatmap
	Accuracy	AUC-ROC
~0.78	       ~0.80	
