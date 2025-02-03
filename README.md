# Fraud_Detection_using_PySpark

## Table of Contents
- Project Overview
- Technology Stack
- Installation
- Dataset Details
- Project Workflow
- Model Results
- Original paper (License)

## Fraud Detection System Using Advanced Machine Learning Techniques

Fraud detection involves identifying and preventing fraudulent activities, such as unauthorized financial transactions or identity theft. It plays a critical role in safeguarding businesses and individuals from financial losses. By leveraging advanced technologies like machine learning and big data analytics, fraud detection systems can analyze patterns, detect anomalies, and flag suspicious activities in real-time, ensuring security and trust in financial systems.

## Project Overview:

This project focuses on creating a fraud detection system using the BankSim dataset, a simulation of bank payments designed with the Multi-Agent-Based Simulation (MABS) framework. BankSim is derived from a sample of aggregated transaction data provided by a Spanish bank, aimed at fostering the development of Big Data applications. For more details about the dataset, please refer to the original paper linked under the "Original Paper" section and access the dataset through the link provided under the "Dataset" section.

The system leverages advanced machine learning techniques to identify fraudulent transactions effectively. Key methodologies include data balancing, feature engineering, and the use of scalable distributed computing for handling large datasets.
The primary goal is to optimize fraud detection while minimizing false positives and false negatives, ensuring precision and scalability for potential real-world applications.

## Technology Stack:

Programming Languages: Python,R
Frameworks & Libraries:
PySpark (MLlib)
scikit-learn, XGBoost
Pandas, NumPy, Matplotlib, Seaborn
Tools: Databricks, Jupyter Notebook,PowerBI
Techniques: SMOTE, Feature Engineering, Model Tuning

## Installation:

Download the files from the zip and save the files into your local machine.
You need to have a compatible software to execute the R and Python files. (We used R studio and Databricks for Python)
Import the files into respective software's and execute them.

## Dataset Details:

Dataset Name: BankSim Dataset 
Source : https://www.kaggle.com/ntnu-testimon/banksim1
* Size: 76.2 MB (594642 rows, 17 columns)
* Features: The dataset has 16 feature columns and a target column. The feature columms are :
Step: This feature represents the day from the start of simulation. It has 180 steps so simulation ran for virtually 6 months.
Customer: This feature represents the customer id
zipCodeOrigin: The zip code of origin/source.
Merchant: The merchant's id
zipMerchant: The merchant's zip code
Age: Categorized age
0: <= 18,
1: 19-25,
2: 26-35,
3: 36-45,
4: 46:55,
5: 56:65,
6: > 65
U: Unknown
Gender: Gender for customer
E : Enterprise,
F: Female,
M: Male,
U: Unknown
Category: Category of the purchase. 
Amount: Amount of the purchase
Transaction_frequency: Number of transactions per customer Avg_transaction_amt: Average amount transacted per customer
Time_of_day: Representative of time for each transaction-inferred from the 'step' variable 
Merchant_interaction: Numerical count
Amount_change_pct: The percentage change in transaction amount from the customer's previous transaction.
Zip_distance: The absolute difference between the customer's zip code and that of the merchant 
Category_count: Number of transactions each customer has made within a particular category 
Fraud: Target variable which shows if the transaction fraudulent(1) or benign(0)

## Project Workflow

1. Exploratory Data Analysis (EDA)
2. Data Preprocessing
3. Oversampling with SMOTE
4. Logistic Regression 
5. Random Forest Classifier
6. Gradient Boost Classifier
7. XGBoost Classifier
8. Deploymnet using PySpark
9. Results

## Model Results

-----------------------------------------------------------------------------------------------------
Model                Precision-Recall AUC    False Positives    Missed Fraud Cases (False Negatives) 
-----------------------------------------------------------------------------------------------------
Logistic Regression  0.728                   4,489              25
Random Forest        0.725                   4,469              16
Gradient Boosting    0.8705                  2,022              77
XGBoost (Best Model) 0.9202                  185                212
-----------------------------------------------------------------------------------------------------


## Original paper (License)
Lopez-Rojas, Edgar Alonso ; Axelsson, Stefan Banksim: A bank payments simulator for fraud detection research Inproceedings 26th European Modeling and Simulation Symposium, EMSS 2014, Bordeaux, France, pp. 144?152, Dime University of Genoa, 2014, ISBN: 9788897999324. https://www.researchgate.net/publication/265736405_BankSim_A_Bank_Payment_Simulation_for_Fraud_Detection_Research

