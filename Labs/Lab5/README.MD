Lab 5: Data Preparation & Preprocessing

Overview: This lab focused on the critical stage of Data Preparation, transforming raw data into a format suitable for machine learning models.
What I Learned: I implemented imputation techniques using the median to handle missing 'Age' values and utilized StandardScaler to normalize numerical features like 'Fare' and 'Age'.
What I Did: I also performed One-Hot Encoding on categorical variables like 'Sex' and 'Embarked' using pd.get_dummies() to ensure the model could process non-numeric data.
Challenges: A key challenge was deciding when to use the median versus the mean for imputation; I concluded that the median is more robust against outliers in the Titanic dataset.
