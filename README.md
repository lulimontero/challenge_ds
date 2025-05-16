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

## 3. Machine Learning Classification
Given the dataset people.csv, create a KNN model to predict if a person is married or not:
- Nulls in any record invalidates that record.
- What value of K you choose? Why?
- Print a graph showing the best values of K related to the accuray.
- Print the accuracy of the model.
- Is the accuray satisfactory? Why?
- What features do you think could be added to increase the accuracy? Please explain your thoughts.
- Which features contributed the least to the model? Support your answer by showing concrete evidence in your notebook.

## 4. Machine Learning Regression
Given the dataset regression.csv, create a predictive model for the target variable **y** defined by: **y = count / max(count)**
  import pandas as pd ; 
  df = pd.read_csv('regression.csv') ;
  df["y"] = df["count"] / df["count"].max()
- To get an understanding of the periodic patterns of the data, have a look at the count variable per hour during a week.
- Since the dataset is a time-ordered event log (hourly demand), use a time-sensitive cross-validation splitter to evaluate the model.

## 5. Outlier Detection
A group of customers bought the lastest generation of a smartwatch released by a technology company. The smartwatch keeps track of user activities on a daily basis and the collected information is sent to cloud servers. For this excercise, you will explore a dataset of user behavior activites (ueba.csv) collected in February 2023.
import pandas as pd ; 
df = pd.read_csv('ueba.csv', parse_dates=['timestamp']) ;
- Create visualizations to identify patterns in the data.
- Try to apply an outlier detection estimator to find users that exhibit unusual behavior compared to the population.
