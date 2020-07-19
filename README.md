# Cradit-Fraud-Detection
The challenge is to recognize fraudulent credit card transactions so that the customers of credit card companies are not charged for items that they did not purchase.
## Dataset
The dataset consists of credit card transactions whose features are the product of PCA analysis and thus we don’t know what they represent except from the ‘Amount’, ‘Time’ and ‘Class’ ones.There were no missing values in the data set. Class represents a fraud transaction when its value equals 1 and a valid transaction when its value equals 0. 
## Exploratory Data Analysis (EDA)
We see that our data is highly imbalanced. Therefore, we cannot use any supervised learning algorithm directly because it will overfit based on the ‘Normal’ examples.In fact, 99.83% of the transactions in this data set were not fraudulent while only 0.17% were fraudulent.
### SMOTE Technique (Over-Sampling):  
SMOTE stands for Synthetic Minority Over-sampling Technique.SMOTE creates new synthetic points in order to have an equal balance of the classes. This is for solving the "class imbalance problems".
## Classifications Algorithms
To be able to test the performance of our algorithms, I first performed an 80/20 train-test split, splitting our balanced data set into two pieces. Then used XGBoost Classifier approach in order to achieve a higher degree of comprehensiveness while only slightly decreasing performance.
## End Note
Implementing SMOTE on our imbalanced dataset helped us with the imbalance of our labels (more no fraud than fraud transactions) and by using XGBoost algorithm we acquire 99% of accuracy. 

This Code is prepared using jupyter notebook.
