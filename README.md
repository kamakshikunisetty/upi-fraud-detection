
UPI Fraud Detection using Machine Learning

This project focuses on detecting fraudulent UPI (Unified Payments Interface) transactions using machine learning techniques. The goal is to build an accurate, efficient, and reliable fraud detection system using real-world inspired transaction data.

📌 Project Overview

UPI transactions are increasing rapidly, and with them, fraud cases are also rising. This project uses machine learning models—primarily XGBoost and Random Forest—to classify transactions as Fraud or Non-Fraud.

The workflow includes:

Data loading and cleaning

Exploratory data analysis (EDA)

Feature engineering

Preprocessing using a Pipeline

Baseline model training

Hyperparameter tuning

Final model evaluation

Visualizations (ROC curve, Precision–Recall curve, Confusion Matrix)

📂 Dataset

The dataset contains UPI transaction records with features such as:

Transaction amount

Transaction type

Device information

Time of transaction

Merchant details

Fraud label (0 = Non-Fraud, 1 = Fraud)

Dataset used: 5000 transactions with ~10% fraud cases (custom dataset provided by user)

🧹 Data Preprocessing

Steps performed:

Removed missing and duplicate records

Encoded categorical variables using OneHotEncoder

Scaled numerical features using StandardScaler

Balanced the classes if necessary

Prepared a unified preprocessing pipeline

📊 Exploratory Data Analysis (EDA)

Conducted EDA to understand:

Amount distribution

Fraud vs Non-fraud ratios

Relationships between features

Correlation heatmaps

Outlier patterns

This helped identify important behavioral trends in fraud transactions.

🤖 Machine Learning Models Used

Baseline XGBoost Model
Trained using default parameters

Gave initial accuracy and recall

Served as the benchmark for tuning

Tuned XGBoost Model
Hyperparameter tuning using GridSearch/RandomizedSearch

Improved accuracy, precision, recall, and F1-score

Better handling of imbalanced data

Random Forest Classifier
Strong performance with low false positives

Confusion matrix shows high accuracy

Works well for tabular financial data

📈 Model Evaluation Metrics used:

Accuracy

Precision

Recall

F1-score

ROC-AUC Score

Precision–Recall AUC

Visualizations:

ROC Curve

Precision–Recall Curve

Confusion Matrix

Example insight: Random Forest achieved high true negatives and low false positives, making it reliable for banking systems.

🧪 Sample Predictions

The final tuned model was used to generate predictions on test samples, successfully identifying:

Normal customer transactions

Suspicious high-risk fraudulent patterns

📌 Conclusion

The XGBoost and Random Forest models performed well in detecting UPI fraud. The tuned XGBoost model shows the best balance between precision and recall, making it suitable for real-time fraud monitoring applications.

Further improvements can include:

Adding more behavioral features

Using deep learning models

Real-time streaming with Kafka / Spark

Larger and more diverse datasets
