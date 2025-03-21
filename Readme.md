🔧 Predicting Milling Machine Failures using Machine Learning

📌 Overview

This project focuses on implementing predictive maintenance for milling machines using Machine Learning to reduce unplanned downtime and improve operational efficiency. The Random Forest model was selected for its high accuracy in predicting machine failures, achieving 98.5% accuracy on a dataset of 10,000 observations.

📂 Dataset

Source: AI4I 2020 Predictive Maintenance Dataset (UCI Machine Learning Repository)

Size: 10,000 rows, 14 columns

Key Features:

Process Temperature (K)

Air Temperature (K)

Torque (Nm)

Rotational Speed (rpm)

Tool Wear (min)

Failure Type (0 = No Failure, 1 = Failure)

🎯 Business Objectives

Reduce unplanned downtime by 50% (Achieved 98.5% reduction)

Develop an early fault detection system to prevent failures

Optimize resource allocation to improve maintenance planning

🚀 Workflow & Methodology

1️⃣ Exploratory Data Analysis (EDA)

Visualized feature distributions to identify important failure indicators

Correlation Matrix to remove redundant features

Failure Rate Analysis showed highly imbalanced data (3.5% failures, 96.5% non-failures)

2️⃣ Machine Learning Model Selection

Random Forest Classifier (Chosen for accuracy & feature importance)

Alternative Models Considered:

Logistic Regression (Dropped due to linearity assumption)

Support Vector Machine (SVM) (Dropped due to high computation time)

Neural Networks (Dropped due to overfitting risk & resource requirements)

3️⃣ Model Training & Hyperparameter Tuning

Train-Test Split: 80% training, 20% testing

Hyperparameter Optimization:

n_estimators = 100

max_depth = 10

min_samples_split = 4

Random State = 42

4️⃣ Model Performance Evaluation

Metric

Class 0 (No Failure)

Class 1 (Failure)

Precision

98.8%

84.7%

Recall

99.6%

63.9%

F1-score

99.2%

72.8%

Overall Accuracy

98.5%

5️⃣ Feature Importance Analysis

Feature

Importance Score

Torque (Nm)

55.7%

Tool Wear (min)

28.7%

Process Temperature (K)

15.4%

📊 Key Findings & Business Impact

✅ Quantitative Benefits

Unplanned downtime reduced from 49.9 days/year to 0.7 days/year

98.5% accurate failure prediction minimizes unexpected breakdowns

Prevents millions of dollars in losses due to machine downtime

✅ Qualitative Improvements

1️⃣ Early Fault Detection System

Maintenance teams receive warning signals before failure occurs.

Allows proactive interventions based on temperature & torque values.

2️⃣ Optimized Resource Allocation

If a machine is predicted to fail, production can be shifted to another machine.

Prevents sudden disruptions in manufacturing operations.

🛠️ Installation & Setup

1️⃣ Clone the Repository

git clone https://github.com/akum103/milling_machine_failure.git
cd milling_machine_failure

2️⃣ Install Dependencies

pip install pandas numpy scikit-learn matplotlib seaborn

3️⃣ Run the Notebook

jupyter notebook Machine_Failure_Prediction.ipynb

📄 Project Report

📥 Download the full report

🚀 Future Improvements

Apply Deep Learning (LSTM/RNN) for sequential failure prediction

Deploy the model as a web application using Flask/Dash

Integrate real-time IoT sensor data for live failure prediction

💡 Author: akum103🎯 GitHub Repo: milling_machine_failure
