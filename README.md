 # Car_insurance_recommender_system
## Project Objective:
The objective of this project is to design and implement a machine learning-based insurance policy recommender system that provides personalized policy recommendations to customers based on their profile, preferences, and past interactions. The system aims to enhance customer satisfaction by suggesting relevant policies while optimizing sales for the insurance company.

## Scope:
The recommender system will use a combination of customer demographic data, historical purchase behavior, policy details, and risk profiles to deliver accurate recommendations. The system will cater for car insurance only.

Key Features:
1. Customer Profiling: Leverage customer data such as age, income, family status, and occupation to build detailed customer profiles.
2. Policy Matching: Match customers with policies based on relevant features like coverage, premium, and tenure using both collaborative and content-based filtering techniques.
3. Behavioral Analysis: Incorporate user behavior, such as past purchases, into the recommendation process.
4. Risk Assessment: Integrate customer risk profiles to suggest suitable coverage options and premiums.
5. Continuous Learning: Implement a feedback loop to refine recommendations over time as more data is gathered.

The reccomendations will be based on:
1. Customer demographics
2. Insurance needs
3. Purchase history

   ## Data
The data used in this project was gotten from kaggle and can be viwed [here](https://www.kaggle.com/datasets/shibumohapatra/customer-life-time-value?select=test_koRSKBP.csv). 
There are two datasets the train and test sets which each has the following columns:

1. id-Unique identifier of a customer
2. gender-Gender of the customer(male or female)
3. area-Area of the customer(urban or rural)
4. qualification-Highesteducational  qualification of the customer
5. income-Income earned in a year (in rupees)
6. marital_status-Marital Status of the customer {0:Single, 1: Married}
7. vintage-No. of years since the first policy date
8. claim_amount-Total Amount Claimed by the customer (in rupees)
9. num_policies-Total no. of policies issued by the customer
10. policy-Active policy of the customer
11. type_of_policy-Type of active policy(Gold, silver or platinum)
12. cltv- Customer lifetime value 
