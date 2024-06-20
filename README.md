# Maternal Health Monitoring System (CTRL)

## Introduction and Motivation
Maternal mortality remains a critical issue in the African Region, where it accounted for 69% of global maternal deaths in 2020. Despite global improvements, the maternal mortality ratio (M.M.R.) in Africa remains alarmingly high due to factors such as inadequate healthcare access, delayed interventions, and insufficient skilled personnel. This project aims to address these challenges by developing an innovative maternal health monitoring system using IoT, machine learning (ML), and mobile technology.


## Problem Statement
Traditional prenatal care methods often fail to detect life-threatening complications early enough, contributing to high maternal mortality rates in Africa. Limited access to quality healthcare services and a shortage of skilled professionals further exacerbate the problem. This project seeks to mitigate these issues through continuous monitoring, early risk detection, and personalized healthcare recommendations.


## Project Objectives
- `Design and develop an IoT wearable:` Monitor vital signs (blood pressure, heart rate, etc.) and fetal health parameters continuously.
- `Implement machine learning algorithms: `Analyze real-time data for early detection of complications like preeclampsia and gestational diabetes.
- `Develop a mobile application: `Provide real-time health monitoring, personalized advice, and educational resources for expectant mothers.
- `Integrate with healthcare provider interface`: Enable remote monitoring and timely intervention for high-risk cases.
- `Ensure data security and privacy:` Implement robust measures to protect patient data and integrate with existing healthcare systems.


## Technical Requirements

### IoT Wearable Device Development
- Hardware Components: Microcontroller (e.g., Arduino, ESP32), sensors (heart rate, blood pressure, SpO2, thermometer), communication modules (BLE, Wi-Fi/GSM/LTE).
- Data Management: Cloud-based databases (Amazon RDS, Google Cloud Firestore), edge computing for data preprocessing.

### Machine Learning Algorithms and Models
- Data Analysis: Time series analysis, classification algorithms (Random Forest, SVM), deep learning models (LSTM, GRU) for predictive analytics.
- Model Deployment: TensorFlow, PyTorch for training; AWS SageMaker, TensorFlow Lite for deployment.

### Mobile Application Development
- Framework: Flutter for cross-platform development (iOS and Android).
- Features: Real-time monitoring, personalized recommendations, notifications, educational resources, telehealth integration.
- Backend Integration: RESTful APIs, GraphQL for communication, data security (TLS, OAuth2.0).

### Data Privacy and Security
- Encryption: End-to-end encryption (AES-256) for data transmission and at rest.
- Access Control: Role-Based Access Control (RBAC), audit trails for data access and changes.

## About Dataset
### Context

Data has been collected from different hospitals, community clinics, maternal health cares through the IoT based risk monitoring system.

- Age: Age in years when a woman is pregnant.
- SystolicBP: Upper value of Blood Pressure in mmHg, another significant attribute during pregnancy.
- DiastolicBP: Lower value of Blood Pressure in mmHg, another significant attribute during pregnancy.
- BS: Blood glucose levels is in terms of a molar concentration, mmol/L.
- HeartRate: A normal resting heart rate in beats per minute.
- Risk Level: Predicted Risk Intensity Level during pregnancy considering the previous attribute.


## How to use the project
In order to run the model localy on your machine, please follow the following steps to get started


# Findings about the data
For the start, the data consisted of the following attributes
- Age
- SystolicBP
- DiastolicBP
- BS
- BodyTemp
- HeartRate
- RiskLevel

The data was then cleaned and preprocessed to remove any missing values and outliers. The data was then split into training and testing sets. The model was then trained on the training set and tested on the testing set. The model was able to predict the risk level of the patient with an accuracy of 0.85. The model was then saved and can be used to predict the risk level of a patient given the input data.

## changing the Categorical Data to the numerical data
During the Data preprocessing, the categorical data was converted to numerical data. The Risk Level was converted to numerical data as follows:

- low risk: 0
- mid risk : 1
- high risk: 2

##outliers in the data
During the Data preprocessing, We noticed a few outliers in the data. Most of the outliers came from the age attribute. We noticed that there we ladies with the age of 10 that were pregnant. We decided to remove these outliers.


## Modeling
In the modeling section, we used two models,
- We built a custom model using Tensorflow and Keras
- We also built another model using the scikit-learn library (Decision Tree Classifier)

The model was trained on the training set and tested on the testing set. The model was able to predict the risk level of the patient with an accuracy of 0.85. The model was then saved and can be used to predict the risk level of a patient given the input data.

## Conclusion
The project was able to predict the risk level of a patient given the input data. And we Decided to move on with the Decision Tree Classifier model. The model was able to predict the risk level of the patient with an accuracy of 0.85. The model was then saved and can be used to predict the risk level of a patient given the input data.

