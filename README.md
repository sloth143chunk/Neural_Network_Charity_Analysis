# Neural Network Charity Analysis

## Overview

-	The purpose of this analysis is to be able to predict whether applicants will be successful if funded by Alphabet Soup.  


## Results

-	Data Preprocessing
-	The column “Is_Successful” is the target variable

-	The features for this model are the columns: Name, Application_Type, Affiliation, Classification, Use_Case, Organization, Status, Income_Amt, Special_Considerations, Ask_Amt

-	The column “Ein” is neither a target nor feature and needed to be removed

-	Compiling, Training, and Evaluating the Model
-	I tried to increase the neurons to help improve the accuracy but found that adding a third layer and increasing the neurons increased the accuracy above 75%.  The first activation was kept as ‘relu’ and the third activation function was made ‘sigmoid’ also helped boost the accuracy to close to 80%.

-	The target model performance of 75% or higher was achieved.

-	I started by increasing the neurons and dropping different columns to try and increase the model performance.  I found adding the ‘NAME’ column and increasing the layers and neurons and changed the second activation function to ‘sigmoid’.


## Summary

By increasing the accuracy to be above 75% we are able to classify each points in the test data.  An applicant has an 80% chance of being successful if they:

-	The NAME of the applicant appears more than 5 times (they have applied more than 5 times) 
-	The type of APPLICATION is one of the following; T3, T4, T5, T6, T7, T8, T10, and T19 
-	The application has the following CLASSIFICATION; C1000, C2000, C3000, C1200, and C2100.
	
Another good model for classification problems is the Random Forest model.  This model produces a 78% accuracy.

## Resources
- Data Source: charity_data.csv
- Software: Jupyter notebook, Machine Learning Environment
