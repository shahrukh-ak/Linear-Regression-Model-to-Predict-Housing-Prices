# Linear-Regression-Model-to-Predict-Housing-Prices

## BUSINESS PROBLEM
<br>
A real estate agent wants some help to predict housing prices for regions in the USA. It would be great if you could somehow create a model for her that allows her to put in a few features of a house and returns back an estimate of what the house would sell for.
<br><br>
She has asked you if you could help her out with your new data science skills. You say yes, and decide that Linear Regression might be a good path to solve this problem!
<br><br>
She gives you some information about a bunch of houses in regions of the United States,it is all in the data set: USA_Housing.csv.
<br><br>
The data contains the following columns:
<br><br>
'Avg. Area Income': Avg. Income of residents of the city house is located in.<br>
'Avg. Area House Age': Avg Age of Houses in same city<br>
'Avg. Area Number of Rooms': Avg Number of Rooms for Houses in same city<br>
'Avg. Area Number of Bedrooms': Avg Number of Bedrooms for Houses in same city<br>
'Area Population': Population of city house is located in<br>
'Price': Price that the house sold at<br>
'Address': Address for the house<br>

Let's get started!

## EDA
Created some simple plots to check out the data!

![1](https://user-images.githubusercontent.com/55116845/122211876-a60f5f00-cec0-11eb-9cf0-15f6370fa38e.png)

![2](https://user-images.githubusercontent.com/55116845/122211905-af98c700-cec0-11eb-9332-3d72ff9a5d7b.png)

![3](https://user-images.githubusercontent.com/55116845/122211939-b6bfd500-cec0-11eb-8de6-9f39aeb897ef.png)

## Training a Linear Regression Model

Train regression model! Splited the data into an X array that contains the features to train on, and a y array with the target variable, in this case the Price column. Toss out the Address column because it only has text info that the linear regression model can't use.

## Model Evaluation

Evaluated the model by checking out it's coefficients and how they can be interpreted.

![T1](https://user-images.githubusercontent.com/55116845/122212427-3f3e7580-cec1-11eb-87c4-b4ca6a228668.PNG)

### Interpreting the coefficients:
<ul>
  <li>Holding all other features fixed, a 1 unit increase in Avg. Area Income is associated with an increase of \$21.52 .</li>
  <li>Holding all other features fixed, a 1 unit increase in Avg. Area House Age is associated with an increase of \$164883.28 .</li>
  <li>Holding all other features fixed, a 1 unit increase in Avg. Area Number of Rooms is associated with an increase of \$122368.67 .</li>
  <li>Holding all other features fixed, a 1 unit increase in Avg. Area Number of Bedrooms is associated with an increase of \$2233.80 .</li>
  <li>Holding all other features fixed, a 1 unit increase in Area Population is associated with an increase of \$15.15 .</li>
</ul>

## Predictions from our Model
Grab predictions off our test set and see how well it did by using different plots.

![4](https://user-images.githubusercontent.com/55116845/122213257-339f7e80-cec2-11eb-9ebe-e3cdcdf7071d.png)

### Residual Plot

![5](https://user-images.githubusercontent.com/55116845/122213423-5e89d280-cec2-11eb-8edb-33998321eedc.png)

## Regression Evaluation Metrics

Here are three common evaluation metrics for regression problems:
<br>
Mean Absolute Error (MAE) is the mean of the absolute value of the errors:<br>

![F1](https://user-images.githubusercontent.com/55116845/122213707-a9a3e580-cec2-11eb-9ded-6e6473d8b0d6.PNG)

Mean Squared Error (MSE) is the mean of the squared errors:

![F2](https://user-images.githubusercontent.com/55116845/122213936-ee2f8100-cec2-11eb-8e63-abfd5e0b2d7d.PNG)

Root Mean Squared Error (RMSE) is the square root of the mean of the squared errors:

![F3](https://user-images.githubusercontent.com/55116845/122214022-0dc6a980-cec3-11eb-937a-8d8c1ab5e4e2.PNG)

Comparing these metrics:
<br>
<ul>
  <li>MAE is the easiest to understand, because it's the average error.</li>
  <li>MSE is more popular than MAE, because MSE "punishes" larger errors, which tends to be useful in the real world.</li>
  <li>RMSE is even more popular than MSE, because RMSE is interpretable in the "y" units.</li>
</ul>
All of these are loss functions, because we want to minimize them.





