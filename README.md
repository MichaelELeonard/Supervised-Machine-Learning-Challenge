<img src="ReadMe Pics/Header.png" width="694" height="354">

# Supervised Machine Learning

[Supervised Machine Learning Code Link]( https://github.com/MichaelELeonard/credit-risk-classification/blob/main/Credit_Risk/credit_risk_classification_working.ipynb)

## Overview

In this challenge, we were tasked to utilize a supervised machine learning logistic regression model to evaluate loan risk. A dataset of lending activity from a peer-to-peer lending services company was provided to build a model that could identify the creditworthiness of borrowers.   


## Data Split into Training and Testing Sets

 The data was read into a DataFrame for analysis.  
<img src="ReadMe Pics/Original Data.png" width="858" height="167">

The “loan_status” column was removed from the DateFrame and it was placed in its own DataFrame resulting in two standalone DataFrames of data.  The two Dataframes can be viewed below. 

<img src="ReadMe Pics/Data Split 1.png" width="785" height="155">
<img src="ReadMe Pics/Data Split 2.png" width="299" height="136">


## Logistic Regression Model

### Logistic regression model fit to training data.

Data from the two DataFrames were portioned into training and testing groups for the logistic regression model.  The data was the fit to the model and predictions were tabulated. The resulting data comparing predicted and actual results was read into a DataFrame for further examination.  

<img src="ReadMe Pics/Logistic Regression.png" width="390" height="42">

<br>

<img src="ReadMe Pics/Prediction.png" width="202" height="277">


## Results

### Confusion Matrix


<img src="ReadMe Pics/Confusion Matrix.png" width="317" height="74">

### Classification report

<img src="ReadMe Pics/Classification Report.png" width="489" height="177">

## Credit Risk Analysis Report
### Overview of the analysis

In this challenge, we utilized a structured machine learning logistic regression model to evaluate the loan risk of borrowers.  This determination was based off a variety of factors.  These factors include: <br>
* Loan Size
* Interest Rate
* Borrower Income
* Debt to Income Ratio
* Number of Revolving Accounts
* Past Negative Credit Marks
* Total Debt

The logistic regression model was established, the provided original data was used to train the model, and a confusion matrix and classification report was run to evaluate the model’s performance.  



### The Results

The confusion matrix results show:
* 18,679 individuals were CORRECTLY identified as credit worthy (True Negative)
* 558 individuals were CORRECTLY identified as not credit worthy (True Positive)
* 67 individuals that were INCORRECTLY identified as not credit worthy (False Negative)
* 80 individuals were INCORRECTLY identified as credit worthy (False Positive)

The rows and columns were summed and compared to assess accuracy and precision.  Both aggregate totals were 19,384 so we can consider the model to be accurate and precise.

<img src="ReadMe Pics/Confusion Matrix Analysis.png" width="421" height="287">

The classification report results show:
* The accuracy of the entire model was 99%
* The precision for healthy loans was 100% 
* The recall for healthy loans was 100%
* The precision for high-risk loans was 87% 
* The recall for high-risk loans was 89%  

### Summary
Some trends can be observed when examining the performance of the logistic regression model.  Overall, the model performed exceptionally well with a 99% accuracy rate. The model excelled at identifying healthy loans, scoring a 100% success rate in precision and recall.  The model did drop off slightly when identifying high-risk loans, scoring 87% in precision and 89% in recall.  One potential reason for the drop off in the high-risk loans results may be due to the small sample size provided for the model, as it only accounted for 3.2% of the total data examined.  Increasing this sample size may provide greater learning opportunities for the model, thus boosting its performance.  It may also be prudent to expose this data to other machine learning models to see if the change affects the performance results.           
