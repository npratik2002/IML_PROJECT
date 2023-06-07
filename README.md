# IML_PROJECT
SVM implementation
import pandas as pd
from sklearn.datasets import load_iris
iris=load_iris()
dir(iris)
The line you provided performs the following actions:
It imports the pandas library and assigns it the alias pd.
pandas is a popular library in Python used for data manipulation and analysis.
It imports the load_iris function from the sklearn.datasets module.
sklearn (scikit-learn) is a widely used library for machine learning in Python.
It creates a variable named iris and assigns it the result of calling the load_iris function.
load_iris is a function provided that loads the Iris dataset, which is a popular dataset used for classificatio
n tasks.
The dir() function returns a list of names in the specified object. In this case,
it will return a list of names (attributes and methods) available in the iris object, allowing you to
explore and understand its structure and functionality.
df=pd.DataFrame(iris.data,columns=iris.feature_names)
The line you provided creates a Pandas DataFrame named df using the data from the Iris dataset.
pd.DataFrame() creates a new DataFrame object from the data passed as the first argument.
In this case, the data is iris.data, which represents the feature values of the Iris dataset.
The columns parameter specifies the column names for the DataFrame.
In this case, it is set to iris.feature_names, which represents the names of the features in the Iris dataset.
df[’target’]=iris.target
iris.feature_names
df[’target’] = iris.target
This line adds a new column named ’target’ to the DataFrame df. The values for this column are assigned
from iris.target
iris.feature_names
This line returns a list of feature names from the Iris dataset.
These feature names represent the column names that can be used to label the columns in the DataFram
e df.
Each feature name corresponds to a specific attribute of the iris flowers, such as ’sepal length’, ’sepal widt
h’, ’petal length’, and ’petal width’.
iris.target_names
df[’species’]=df.target.apply(lambda x:iris.target_names[x])
