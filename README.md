# fraud-detection
a classification model that predicts fraud in an organisation
BACKGROUND
Blossom Bank also known as BB PLC is a multinational financial services group, that offers retail and investment banking, pension management, asset management and payments services, headquartered in London,UK.
PROBLEM
Blossom Bank wants to build a Machine Learning model to predict online payment fraud.

SOLUTION
Obviously, the financial institution is experiencing occasional fraudulent transactions and they intend to prevent such occurrences. The development of this machine learning model, when deployed into the bank application will  assist to predict a transaction that will end as a fraudulent activities, and appropriate care such as Flags can then be raised to monitor such transactions.

The solution being proffered will enhance customer trust and confidence in the bank. This will result in the improved profitability of the organization as more customers will troop into the company.

The following activities were taken in sequence in developing the model
 
Step1: Loaded the dataset into pandas library
Step 2: Checked the dataset information 

Step 3: Confirmed the presence or absence of null values in the datasets
Step 4: Checking different datatype column
Step 5: Exploratory data analysis was performed on the data to understand the data more
These include the following: 
a.	Univariate graphs were explored using matplotlib and seaborn libraries
b.	Multivariate graphs were explored using matplotlib and seaborn libraries
Step 6:  Checking the data correlation among columns
Step 7 : Encoding Type data (Categorical value) into numeric data
Step 8: Feature engineering was performed, resulting in dropping of irrelevant data
Step 9: Splitting data (Making train dataset to be 80% and test data to be 20%)
Step 10: Building the Model, RandomForestClassifier and NaiveBayes classifiers were used
Step 13: Evaluating our model by checking for Accuracy, F1 score and Confusion Matrix



CHALLENGES FACED
SVM algorithm was observed to be very slow in model classification. It wasted my time as I didn’t know it does not have capacity for large dataset. I was bent on using it as it is very common.

OUTPUT
RandomForest outperformed NaiveBayes in Accuracy and F1 score. The accuracy of Randomforest was 99.97% whereas NaiveBayes was 57.1. For the F1 score, RF had a value of 89.84% while NB had a poor 0.4% value. 
Using the confusion matrix of evaluation showed that True Positive, representing prediction
 that was said to be positive and were truly positive was 209,471 predictions out of the 209,714 total predictions, this is a good development. Just 3 predictions were expected to be fraudulent, but were eventually found to be false. 199 predictions were expected not to be fraudulent, and it was so. 42 predictions were expected not be fraudulent, but were later found 
to be fraudulent. 45 wrong predictions were made in total when RandomForest classifier was used on the data this represents just about 0.03% inaccuracy. This percentage is negligible and the model is hereby recommended for deployment. Naivebayes however incorrect prediction amounting to almost 43%.  

http://localhost:8888/notebooks/capstone.ipynb
