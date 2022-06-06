# Credit_Risk_Analysis

## Overview

For this project, we are being asked by a fictional company to use supervised machine learning to create a model to predict the risk level for credit cards applicants. We will use six different kinds of models, two oversampling techniques, an undersampling technique, a combined technique, and two imbalanced techniques, and then see if there is a model that is reliable enough to apply to credit card applicants.  

## Results

##### Naive Random Oversampling

Balanced Accuracy: 

![image](https://user-images.githubusercontent.com/98666269/172079358-1216154d-06cf-4627-bbbd-435488ef0dc4.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172079551-141ca459-69db-418c-9bbd-dc3acd5dbed1.png)

Our balanced accuracy for the model with this seed is sitting at around 65%. Our low risk scores are fine, with 100% precision and 68% recall. Our precision for high risk clients is a measly 1%, and a slightly lower 62% recall. The accuracy is 68%, so the balanced accuracy score is close.

##### SMOTE Oversampling

Balanced Accuracy: 

![image](https://user-images.githubusercontent.com/98666269/172080444-900af79c-9752-48a9-b70f-f07d220eaa5b.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172080472-0e5a438d-dd4a-4e13-b193-cee92fe02cd9.png)

This is a worse model than previous, as our balanced balanced accuracy score is lower at around 62%. Although the precision is the same for both the high and low risk clients, the recall is lower for both at 59% and 66% respectively.

##### Undersampling

Balanced Accuracy: 

![image](https://user-images.githubusercontent.com/98666269/172082254-4635672e-4e74-458a-b619-f3fee7f0f455.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172082988-1d3f9166-da14-46ef-9ee6-c3de99779a23.png)

For this model, our balanced average is roughly 59%. Our precision is the same for both high and low risk clients, but the recall scores are swapped compared to our previous models. This time around, the high risk recall is higher than our low risk recall. The high risk is catching 61% of positive cases, while our low risk is only at 57%.

##### Combination Sampling

Balanced Accuracy:

![image](https://user-images.githubusercontent.com/98666269/172084573-7e6765fe-57c6-45b5-906d-fcbaa23c8bd8.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172084614-b698a181-11fa-41f8-a239-6a3eecce3c60.png)

We once again have a model at around 65% accuracy, but unlike our Naive Random Oversampling we're rounding up to get that number instead of rounding down. This is also above the average score in our classification report. Again, our precision remains the same for our high and low risk clients. Our high risk recall is the best score we have so far at 71%, while our low risk is near our worst with 58%.

##### Balanced Random Forest Classifier

Balanced Accuracy:

![image](https://user-images.githubusercontent.com/98666269/172085151-47436d1c-39f6-4e22-aab9-1fbfedff2476.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172085180-166bcf95-11f0-4f20-9eb8-d6aa35882541.png)

With our first imbalanced sorting, we see a much better model. The balanced accuracy is up to around 79%, with the precision of high risk clients up to 4% while still maintaining the 100% low risk precision. The recall for high risk is a respectable 67%, while low risk recall is the best we've seen at 91%.

##### Easy Ensemble AdaBoost Classifier

Balanced Accuracy: 

![image](https://user-images.githubusercontent.com/98666269/172085513-81324d72-cd98-4bfc-94c7-194685d35553.png)

Classification Report:

![image](https://user-images.githubusercontent.com/98666269/172085546-9a688b48-9d00-45d7-8e41-cc3fb93f4b28.png)

This is far and away our best model. The balanced accuracy is sitting at a nearly a whopping 93%. The precision for high risk is at 7%, while again our low risk stays at 100%. Our recall scores also incredible, with 91% for high risk and 94% for low risk. 

## Summary
