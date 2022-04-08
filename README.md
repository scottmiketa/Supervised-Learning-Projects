# Supervised-Learning-Projects
This repo includes: Polynomial Regression, Support Vector Machines, kNN Classifiers, and Gradient Boosting Classifiers.

## kNN_Cancer.ipynb
This notebook contains a k-Nearest Neighbor classifier on scikit-learn's breast cancer dataset, that includes 30 different features. I have detailed how I chose a value of k, and the comparison between the test accuracies of different k-means.

## Spam_Classification_Evaluation.ipynb
Using a Support Vector Machine, I have used GridSearchCV to find which parameters yield the highest recall score on the ability to classify certain e-mails as spam or not spam, and have visualized both a precision-recall curve, and a ROC curve with the data.

## Polynomial_Regression.ipynb
In this notebook, I will be exploring how model complexity relates to generalization performance, and how Lasso regression methods constrain model complexity and reduce overfitting.

## Blight_GradientBoostingClassifier.ipynb
Blight violations are issued by the city of Detroit to individuals who allow their properties to remain in a deteriorated condition. I have used a Gradient Boosting Classifier to predict the probability that a blight ticket will be paid on time

### Data fields

#### train.csv & test.csv

ticket_id - unique identifier for tickets

agency_name - Agency that issued the ticket

inspector_name - Name of inspector that issued the ticket

violator_name - Name of the person/organization that the ticket was issued to

violation_street_number, violation_street_name, violation_zip_code - Address where the violation occurred

mailing_address_str_number, mailing_address_str_name, city, state, zip_code, non_us_str_code, country - Mailing address of the violator

ticket_issued_date - Date and time the ticket was issued

hearing_date - Date and time the violator's hearing was scheduled

violation_code, violation_description - Type of violation

disposition - Judgment and judgement type

fine_amount - Violation fine amount, excluding fees

admin_fee - $20 fee assigned to responsible judgments

state_fee - $10 fee assigned to responsible judgments

late_fee - 10% fee assigned to responsible judgments

discount_amount - discount applied, if any

clean_up_cost - DPW clean-up or graffiti removal cost

judgment_amount - Sum of all fines and fees

grafitti_status - Flag for graffiti violations


#### train.csv only

payment_amount - Amount paid, if any

payment_date - Date payment was made, if it was received

payment_status - Current payment status as of Feb 1 2017

balance_due - Fines and fees still owed

collection_status - Flag for payments in collections

compliance [target variable for prediction] 
 Null = Not responsible
 0 = Responsible, non-compliant
 1 = Responsible, compliant
 
compliance_detail - More information on why each ticket was marked compliant or non-compliant
