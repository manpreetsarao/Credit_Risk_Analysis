# Credit_Risk_Analysis
## Overview of the Analysis
In this analysis, we want to predict best machine learning model for credit card risk. we used different supervised machine learning models to predict the target values. To evaluate the results we used confusion matrix, accuracy score and imbalanced classification report. 
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

To find the best fit model, we used ensemble classifer and resampling model techniques. For first four models we used undersampled, oversampled  and did a combination of both. The next two models ensemble classifiers to try and predict which loans are high or low risk. The accuracy score for first four models is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Overall,  models  with a good balance of recall and precision are the ensemble classifiers. The best one is  the Easy Ensemble had the best balance of all the models because of it has high accuracy score and good balance of precision and recall scores.

