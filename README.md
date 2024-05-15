# Week 20 Challenge - Credit-Risk-Classification

<img src="ReadMe Pics/Pic 12.png" width="648" height="391">

In this Challenge, we were challenged to utilize a supervised machine learning model to evaluate loan risk. A dataset of historical lending activity from a peer-to-peer lending services company was provided to build a model that can identify the creditworthiness of borrowers.   


## Split the Data into Training and Testing Sets

### Read `lending_data.csv` data into a Pandas DataFrame.

 The data was read into a Pandas DataFrame for analysis.  
<br>
<img src="ReadMe Pics/Pic 1.png" width="858" height="167">

<br>


The “loan_status” column was removed from the DateFrame and it was placed in its own DataFrame resulting in two standalone DataFrames of data.  The two Dataframes can be viewed below. 

<br>
<img src="ReadMe Pics/Pic 3.png" width="785" height="155">
<img src="ReadMe Pics/Pic 2.png" width="299" height="136">


## Create a Logistic Regression Model with the Original Data

### Fit a logistic regression model by using the training data.

The data in the two Dataframes were portioned into groups that were used to train and test the logistic regression model.  The data was the fit to the model and predictions were tabulated. The resulting data comparing predicted and actual results was read into a DataFrame for further examination.  

<img src="ReadMe Pics/Pic 16.png" width="390" height="42">

<br>

<img src="ReadMe Pics/Pic 4.png" width="202" height="277">
<br>



## Evaluate the model’s performance

### Generate a confusion matrix.


<br>
<img src="ReadMe Pics/Pic 5.png" width="317" height="74">

### Print the classification report.

<img src="ReadMe Pics/Pic 6.png" width="452" height="181">
<br>

## Credit Risk Analysis Report
### Overview of the analysis





### The results

The confusion matrix results show:
<br>
* 18,679 individuals were correctly identified as credit worthy (True Negative)
* 558 individuals were correctly identified as not credit worthy (True Positive)
* 67 individuals that were incorrectly identified as not credit worthy (False Negative)
* 80 individuals were incorrectly identified as credit worthy (False Positive)

  
### Summary

