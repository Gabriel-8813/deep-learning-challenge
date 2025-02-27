# deep-learning-challenge
Module 21 challenge
Report on Neural Network Model Performance for Alphabet Soup

# Overview of the Analysis

The purpose of this analysis is to evaluate the performance of a deep learning model developed to predict the success of applications in the Alphabet Soup dataset. This dataset contains various features related to applicants, and the goal is to classify whether each application is successful or not. By employing a neural network model, we aim to uncover patterns in the data that can lead to accurate predictions.

# Results

Data Preprocessing

# Target Variable:
IS_SUCCESSFUL: This binary variable indicates whether an application was successful (1) or not (0).
Feature Variables:
All columns in the dataset except for IS_SUCCESSFUL. These features may include various applicant characteristics such as education level, experience, and other relevant metrics.

# Variables to Remove:
Any identifier or non-informative variables that do not contribute to the prediction of success should be excluded. This could include columns like APPLICATION_ID or any other unique identifiers.

# Compiling, Training, and Evaluating the Model
Model Architecture:
Neurons and Layers:
First hidden layer: 80 neurons with ReLU activation function.
Second hidden layer: 30 neurons with ReLU activation function.
Third hidden layer: 10 neurons with ReLU activation function.
Output layer: 1 neuron with sigmoid activation function.

# Reason for Selection:
The chosen architecture was designed to capture complex patterns in the data while avoiding overfitting. The use of multiple layers allows the model to learn hierarchical representations of the data.
Achieved Target Model Performance:
The model achieved an accuracy of approximately 73.11% and a loss of 0.5584 on the test data.

# Steps Taken to Increase Model Performance:
Implemented a dropout layer with a rate of 10% to prevent overfitting.
Experimented with different numbers of neurons in each layer to find an optimal configuration.
Scaled the input features using StandardScaler to ensure that all features contribute equally to the model training.

# Summary
The deep learning model developed for the Alphabet Soup dataset demonstrated a respectable accuracy of 73.11%. While this performance is a good starting point, there is room for improvement.