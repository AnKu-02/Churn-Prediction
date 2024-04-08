# Churn-Prediction

## Overview
This project demonstrates how to implement a deep learning model to predict customer churn using TensorFlow and Keras. Customer churn prediction can help businesses identify customers likely to leave their service for competitors, enabling proactive measures to improve retention. The dataset used in this project contains various customer attributes along with their churn status.

## Setup and Installation
Ensure you have Python installed on your system. Then, install the required libraries.

## Key Libraries
- **pandas**: For data manipulation and analysis.
- **scikit-learn**: For splitting the dataset into training and testing sets.
- **tensorflow**: Provides the backend for Keras, a high-level neural networks API used for building and training deep learning models.

## Data Preprocessing
- Load the dataset using pandas.
- Convert categorical variables into dummy/indicator variables.
- Encode the target variable Churn as binary.
- Split the dataset into training and testing sets.

## Model Building and Training
1. Define a Sequential model with three Dense layers:
- The first layer with 32 neurons and 'relu' activation function.
- The second layer with 64 neurons and 'relu' activation function.
- The output layer with 1 neuron and 'sigmoid' activation function for binary classification.
2. Compile the model using 'binary_crossentropy' as the loss function, 'sgd' (Stochastic Gradient Descent) as the optimizer, and track 'accuracy' as the metric.

## Training and Evaluation
- Training: Train the model on the training data for 200 epochs with a batch size of 32.
- Evaluation: Predict churn on the test set and evaluate the model's performance using accuracy score.
- Saving and Reloading: Save the trained model for later use and demonstrate how to reload it to make new predictions.

## Conclusion
This project illustrates the power of deep learning for predictive modeling in a business context. By accurately predicting customer churn, businesses can take targeted actions to retain valuable customers and improve overall customer satisfaction.
