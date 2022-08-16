### Credit Risk Analysis 

### Overview
#### A lending company has requested assistance in analyzing their loan data to determine the risk of various loans. Their desire is to predict loans that will be either high risk or low risk based on other known metrics of the borrowers. To make these predictions, this analysis utilized several machine learning techniques to create different models to predict risk. By developing different models, the team at the lending company can decide which models are most appropriate for their use. Python offers several machine-learning modeling techniques through scikit-learn and imbalanced-learn libraries including oversampling, undersampling, combination sampling, random forests, and boosting. All of these models take in a portion of the provided data, train a model to analyze the data, and then test the model using the remaining data from the dataset to determine the model's accuracy. The various modeling conducted led to differing results as explained in this analysis.

### Resources
### Data Source: LoanStats_2019Q1.csv

### Software: Python 3.7.6; Anaconda 4.10.3; 


## Credit Risk Analysis Results
#### Below are the balanced accuracy scores and precision and recall scores for the various models utilized for this analysis:
*For the Random Oversampling model, the balanced accuracy score was 0.66. The precision score was 0.99 and the recall score was 0.62.



*The SMOTE Oversampling method created a balanced accuracy score of 0.65, a precision score of 0.99, and a recall score of 0.68.




*The undersampling model resulted in a balanced accuracy score of 0.54, a precision score of 0.99, and a recall score of 0.40.




*A combination of oversampling and undersampling showed a balanced accuracy score of 0.64, a precision score of 0.99, and a recall score of 0.57.




*Using the BalancedRandomForest classifier led to a balanced accuracy score of 0.79, a precision score of 0.99, and a recall score of 0.87.




*Finally, the Easy Ensemble AdaBoost classifier showcased a balanced accuracy score of 0.93, a precision score of 0.99, and a recall score of 0.94.







## Credit Risk Analysis Summary
The balanced accuracy score for the models indicates how accurate each model was at determining the risk of a borrow. The precision score evaluates how reliable a model is at providing a positive classification. Lastly, the recall score (or sensitivity score) measures how consistent a model is at providing true positive and false negative classifications of a dataset. All scores play a part in determining the effectiveness of a model in predicting the targeting feature, however recall is more important in determining high risk loans. Based on the models ran for the loan data, the Easy Ensemble AdaBoost would be the most recommended model for the lending team to use. 


While all models had a precision score of 0.99, the Easy Ensemble classifier showed an accuracy score of 0.93 and a recall score of 0.94. Undersampling and combination over- and undersampling showed the worst recall and accuracy scores and should likely not be considered for the lending companyÕs uses. The BalancedRandomForest classifier had a relatively high accuracy score and recall score; however, the metrics of Easy Ensemble are significantly better than those displayed by BalancedRandomForest. 


