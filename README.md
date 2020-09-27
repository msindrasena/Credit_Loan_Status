# Credit Loan Status

## In this project, we built machine learning models and analyzed whether we should accept or reject a person's credit card loan based on a number of factors. 

We used Precision, Recall (Sensitivity), and a Balanced Accuracy Score to make these decisions. 
The Precision Score, or Positive Predicted Value is looking at how reliable a positive classification
is by taking the true positives and dividing it by the total of all positives (both true and false positives). 
The recall, or sensitivity score looks at the positives that were correctly identified. This is calculated
by taking all the true positives and dividing it by the true positives + false negatives. Lastly, the 
Balanced Accuracy Score looks at the average of recall on each class. 


## Oversampling with Naive Random Oversampling and SMOTE

The oversampling with Naive Random Oversampling and SMOTE provided similar results.
The precision for high-risk and low risk was .01 and 1.00, respectively- for both models.

The recall rate for NRO was .69 for high-risk and .61 for low risk.
The recall rate for SMOTE was .63 for high-risk and .69 for low risk.  

The F1 score for NRO was .02 for high-risk and .76 for low risk.
The F1 score for SMOTE was .02 for high-risk and .82 for low-risk. This makes us think the model
is good at predicting low-risk applicants but not amazing at predicting high-risk applicants. 

The balanced accuracy score was around 65-66%.

## Undersampling

I used the Cluster Centroids algorithm to decrease the size of the majority class. The
precision rate was .01 and 1.00 for high and low risk respectively. The recall rate was .68 and 
.41 for high and low risk. The F1 rate was .01 and .58 respectively.
These are very similar to the oversampling models used. The balanced accuracy score was around 55%. 

## Combination Sampling with SMOTEENN
This model projected similar results to our last two models. The precision rate for high and low 
risk was .01 and 1.00. The recall rate was .72 and .57 respectively, which was the highest
in all of the models for both high and low risk applicants.  The balanced accuracy score 
was around 64%. The F1 Score was very low for high-risk and high for low-risk (.72), making us 
believe again that the model is good at predicting low-risk but not as good at predicting
high-risk applicants. 

## Recommendations

We also tested the Easy Ensemble AdaBoost Classifier, which turned out with the highest precision 
rate and also the highest recall and balanced accuracy score (92%). I believe this model will do a 
better job at determining who is a low-risk and high-risk applicant.
