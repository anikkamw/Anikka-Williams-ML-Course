Lab 8: The Bias-Variance Tradeoff

Overview: This lab focused on understanding and visualizing Bias and Variance to determine how model complexity impacts the ability to generalize to new data.
What I Learned: I practiced using Polynomial Regression to create models of varying degrees (1, 4, and 15) to observe the effects of underfitting (high bias) and overfitting (high variance) on a synthetic sine wave dataset.
What I Did: I implemented Learning Curves using scikit-learn to diagnose model performance. I observed that my Degree 1 model suffered from high bias (plateauing at poor scores), while my Degree 15 model showed high variance by trying to "memorize" the noise in the data rather than the underlying pattern.
Challenges: A key challenge was interpreting the learning curve scores; I learned that when both training and cross-validation scores stay low (near zero), it indicates the model is too simple to learn the pattern, regardless of how much data is provided.
