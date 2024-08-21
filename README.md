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

## Tools used :
Everything was done in python using jupyter notebook. 

## Data cleaning and preparation 
Steps undertaken : 
1. Checked for missing values - there were no missing values
2. Checked for duplicates - there were no duplicates
3. Checked the data types - there are some categorical values and since machine learning models do not work well with text data  I encoded the categorical columns.
    
gender, area, num_policies, policy, income, qualification, and type_of_policy are categorical columns, one hot encoding was used to encode them. 

## Exploratory data analysis
### Questions asked
1. How many males and females have taken policies?
   - 64849 females have taken up policies. 
   - 84138 males have taken up policies.
 2. How many females and males have taken each type of policy?
### Policy Counts by Gender

| Policy Type | Female Count | Male Count |
|-------------|--------------|-----------|
| Gold        | 15013          | 19207 |
| Platinum    | 33977         | 45727 |
| Silver      | 15859         | 19204  |

3. How many females and males live in the rural and urban areas
   ### Area count by gender
   
| Area Type | Female Count | Male Count |
|-------------|--------------|-----------|
| Rural       | 21160        | 23931|
| Urban       | 43689        | 60207|

4. Claim amount distribution
   - The trend in claim amaount is the same for both the train and test set.
   - The distribution is abit skewed to the right.
   - The range of claims is between zero and 30000
     
5. Claim amount by gender
6. Claim Amount by Policy Type
7. Claim Amount by Vintage
8. Income Distribution
   
| Income type          | Count |  
|-------------         |--------------|
| income_2L-5L        | 21158  |
| income_5L-10L        | 52716  | 
| income_<=2L         | 1854  |
| income_More than 10L| 13664 | 

9. Income distribution for males and females
    
| Policy Type          | Female Count | Male Count |
|----------------------|--------------|-----------|
|income_2L-5L          | 15758	       | 19460 |
| income_5L-10L        | 37073	       | 50731 |
| income_<=2L          | 1782         | 1356  |
| income_More than 10L | 10236        | 12591 |

    
