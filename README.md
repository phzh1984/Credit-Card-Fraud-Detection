# Credit-Card-Fraud-Detection-using-Artificial-Neural-Networks-ANNs-and-XGBoost

Overview

This repository contains Python code for a Credit Card Fraud Detection project. The goal of this project is to build and compare models based on Artificial Neural Networks (ANNs) and XGBoost to detect fraudulent credit card transactions.

Problem Statement

Credit card fraud is a significant problem for both credit card companies and cardholders. Fraudulent transactions can result in financial losses and inconvenience for cardholders. The objective of this project is to create a model that can accurately identify fraudulent transactions while minimizing false positives.

Dataset

The dataset used for this project contains credit card transactions made by European cardholders in September 2013. It consists of the following attributes:

V1-V28: Numerical features obtained from PCA transformation (anonymized).

Time: Seconds elapsed between each transaction and the first transaction.

Amount: Transaction amount.

Class: Binary label (1 for fraudulent transactions, 0 for genuine transactions).

Data Characteristics

Highly imbalanced dataset with less than 1% of transactions labeled as fraudulent.

Challenges

Imbalanced data: Dealing with the highly imbalanced nature of the dataset requires careful handling to avoid overfitting and biased models.

Lack of feature information: Due to confidentiality, no metadata is provided about the original features, limiting the ability to perform feature analysis.

Ground truth definition: Defining what constitutes "fraud" can be subjective, and establishing a reliable ground truth is challenging.

Approach

Two different modeling approaches are explored in this project: Artificial Neural Networks (ANNs) and XGBoost.

Artificial Neural Networks (ANNs): ANNs are a type of deep learning model that can capture complex patterns in the data. They will be trained on the dataset to classify transactions as either fraudulent or genuine.

XGBoost: XGBoost is a powerful gradient boosting algorithm known for its effectiveness in classification tasks. It will also be trained on the dataset and compared with the ANN model.

Evaluation

Due to the class imbalance, accuracy is not an appropriate metric for this problem. Instead, the Area Under the Precision-Recall Curve (AUPRC) will be used to assess model performance. The goal is to maximize recall while controlling the false positive rate.
