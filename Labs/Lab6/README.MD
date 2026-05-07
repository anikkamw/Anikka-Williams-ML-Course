Lab 6: Regression and Classification Models

Overview: This lab established the fundamental distinction between Regression (predicting continuous values) and Classification (predicting discrete categories) using the Titanic dataset.
What I Learned: I practiced building a Linear Regression model to predict passenger Fares based on Class and Age, and a Logistic Regression model to predict Survival probability based on Age, Class, and Sex.
What I Did: I implemented evaluation metrics for both tasks, using Mean Squared Error (MSE) for the fare prediction ($58.01 average error) and Accuracy Score for the survival classification (74.83% accuracy).
Challenges: A key challenge was interpreting the .coef_ attribute; I learned that negative coefficients in my regression model indicated that as passenger Class or Age increased, the predicted Fare tended to decrease.
