# NBA Shot Success Prediction Using K-Nearest Neighbors (KNN)

## Project Overview
This project implements a K-Nearest Neighbors (KNN) classifier from scratch to predict whether an NBA shot was successful (made or missed) based on shot location and game context data.

## Dataset
- Features orignally included: LOC_X, LOC_Y (shot coordinates), SHOT_DISTANCE, QUARTER, MINUTES_LEFT, SECONDS_LEFT, etc.
- Target variable: SHOT_MADE (1 if made, 0 if missed)
- Source: Public NBA shot data (found through Kaggle)

## Methodology
- Engineered a cumulative time feature combining quarter, minutes left, and seconds left to capture game timing.
- Calculated Euclidean distance between shots for neighbor identification.
- Tested multiple values of *k* (number of neighbors) to find optimal accuracy.
- Used unweighted majority voting to classify shots.
- Visualized accuracy vs. *k* to analyze model behavior.

## Results
- The model showed improved accuracy for moderate values of *k*.
- Successfully predicted shot success on unlabeled test data, generating a new feature that can be used for further analysis.

## How to Run
1. Clone the repo.
2. Open the Jupyter notebook `nba_knn_analysis.ipynb`.
3. Run each cell sequentially to preprocess data, train the model, evaluate accuracy, and generate predictions.

---

Feel free to reach out if you want to discuss the project or collaborate!

