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
