Build a multi-class Logistic Regression model to predict categories of "crop" with a F1 score of more than 0.5.

Read in soil_measures.csv as a pandas DataFrame and perform some data checks, such as determining the number of crops, checking for missing values, and verifying that the data in each potential feature column is numeric.
Split the data into training and test sets, setting test_size equal to 20% and using a random_state of 42.
Predict the "crop" type using each feature individually by looping over all the features, and, for each feature, fit a Logistic Regression model and calculate f1_score(). When creating the model, set max_iter to 2000 so the model can converge, and pass an appropriate string value to the multi_class keyword argument.
In order to avoid selecting two features that are highly correlated, perform a correlation analysis for each pair of features, enabling you to build a final model without the presence of multicollinearity.
Once you have your final features, train and test a new Logistic Regression model called log_reg, then evaluate performance using f1_score(), saving the metric as a variable called model_performance.