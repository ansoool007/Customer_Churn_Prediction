# Customer Churn Prediction using ANN

## Overview
This project aims to predict customer churn using an **Artificial Neural Network (ANN)**. The model is trained on a dataset from Kaggle and employs various preprocessing techniques, such as Min-Max scaling and one-hot encoding, to enhance prediction accuracy. Additionally, the **SMOTE** (Synthetic Minority Over-sampling Technique) algorithm is used to handle data imbalance in the target variable.

## Introduction
Customer churn prediction is a crucial task in many industries, allowing companies to identify customers likely to leave and take proactive retention measures. This project utilizes an Artificial Neural Network (ANN) to classify customers as churn or non-churn based on historical data. 

## Dataset
- **Source**: A training dataset from [Kaggle](https://www.kaggle.com/) was used.
- **Target Variable**: Churn (Binary classification - Yes/No)
- **Features**: A mix of numerical and categorical features that provide insights into customer behavior.

## Data Preprocessing
To ensure the data was ready for training, the following preprocessing steps were implemented:
- **Min-Max Scaling**: Applied to all numeric features to bring them into a standardized range [0, 1].
- **One-Hot Encoding**: Used `pd.get_dummies` to transform categorical variables into a format suitable for model input.
- **SMOTE Algorithm**: Employed to handle data imbalance in the target variable, ensuring a balanced distribution of the churn class.

## Model Architecture
The ANN model includes:
- **Input Layer**: Takes in preprocessed features.
- **Hidden Layers**: Multiple dense layers with sigmoid activation functions for learning complex patterns.
- **Output Layer**: A single neuron with a sigmoid activation function to output a binary churn prediction (0 or 1).

### Key Features:
- **Activation Function**: Sigmoid used for all layers to handle binary classification.
- **Loss Function**: `binary_crossentropy` for binary classification.
- **Optimizer**: Adam Optimizer for efficient model training.
- **Evaluation Metrics**: Accuracy, Precision, Recall, and F1-Score.
