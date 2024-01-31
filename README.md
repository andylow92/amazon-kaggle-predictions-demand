Kaggle Competition: Backlog Prediction
Overview

This repository contains my solution to the Kaggle competition titled "Backlog Prediction: MNR/Earlies Expected." In this competition, I achieved the 11th place by designing a regression algorithm to predict the difference between Earlies_Expand MNR_Exp based on a training dataset holding 5 months of historical values (01/02/2021 - 30/06/2021). The goal was to create a feasible forecast for EU Delivery Stations, taking into account day-of-week seasonality.
Competition Description

Inside AMZL Operations exists EU CO Forecast, a team that owns EU short-term planning Out for Delivery (OFD) volume forecast. The team predicts how many packages will arrive at Delivery Stations to adjust operation capacity accordingly. To ensure high performance, it is crucial to set up CAPs based on downstream capacity.
Goal

Design a regression algorithm that predicts the difference between Earlies_Expand and MNR_Exp based on historical data. The algorithm should be day-of-week aware to consider seasonality.
Data

    Training dataset (train_data.csv) containing historical values from 01/02/2021 to 30/06/2021.
    Test dataset (test.csv) for predictions in the entire month of July.

Evaluation Metric

The evaluation metric for this competition is Root Mean Square Error (RMSE), a common metric for regression problems that measures the difference between expected and actual values.
Submission Format

The submission files should contain two columns:

    Id: the combination of ofd_date (yyyy-mm-dd) and station (Dxx), joined by "_" (e.g., 2021-07-31_D33).
    Expected: predictions for the month of July.

Your solution should include one row per day predicted, and you should predict the difference between Earlies and MNRs for every day of July 2021 (31 days = 31 rows).
How to Use

    Clone this repository to your local machine.
    Ensure you have the required libraries installed: pandas, numpy, scikit-learn, matplotlib, seaborn, and more (as mentioned in the code).
    Train the regression algorithm using the provided training dataset (train_data.csv).
    Predict the backlog for the entire month of July using the test dataset (test.csv).
    Submit your predictions on Kaggle and evaluate your RMSE score.

Acknowledgements

I would like to thank Amazon for providing this dataset and Kaggle for hosting this competition.

Good luck with your regression algorithm and may you achieve outstanding results in this Kaggle competition!
