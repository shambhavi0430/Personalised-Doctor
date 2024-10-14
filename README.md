# Personalised-Doctor
Project Overview: Personalized Medical Recommendation System
This project is designed to predict potential diseases based on user-input symptoms, leveraging machine learning models. The goal is to help users identify their conditions and provide medical recommendations using a dataset of medical conditions and symptoms.

Components of the Project:
Dataset Loading:

The project uses a dataset (Training.csv) that maps symptoms to diseases (prognosis).
The dataset is loaded using pandas for analysis.
Data Preprocessing:

The dataset is split into features (symptoms) and the target variable (prognosis).
LabelEncoder is used to transform the prognosis into numerical values for training the machine learning model.
Modeling:

Train-Test Split: The dataset is divided into training and test sets using train_test_split from sklearn.
A machine learning model (Support Vector Classifier, svc) is used to train the model. Features are binary encoded, where each symptom is either present (1) or absent (0).
Prediction Logic:

Input symptoms are provided by the user, converted into a vector, and passed to the machine learning model.
The model predicts the disease based on these symptoms.
Model Interpretation:

A function (get_predicted_value) maps the user's symptoms to the corresponding disease using the trained model and a list of diseases.
