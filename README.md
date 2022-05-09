# CreditCardCompanyChurn

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Screenshots](#screenshots)
* [Usage](#usage)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)
<!-- * [License](#license) -->


## General Information
We have built a model that can correctly predict 6 out of every 7 customers who will churn. There are a few key takeaways from the features that are important to note: Customers are more likely to churn if they have a lower number of total transactions and total transactions amount, lower total revolving balance and lower average utilization ratio, and if they have less total company products (credit card accounts open). We have three recommendations that we believe will decrease churn rate and increase profits 

1. Reward customers with higher cashback rewards when customers reach a certain number of transactions per month. 

2. Offer different incentives for individuals who use above their average monthly credit balance. 

3. Offer incentives such as increased rewards for customers who have more than one company product. 

We believe that these recommendations are a great start to decreasing your churn rate based on the model that we have built. In the rest of this report, we will explain the problem faced, description and visualization of the dataset that we used, explain how we built our model and how it successfully solves the problem, and finally go more in depth into the recommendations we believe are very beneficial to your company. 

## Technologies Used
- R - v2022.02.2+485
- RStudio - v2022.02.2+485
- Rattle -	v5.5.1

## Screenshots
See folder "CCChurnModelReview" for screenshots of data interpretation.


## Usage
Data: This dataset consists of 10,000 customers with their age, salary, marital status, credit card limit, credit card category, and other information.  

Categoric Features: 6. Key examples - Income Category, Card Category, Gender, Education 

Numeric Features: 16. Key Examples - Total Revolving Balance,Total Transactions, Average Utilization Ratio, Age, Total Product Count (how many credit cards they have open with the company), Credit Limit 

We used all classification models such as gradient boosting, Ada boost, Logistic regression, random forest, and SVM. We did cross-validation with all models with random seeds 42, 294290, and 990998. We chose the best model by looking at the ROC curve and AUC and the lowest error provided by the error matrix. We also looked at the Precision-Recall curve because since our data was highly unbalanced, the AUC could be misleading. The best model was a gradient boosting model with an AUC of .9911 and an average error rate of 7.6%.  This model was also the best on the precision-recall curve.  
Error Matrix - (CCChurn9.png)

Target Variable: Attritted: We have only 16.07% of customers who have churned, which creates a highly unbalanced dataset. 

## Key takeaways from features 
Customers with lower number of transactions and lower total transactions amounts are more likely to churn (CCChurn1.png / CCChurn2.png ).  

Customers with lower total revolving balance and lower average utilization ratio are also more likely to churn. (CCChurn3.png / CCChurn4.png) 

Customers with fewer total products through the company are more likely to churn. (CCChurn5.png)

Precision Recall Curve (Gradient Boosting) - (CCChurn6.png)

AUC of different models tested - (CCChurn7.png)

SEE FEATURE IMPORTANCE FOR IMPORTANCE OF FEATURES IN OUR MODEL (CCChurn8.png)
## Acknowledgements
- Many thanks to our BAIS educators to assist us in any of our technical problems throughout the development of this model.


## Contact
Created by [@cadekeenan] <br>
Created by [@immcsorley] <br>
Created by [@timcookk] <br>


 - feel free to contact me!
