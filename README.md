### Mental Health Condition Prediction using Wearable Data
Overview
This project aims to build a predictive model for identifying the likelihood of mental health conditions, such as anxiety or depression, using physiological and behavioral data collected from wearable devices. The dataset is synthetic and contains 10,000 samples, making it ideal for beginners to practice binary classification.

Dataset
The dataset used is synthetic and was generated to simulate real-world data patterns found in wearable devices. It includes features like heart rate, sleep duration, physical activity, and self-reported mood ratings.

Columns:
Heart_Rate_BPM: User’s heart rate in beats per minute.
Sleep_Duration_Hours: Hours of sleep per night.
Physical_Activity_Steps: Total number of steps in a day.
Mood_Rating: Self-reported mood rating (1-10 scale).
Mental_Health_Condition: Binary target variable (1: High risk, 0: No risk).
Objective
The main objective is to predict the Mental_Health_Condition of users based on their wearable data. The project employs various machine learning models to perform this binary classification task.

Features
Heart Rate (BPM)
Sleep Duration (hours)
Physical Activity (steps)
Mood Rating (scale 1-10)
Pipeline Overview
The project is modularized and uses a robust data pipeline to ensure scalability and maintainability. Below are the key components of the project:

1. Data Preprocessing
Data cleaning and handling of missing values.
Feature scaling using StandardScaler.
Splitting data into training and test sets.
2. Model Building
Logistic Regression
Decision Trees
Random Forest
Support Vector Machines
Neural Networks
Model performance will be evaluated using metrics like accuracy, precision, recall, and F1-score.

3. Model Tracking and Experimentation
MLflow is used to track experiments, log metrics, and store model artifacts for comparison and performance monitoring.
4. Data Pipeline Integration
Integrated with Datapipeline for smooth and scalable data processing, ensuring each stage in the machine learning workflow is modular and easy to debug.
5. Model Deployment
Final models are deployed, and predictions are made using the most efficient model.
Installation & Requirements
To run the project locally, clone the repository and install the required dependencies.

bash
Copy code
git clone <repo-url>
cd mental-health-condition-prediction
pip install -r requirements.txt
How to Run
Preprocess data using the data_preprocessing.py module.
Train models using the train_model.py script.
Track your experiments using MLflow.
Run the pipeline through the DagsHub interface.
Tools & Libraries
Python
Pandas for data manipulation
Scikit-learn for machine learning models
MLflow for experiment tracking
Datapipeline for data processing
Matplotlib/Seaborn for data visualization
Results
The model performance is tracked, and the best-performing model is selected based on F1-score, accuracy, precision, and recall. All results are logged in MLflow for future reference.

Contributions
Feel free to open a pull request to suggest improvements or new ideas.