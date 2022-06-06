# Credit_Risk_Analysis

## Overview

For this project, we are being asked by a fictional company to use supervised machine learning to create a model to predict the risk level for credit cards applicants. We will use six different kinds of models, two oversampling techniques, an undersampling technique, a combined technique, and two imbalanced techniques, and then see if there is a model that is reliable enough to apply to credit card applicants.  

## Results

###### Naive Random Oversampling

Balanced Accuracy: 
![image](https://user-images.githubusercontent.com/98666269/172079358-1216154d-06cf-4627-bbbd-435488ef0dc4.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172079551-141ca459-69db-418c-9bbd-dc3acd5dbed1.png)

Our balanced accuracy for the model with this seed is sitting at around 65%. Our low risk scores are fine, with 100% precision and 68% recall. Our precision for high risk clients is a measly 1%, and a slightly lower 62% recall. The accuracy is 68%, so the balanced accuracy score is close.

###### SMOTE Oversampling

Balanced Accuracy: 

![image](https://user-images.githubusercontent.com/98666269/172080444-900af79c-9752-48a9-b70f-f07d220eaa5b.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172080472-0e5a438d-dd4a-4e13-b193-cee92fe02cd9.png)

This is a worse model than previous, as our balanced balanced accuracy score is lower at around 62%. Although the precision is the same for both the high and low risk clients, the recall is lower for both at 59% and 66% respectively.

###### Undersampling

Balanced Accuracy: 

![image](https://user-images.githubusercontent.com/98666269/172082254-4635672e-4e74-458a-b619-f3fee7f0f455.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172082988-1d3f9166-da14-46ef-9ee6-c3de99779a23.png)

For this model, our balanced average is roughly 59%. Our precision is the same for both high and low risk clients, but the recall scores are swapped compared to our previous models. This time around, the high risk recall is higher than our low risk recall. The high risk is catching 61% of positive cases, while our low risk is only at 57%.



## Summary
