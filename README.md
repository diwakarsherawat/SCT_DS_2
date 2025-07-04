 🚢 Titanic Survival Prediction & Exploratory Analysis
This project takes a deep dive into the iconic Titanic dataset from Kaggle. The goal was to clean and analyze the data, engineer meaningful features, and build a predictive machine learning model to determine which passengers were more likely to survive.

📁 Dataset Overview
The dataset originates from Kaggle’s Titanic Machine Learning Competition and includes:

train.csv — Training set with survival labels

test.csv — Test set without survival outcomes

gender_submission.csv — Example submission file format

🎯 Project Goals
Explore and visualize passenger demographics and survival patterns

Handle missing and inconsistent data

Engineer new features to boost model performance

Train and evaluate a classification model

Generate a valid submission file for the Kaggle leaderboard

🛠️ Tools & Technologies
Python 🐍

Pandas, NumPy for data manipulation

Matplotlib, Seaborn for visualization

Scikit-learn for modeling and evaluation

Jupyter Notebook / Google Colab as the development environment

🔎 Exploratory Data Analysis (EDA)
During EDA, the following analyses were performed:

Checked for null values and data distribution

Explored survival patterns based on:

Gender

Passenger Class (Pclass)

Embarked Port

Age groups

Family Size

Created visualizations:

Count plots

Histograms

Box plots

Heatmaps for feature correlation

Sample Plot:

python
Copy code
sns.countplot(x='Survived', hue='Sex', data=train_df)
🧹 Data Cleaning
Steps taken to prepare the dataset:

Imputed missing Age values using median

Filled missing Embarked entries with mode

Replaced missing Fare in the test set with median

Dropped Cabin due to excessive missing data

🏗️ Feature Engineering
New features and transformations included:

Extracted passenger titles (e.g., Mr, Mrs, Miss) from the Name column

Encoded categorical variables (Sex, Embarked, Title) numerically

Created FamilySize = SibSp + Parch + 1

Dropped less relevant columns: Ticket, Name, Cabin, PassengerId
