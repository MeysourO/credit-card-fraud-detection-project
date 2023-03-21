# Credit-Card-Fraud-Detection-Project
**Meysour Omezzine**  
**IronHack, Paris 21 Mar 2023**

## Overview

* How we can Banks/Credit card companies predict fraudulent credit card transactions?  

Used:

	* Python
	* Statistical analysis
	* Data visualization
	* Jupyter Notebook
	* Tableau
	* Machine Learning (Logistic Regression)
  
  ## Data Preparation

### Overview: 
* Data is about Credit card transactions.
	* [https://www.kaggle.com/datasets/ealtman2019/credit-card-transactions]
  
* 15 columns 
* 19963 rows 
* columns:

  - User, 
	- Card,  
	- Year,  
	- Month, 
	- Day, 
	- Time,
	- Amount, 
	- Use chip,
	- Merchant Name,
	- Merchant city,
  - Merchant State,
	- Zip,
	- MCC,
	- Errors?,
	- Is Fraud?.
  
	### Data Wrangling and Cleaning
  
- Overall Data description
- Deleting  columns with hight unique values: User,Merchant Name,Zip 
- Looking for outliers column by column 
- Changing MCC to MCC Category: Check for each MCC number Category name and then group same categories fields together
- Changing Year and Day to Date
- Changing Time to Time period
- Changing Merchant City to Merchant Type : Online or In-person
- Dropping  with NaN values in columns Errors? and Merchant State
- Creating plots for each column to check where most fraudulent transactions occured.

### Data Storage

* Dump your data as `.csv` file. 

## Data Analysis
* Use tableau to analyze 
* 
### Data Exploration and Visualization
Used Tableau to visualize my overall data.

### Model Training and Evaluation
- Define predictors and target values (X, y)
- Standard scaling for numericals : for Train and Test set
- OneHotEncoding for categoricals : for Train and Test set
- Balancing data : Oversampling our target values in our Train set. 
- Model : LogisticRegression
- Compared accuracy 
- Confusion Matrix

## Conclusion

- Based on our Recall rate, our model can alert us on fraud transactions where transactions are actually frauds, how ever based on the confusion matrix it predicted some false positives. 
- Our model had an accuracy of 89%. 
 
