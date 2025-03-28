# Water Potability Prediction

## Project Overview
This project is a machine learning application developed to predict the potability of water. The dataset used in the project aims to classify whether water is potable or not based on various chemical and physical properties of the water. In this project, machine learning algorithms, particularly the Voting Classifier, have been used to combine models and achieve success in predicting potable water.

### Project Purpose
Predicting water potability is critically important for water resource management, health, and environmental issues. In this project, a model has been created to predict whether different water samples are potable. The model classifies water's potability based on analysis of its various chemical and physical parameters.

## Dataset
The dataset used in this project consists of various parameters related to water potability. The dataset includes the following features:

- **pH**: A value that indicates whether the water is acidic or alkaline.
- **Hardness**: The concentration of minerals in the water.
- **Chlorine**: The chlorine level in the water.
- **Oxygen**: The dissolved oxygen level in the water.
- **Phosphate**: The phosphate concentration in the water.
- **Sodium**: The sodium level in the water.
- **Magnesium**: The magnesium concentration in the water.
- **Potability**: Whether the water sample is potable or not (1: potable, 0: not potable).

### Labels
Each water sample has an associated label indicating its potability:
- **1**: Potable Water
- **0**: Not Potable Water

## Project Steps

### 1. Data Loading and Preprocessing
- **Data Loading**: The dataset is loaded in `.csv` format.
- **Missing Data**: Missing values in the dataset are filled using the mean or median.
- **Data Cleaning**: Outliers are detected and removed from the dataset.
- **Feature Normalization**: The data is normalized to eliminate scale differences between features.

### 2. Feature Selection
Some features in the dataset may not contribute to the model's accuracy. Therefore, only the most important features are selected. Feature engineering techniques are applied to remove unnecessary data and enhance the model's performance.

### 3. Model Selection and Training
Several machine learning algorithms have been used to train the model:
- **Logistic Regression**
- **Decision Trees**
- **Random Forest**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)**
- **Gradient Boosting Machine (GBM)**
- **XGBoost**

Additionally, a **Voting Classifier** has been created by combining the predictions of different algorithms. This allows for more accurate results by aggregating the predictions of various models.

### 4. Model Evaluation
To evaluate the model's performance, the following metrics have been used:
- **Accuracy**: The ratio of correctly predicted instances to the total instances.
- **Precision and Recall**: Precision measures the accuracy of positive predictions, while recall measures the ability to correctly identify positive cases.
- **F1-Score**: A metric that balances precision and recall.

### 5. Making Predictions
Once the model is trained, it is tested on unseen data, and predictions are made to determine whether the water samples are potable or not.

## Technologies and Libraries Used
The following technologies and libraries have been used in this project:
- **Python**: The programming language used for the project.
- **Pandas**: Used for data loading, processing, and analysis.
- **NumPy**: Used for numerical computations and data manipulation.
- **Scikit-learn**: Used for training and evaluating machine learning algorithms, and implementing the Voting Classifier.
- **XGBoost**: Used for Gradient Boosting models and advanced machine learning techniques.
- **Matplotlib / Seaborn**: Used for data visualization.
