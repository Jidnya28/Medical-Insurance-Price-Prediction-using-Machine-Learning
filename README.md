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
(I used 5-fold cross-validation using cross_val_score. The dataset was divided into 5 folds, and the model was trained on 4 folds and tested on 1 fold iteratively. I took the average R² score to evaluate model performance. This helped me ensure the model generalized well and avoided overfitting)

(“I used R² for model comparison because it explains variance and helps detect overfitting. RMSE can definitely be used as a complementary metric to understand error magnitude in real currency terms.”)(“In a production scenario, I would report both R² and RMSE—R² for model performance and RMSE for business impact.”)

📌 Results & Observation

Linear Regression gave moderate accuracy

It failed to capture non-linear relationships

Underperformed for smoker vs non-smoker patterns

“Linear Regression was used as a baseline model, but it could not capture complex non-linear relationships in insurance data.”


🔹 Why I Used Random Forest

Since insurance pricing depends on non-linear interactions, I used Random Forest Regressor, which is an ensemble learning technique.

📌 How Random Forest Works (Simple Explanation)

Builds multiple decision trees

Each tree predicts independently

Final output = average of all tree predictions

Reduces overfitting compared to a single decision tree

🔹 Random Forest – Implementation Steps

Trained Random Forest Regressor

Evaluated using R² score and cross-validation

Tuned hyperparameters using GridSearchCV

Identified important features

<img width="831" height="316" alt="image" src="https://github.com/user-attachments/assets/5dfd6a48-33f7-4138-b8f6-b993d3210b70" />

“Random Forest helped me identify important features, allowing me to remove less impactful variables and improve performance.”

