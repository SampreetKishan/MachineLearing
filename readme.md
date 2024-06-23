
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


### Weather predictor

The dataset resides here: https://www.kaggle.com/datasets/budincsevity/szeged-weather. The goal of this exercise is to determine if apparent temperature is dependent on humidity. 

I took the liberty of ignoring non-numerical columns. I think went ahead and tried to find correlation between different variables. It seems like there is a correlation between apparent temperature and not only  humidity but also visibilty and temperature etc. 

Thus, I build one linear model where I assume there is a relationship between apparent temperature and other numerical variables including humidity. I obtain excellent values for R2, MSE, and MAS. Additionally, the residuals from this model form an almost perfect normal distribution.

Additionally, I build another linear model to see if apparent temperature depends only on humidity by ignoring the other numerical columns besides these days. I obtain mediocre values for R2, MSE, and MAS. Also, while, the residuals from the model form a decent normal distribution, they're not all shapely as the residuals from the first model. 