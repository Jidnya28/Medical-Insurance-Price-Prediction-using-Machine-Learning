# Medical-Insurance-Price-Prediction-using-Machine-Learning
This project focuses on predicting medical insurance charges based on customer attributes such as age, BMI, smoking habits, number of children, and region. The goal is to help insurance companies estimate policy costs accurately and understand the key factors affecting insurance premiums using machine learning.
2️⃣ Problem Statement
Insurance companies often struggle to price policies fairly and accurately due to multiple influencing factors like lifestyle and health indicators.
Problem:
Given customer demographic and health-related data, predict the expected medical insurance charges.
This is a regression problem where the target variable is continuous (charges).
🔹 Why I Used Linear Regression

I first applied Linear Regression as a baseline model to understand the linear relationship between features and insurance charges.

📌 How Linear Regression Works (Simple Explanation)

<img width="776" height="124" alt="image" src="https://github.com/user-attachments/assets/04619168-127b-481f-9037-55fb7607581a" />

📌 Steps I Followed

Split data into train and test sets

Trained Linear Regression model

Evaluated using R² score and cross-validation

📌 Results & Observation

Linear Regression gave moderate accuracy

It failed to capture non-linear relationships

Underperformed for smoker vs non-smoker patterns

“Linear Regression was used as a baseline model, but it could not capture complex non-linear relationships in insurance data.”
