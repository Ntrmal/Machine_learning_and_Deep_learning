## IPL Score Prediction using Machine Learning
# Project Overview
This project aims to predict the final scores of IPL (Indian Premier League) cricket matches using various machine learning algorithms. The dataset used for this project includes detailed information about each match, such as the batting and bowling teams, individual players, runs scored, wickets taken, and more.

# Dataset
The dataset consists of the following columns:

mid: Match ID

date: Date of the match

venue: Venue of the match

bat_team: Batting team

bowl_team: Bowling team

batsman: Batsman on strike

bowler: Bowler delivering the ball

runs: Runs scored on the current ball

wickets: Total number of wickets fallen till the current ball

overs: Number of overs completed

runs_last_5: Runs scored in the last 5 overs

wickets_last_5: Wickets fallen in the last 5 overs

striker: Batsman on strike's runs

non-striker: Runs scored by the non-striker

total: Total score at the end of the innings

Project Structure

data/: Contains the dataset files.

notebooks/: Jupyter notebooks for data exploration, preprocessing, model training, and evaluation.

models/: Serialized machine learning models.

README.md: Project overview and instructions.

# Usage
# Data Preprocessing:
Load the dataset.
Remove inconsistent teams.
Filter out unnecessary columns.
Remove the first 5 overs of each match.
# Feature Encoding:
Use LabelEncoder to encode categorical features (bat_team and bowl_team).
Use OneHotEncoder for one-hot encoding categorical features during model training.
# Model Training:
Train various machine learning models including Linear Regression, Decision Tree Regressor, Random Forest Regressor, and K-Nearest Neighbors Regressor.
Evaluate models using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
# Model Evaluation:
Evaluate the trained models on test data.
Use R-squared scores to determine the performance of the models.
# Score Prediction Function:
Implement a function score_predict to predict the final score based on input features.
# Visualization:
Visualize the distribution of runs and wickets using histograms.
