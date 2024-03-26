# Time Series Prediction Project

This project encompasses three distinct tasks, each addressing different predictive challenges within the dataset.

## Task 1: Log In and Log Out Time Prediction

The first task involves predicting the log in and log out times. This requires several preprocessing steps, including removing duplicate rows, handling null values, encoding categorical variables, and normalizing the data. Timestamps are converted into seconds to facilitate modeling, and lag features are calculated to capture temporal dependencies. Additionally, features such as the hour of the day and the day of the week extracted from the timestamps are incorporated into the model to enhance predictive performance.

### Metrics:
- R^2 Score: 0.10081
- Mean Squared Error: 0.00031
- Mean Absolute Error: 0.01128

## Task 2: Computer Usage Forecasting

The second task is a regression problem aiming to forecast the number of students using computers at any given time. All available columns are utilized in this model, undergoing proper encoding and normalization to prepare the data for modeling. Similar to the first task, lag features are computed to capture historical patterns, and timestamp features are derived and included as additional predictors.

### Metrics:
- R^2 Score: 0.6270
- Mean Squared Error: 7.402081620110233e-06
- Mean Absolute Error: 0.00211

## Task 3: Cluster Name Prediction

The third task focuses on a classification problem, predicting cluster names for log in or log out events. The model utilizes the last 10 lagged observations as predictors, allowing it to capture recent trends and patterns in the data. It is trained to classify log in and log out events into predefined clusters, contributing to a better understanding and management of user behavior.

### Metrics:
- Accuracy: 1.0
- Precision: 1.0
- Recall: 1.0
- F1 Score: 1.0

In each task, the predictive models are evaluated using the last 100 rows of data for testing, ensuring robust evaluation of model performance on unseen data. By addressing these diverse prediction challenges, the project aims to provide valuable insights and actionable recommendations for optimizing resource utilization and enhancing user experience in the analyzed environment.

