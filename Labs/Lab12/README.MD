Lab 12: Ethics, Fairness, and Bias in ML

Overview: This lab focused on auditing machine learning models for Algorithmic Bias to understand how models can inherit and amplify societal inequalities.
What I Learned: I practiced "Fairness Auditing" by comparing model performance across different demographic groups (sex and race) using the Adult Income dataset.

What I Did: I trained a baseline Logistic Regression model and calculated subgroup metrics. While the overall accuracy was 84.61%, I discovered a significant "Disparate Impact": the model had a False Negative Rate of 47.84% for females, nearly 10% higher than for males, meaning it was much more likely to incorrectly predict low income for qualified women.

Challenges: The most insightful challenge was the "Mitigation Paradox"—I learned that simply removing a sensitive feature like "Sex" doesn't fix bias because other features (like occupation or relationship status) act as proxies that the model can still use to learn biased patterns.
