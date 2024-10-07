# Titanic Survival Prediction Model - Azure Deployment
This project demonstrates how to build and deploy a Titanic Survival Prediction model using Logistic Regression in Python. The model is deployed on Azure Container Instances (ACI) using Azure Machine Learning services. The prediction model is trained on the famous Titanic dataset and predicts the likelihood of a passenger's survival based on a set of features.

# Project Structure
├── config.json                # Azure configuration file
├── logistic_regression_model.pkl # Trained Logistic Regression model
├── score.py                   # Scoring/inference script for model deployment
├── deployMLmodelAzure.ipynb.py # Script for model deployment on Azure
├── README.md                  # This file
└── requirements.txt           # Required dependencies

# Key Components
1. **Training and Model Registration:**
- The model is built using Logistic Regression from Scikit-learn.
- After training, the model is saved as a pickle file (logistic_regression_model.pkl).
- The model is then registered with Azure ML Workspace for deployment.
2. **Azure ML Workspace:**
A new Azure ML Workspace is created. This workspace manages all machine learning resources and deployments.

3. **Model Deployment:**
- The registered model is deployed using **Azure Container Instances (ACI)**, allowing for real-time inference.
- **InferenceConfig** is defined, which includes the model scoring script and environment details (dependencies).
- The deployed model is made available via a REST API endpoint.
# Setup Instructions
**Prerequisites:**
- Python 3.x
- An Azure account
- Installed Azure CLI, Azure ML SDK, and dependencies
