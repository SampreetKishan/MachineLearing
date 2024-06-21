
# Introduction
This is a repository that python scripts implementing several machine learning and/or statistical analysis models. 

Each folder within the root folder represents one machine learning model. 

## Linear Regression

### E-commerce website

We start off with a linear modeal(Linear regression). The dataset contains e-commerce information about yearly amount by a customer, time spent on the phone app, time spent on website, amount of time a customer spent in the store(session length), customer details. The objective is to determine whether time spent on phone app or time spent on the website was more important. 

We start off with ingesting the data into a dataframe. Then we do some exploratory analysis looking at the structure of the dataframe, looking at the mean, median, etc metrics of the numerical columns. 

Thereafter, we try to look at the correlation between different numerical columns. We do notice a pattern (see Jupyter notebook for more information). 

With this assumption in mind, we go ahead and start building our linear model. As customary practise, we split the data into training and testing datasets. Then we build a Linear Regression model on the training dataset. We then calculate the coefficients and intercept. We also determine the R^2 to make sure our model did well. For further testing, we run our model against the test data and compare them against the test data's true values. We then see how well our model performs against the test data using Mean squared error, mean absolute error. Additionally, we plot the test values against the predicted values to make sure they follow each other nearly 1:1 linearly.

 Lastly, we do an analysis on the residuals to ensure that the residuals fit a normal distribution to make sure our data/analysis doesn't have any bias one way or another.    
