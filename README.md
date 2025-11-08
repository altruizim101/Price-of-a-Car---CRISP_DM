# Price-of-a-Car---CRISP_DM

## (Goal & Objective)
# - Business Understanding: The Task -
# 
Make use and analyze past vehicle data to determine what factors drive the price of a used car. 
Build and develop a predictive model that estimates the price of a used car based on factors (such as Make, Model,...)
and highlight the most important factors to better inform the car dealership in setting competitive prices and boost sales.


Data Source:
- CRISP-DM Overview:   [https://classroom.emeritus.org/courses/13354/assignments/351342?module_item_id=2656622]
- Used Car Dataset:   [(https://mo-pcco.s3.us-east-1.amazonaws.com/BH-PCMLAI-R2/module11/readings_starter.zip)]

## Deliverables
The final submission should include the Jupyter Notebook and other relevant files, such as the dataset provided and uploaded to a GitHub repository.

## Links to Project Deliverables
- READMe file with summary of findings >>  [https://github.com/altruizim101/Price-of-a-Car---CRISP_DM/blob/main/README.md]
- Link to Jupyter notebook here >>         [https://github.com/altruizim101/Price-of-a-Car---CRISP_DM/tree/main]
- Data Analysis & Results >>               [https://github.com/altruizim101/Price-of-a-Car---CRISP_DM/tree/main]

## Data Understanding & Cleaning
I checked for possible Null (NaN) values in data for removal before analysis. Then filtered NaN data as appropriate.
I cleaned and prepared numeric and categorical data accordingly.

## Analysis
I split data into train and test data sets. Using multiple Regression models, I evaluated the performace of each.
Regression models applied in this analysis include Linear, Lasso, and Ridge Regression models.

From the above results of these models, 
 1)  the performance are almost identical for the models.
 2)  the models explain only 10% of the variability in the price. This implies weak weak modeling.
 3) 90% of price variation is left unexplained by the models.

Next, applying cross-validation and scoring the models, we observed that the models explain the data with similar level of variability.
The R2 score and the Mean-score are comparable for the models.
Furthermore, the models explain only ~10% of the variability in the price. This implies weak weak models.
With these models unable to explain ~90% of the price, the relationship between Price and features is non-linear.
Non-linear techniques should be employed for this.

## Summary of findings & Reccommendations

From the above analysis of data provided in predicting the proice of a used car, our modeling tool was able to
only explain 10% of what causes price difference in used car sales.
This could imply buyers do consider other factors in used car purchase not captured in this data, such as
brand reputation of the Make/Model, service history of the vehicle, ...
Given these findings, additional details in data will be very useful in accuractely 
predicting the price of used car sales.
This dataset was insightful from the fact that factors to predict used car sales is not 
a linear relationship among these features in current data set.
In summary, we will need addtional details, or engineer new features using non-linear model technicques.
Further modeling and data analysis is required to present a more informed decision on used car pricing.
