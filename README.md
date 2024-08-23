# Heart Disease Prediction
## Overview

The Heart Disease Prediction App estimates the percentage of heart disease in a population based on input percentages of biking and smoking. It uses a multiple linear regression model trained on a dataset from 500 fictional towns, which includes data on biking rates, smoking rates, and heart disease prevalence.

## Features

- Web Interface: Users can enter the percentage of people biking to work and smoking to receive a prediction of heart disease percentage.
- Model: The application uses a multiple linear regression model to make predictions based on the input data.
- Visualization: Includes plots to help users understand the relationship between biking, smoking, and heart disease rates.

## Dataset

The model is trained using a dataset that contains:

- Percentage of people biking to work: Reflects how many people bike to work in the sample towns.
- Percentage of people smoking: Indicates the proportion of smokers in the sample towns.
- Percentage of people with heart disease: Shows the prevalence of heart disease in the towns.

The dataset is an imaginary sample of 500 towns designed to illustrate the relationships between these variables.

## Prerequisites

- Python 3.x
- Flask: Web framework for creating the web interface.
- Scikit-learn: For building and using the regression model.
- Pandas: For data manipulation and analysis.
- Seaborn: For creating plots to visualize data.
- Pickle: For saving and loading the trained model.

## Code Structure

- app.py: Contains the Flask application code that handles web requests and predictions. It serves the web interface and processes user inputs.
- train_model.py: Script used to train the multiple linear regression model with the dataset and save the trained model as model.pkl.
- heart_data.csv: The dataset file used for training the model. It contains data on biking, smoking, and heart disease rates.
- templates/index.html: HTML template for the web interface where users input their data and receive predictions.
- model.pkl: Serialized file of the trained model used by the Flask app to make predictions.
