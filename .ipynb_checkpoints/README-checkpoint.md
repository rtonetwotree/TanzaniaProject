# DS-Project-3
Flatiron School Data Science Project - Phase III

## Overview
* Purpose: To use predictive analytics to help solve the tanzanian water crisis by determing the primary factors in functional and non-functional wells
* Source of data: Sourced data from Taarifa & Tanzanian Ministry of Water
* Focus areas and consideration:
  * Primary Success Metrics: Source Basin, Water Point Type, payment type, years old
  * Others : region, management
* Data excluded - None
  *We did impute the values for any well that did not have a construction year with the average construction year

 
# Presentation and Sources
Presentation: [Link](https://docs.google.com/presentation/d/1TX8SpnVb1Cyu7uWYlujMT3me6SGN8nRktH8dX18GbBk/edit?usp=sharing)

Datasets: [Link](https://github.com/taarifa/TaarifaWaterpoints/tree/master?tab=readme-ov-file#waterpoints)


# Repository Navigation
Our Github Repository contains 2 jupyter notebooks in it. The first of those notebooks is titled LogRegModel+Cleaning and contains data cleaning and the logistical regression modeling. The second notebook is titled Decison_Tree_Analysis and contains the final model for the decision tree, which was the ultimate one we used for our recommendations. Also included in the repository is csvs containing all the data used to build the models. 

## Data Analysis & Recommendations

The first step we took was making the data more accessable and manipulatible by importing csv files and converting files into pandas dataframes. We then explored our data, looking at different summary statistics and sorting through the various features available to us for analysis in order to narrow down the dataset in to useful information only. We used a preliminary analysis of both the distribution of features as well as calculating a ratio of functional vs non functional wells for each feature to see which ones had the most impact.

Based off of our exploration we chose Basin, Payment Type, and waterpoint type as the three most important variables that contribute to box office success and this was confirmed by both the logistical regression and decision tree models we ran.

![Waterpoint_type](https://github.com/Keys2610/TanzaniaProject/assets/151547876/870d35e4-9d95-4efd-9c7c-209c46bf3404)

![Payment_Type](https://github.com/Keys2610/TanzaniaProject/assets/151547876/c990a442-51f1-4f73-9035-3f607639bb2e)






# Logistic Regression Model






# Decision Tree Model

*We spent some time tuning the model using various paramaters including splitter types, number of tiers, and minimum sample splits ultimately resulting in the following parameters: 

Entropy decision making type
Max Tree Depth of 35
Minimum sample split 3

This model was able to predict weather a well was funtional based on the feature set with over 75% accuracy.

![decision_tree](https://github.com/Keys2610/TanzaniaProject/assets/151547876/c9cb0da5-bdb0-4db9-804d-70ffdf543f35)




Our recommendations are the following: 

* Based on our intuition, EDA, and the modelling, we determined that the most successful wells are paid, hand pumps, and sourced from the Lake Nyasa basin.





