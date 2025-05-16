# challenge_ds

# Dear Candidate
Thank you for your interest in participation in Mercado Libre's Data Science selection process. This is a challenge of 5 independent exercises. They go from exploratory data analysis to machine learning techniques. The challenge aims at any seniority level. The results are analyzed according to the candidate's level and particular needs of the position.

# Goals
The challenge aims to assess the following aspects:
- Analytical skills and data exploration.
- Data visualization of results.
- Techniques of data preparation, features extraction and modeling.
- Applied machine learning (classification, regression, outlier detection).
- Ability to deal with unclear scenarios.

# Rules and Tips
- You have 7 days to deliver the results.
- You do not have to work on all the problems.
- We expect you to work on at least 3 excercises.
- Preferably use Jupyter Notebooks to deliver your solution.
- Share your solution with us through a private GitHub repository.

# Excercises
## 1. Data Visualization
Use the iris dataset for this exercise:
**from sklearn.datasets import load_iris
iris = load_iris()**
- Create a Pandas dataframe from the dataset.
- Print a table with the feature_names as column names, plus variety.
- Print statistics of the features (max, min, avg, etc.).
- Plot a graph showing the relationship between petal width and length.
- Plot a graph showing the relationship between sepal width and length.
- Add colors to point the variety (Virginica, Setosa, Versicolor) of each feature (width, length).
- Add any other graph you find useful to see how to split the data in categories.
- Write down comments supporting your thoughts.

## 2. Finding Similarities
Given the dataset people.csv, create a similarity measure between the people. Take in consideration that your resulting calculation could be used in a posterior data model.
- ID, Name, Surname and E-mail address do not matter for the measurement.
- Nulls in any record invalidates that record.
- Since Salary has a wide range, it requires some kind of treatment before use.
- You are free about how to treat Gender.
- Print the full name of the closest people in the dataset along with the measure you created.
