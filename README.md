# Customer Churn Prediction Project

The Customer Churn Prediction project is designed to predict customer churn using a machine learning model deployed via a Flask API. This project helps businesses identify customers who are likely to leave, allowing for proactive retention strategies.

## Table of Contents

- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [Request Format](#request-format)
- [Response Format](#response-format)
- [Error Handling](#error-handling)

## Project Overv
### Objective

The primary objective of this project is to predict customer churn based on historical customer data. The project consists of two main components: a machine learning model and a Flask API for model deployment.

### Components

1. **Machine Learning Model**: This component involves the training and evaluation of a machine learning model using historical customer data. The model is designed to predict whether a customer is likely to churn or not.

2. **Flask API**: The Flask API serves as an interface to the machine learning model. It allows users to send customer data and receive churn predictions in real-time.

## Getting Started

### Running the API
To run the Flask API, execute the following command:

python app.py


By default, the API runs on http://localhost:5000.

### API Endpoints

Predict Endpoint
URL: /predict
Method: POST
Description: Make predictions using the pre-trained machine learning model.

### Request Format
Input Data
The input data should be provided in JSON format with the following fields:

CustomerID: The unique identifier for the customer.
Name: The customer's name.
Age: The age of the customer

### Response Format
The API response will be in JSON format and will include churn predictions.

Example Response:

{
    "predictions": [0, 1, 0, 0, 1]
}

### Error Handling
In case of any errors, the API will return an error message in JSON format.

Example Error Response:

{
    "error": "Invalid input data."
}
