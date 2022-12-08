# Credit_Risk_Analysis
## Overview of the Analysis
In this project, we want to look at how all the factors in our loan states csv helps predict whether someone is low or high-risk status. In this analysis, we used different supervised machine learning models to predict the target values. We used different methods to find out the best model for prediction. To evaluate the results we used confusion matrix, accuracy score and imbalanced classification report. 
The Purpose of this analysis, to compare the output of different machine learning models to find the best one for prediction. 
## Results
### OverSampling
-	#### Navie Random 
  The  balanced accuracy for this model is 64%, the average precision is 99% and average recall is 60%.
![Screenshot_20221208_110240](https://user-images.githubusercontent.com/111101038/206549841-88faeefc-b577-4e53-912d-46212eb9b53d.png)

-	 #### SMOTE 
 The  balanced accuracy for this model  is 66%, the average precision is 99% and average recall is 69%.
![Screenshot_20221208_110456](https://user-images.githubusercontent.com/111101038/206549874-04bd777e-32ec-4249-8fc9-03386771ed39.png)


### Undersampling
-	#### Cluster Centroids 
TThe  balanced accuracy for this model  is 54%, the average precision is 99% and average recall is 40%.
![Screenshot_20221208_110535](https://user-images.githubusercontent.com/111101038/206549932-48baa0cc-f634-4cbb-ac19-3dc9af368ad8.png)


### Combination (Over and Under)Sampling
-	#### SMOTEENN
The  balanced accuracy for this model is 54%, the average precision is 99% and average recall is 57%.
![Screenshot_20221208_110626](https://user-images.githubusercontent.com/111101038/206549976-98972983-ffdb-40ef-ad0a-a102d531b1bc.png)


### Ensemble Learners
-	#### Balanced Random Forest Classifer
The  balanced accuracy for this model is 78%, the average precision is 99% and average recall is 87%.
![Screenshot_20221208_110710](https://user-images.githubusercontent.com/111101038/206550007-85bac8dd-e6a4-4e76-9c9b-9b3348f87068.png)

-	#### Easy Ensemble AdaBoost Classifer
The  balanced accuracy for this model is 93%, the average precision is 99% and average recall is 94%.
![Screenshot_20221208_110748](https://user-images.githubusercontent.com/111101038/206550043-ccc0f1b5-6f27-490f-97b2-ec1419dbc2b3.png)

## Summary

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.

