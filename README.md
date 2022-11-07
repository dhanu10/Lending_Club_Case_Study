# Project Name
> Lending Case Study, Project Group members - Dhananjay Joshi and Shajiv Kalangath



## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
This project is for data analyst working in a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
 

In this case study, we used variius principles, tactics under EDA (Exploratory Data analysis ) to understand how consumer attributes and loan attributes influence the tendency of default and provided various recommendations.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
# Some upfront observations from data and adjustments to data :
    Loan amount distribution skewed between 5K to 10K
    Only 2 Terms of loan - 12 adn 36 months , we called 0 and 1
    Majority of loans distribted between 10 - 15% intrest rate
    issue_d i.e. issue date could be intresting field to inspect
    Zip code 800+ has more loan disbursment, may be particular state
    Earliest credit line year between 1998-2000 has more default instances to be checked
    last_credit_pull_d has major instances in 2016 for some reason
# Conclusions from data  :
- no major outliers apart from interest_rate_pct. However not significant number to be dropped form analysis.
- in cases, where there are outliers, number of such instances are very high like annual income, so we didn't drop anything from analysis.
- 7-8 types of clean-ups required in the data which was performed as shown in the code.
- No particular relation with home_ownership and defaulting or non-defaulting customers.
- As intrest rate grows, there is a high risk of defaulting and even otherwise Bank may choose higher interest rates for high risk consumers.
- If interest rate is >10%, higher default rate, % of defaults increase with every interest rate change.
- Grades E, F, G in particular and in general as grade increases, higher defaulting risks from approved loan requests.
- Zip code ranges 300xx-400xx , 900xx+ and 800xx-900xx have higher defaulting tendency. ( may be certain income groups ? )
- NE state stands out in percentage terms, however, in absolute terms, CA has higher defaulting rate.
- Verification status has no particular bearing on default or success rate of loan application.
- By absolute terms and percentage terms - 'small business' and 'debt consolidation' have higher default.
- whoever have 2006/2007 as initial credit line year , have higher defaulting rate.
- %wise higher defaults in 2007, however absolute number wise 2011 was special year as well when default numbers increased.
- longer term loans ( 36 months) have higer risk than shorter term loans, specially it also links to employment length. So employment length 10+ year, higher intrest rate and longer term loans have higher risk of defaulting - kind of deadly combination.
- out of approved loan_amount, around 60% of principle could be recovered i.e. remaining average 40% is risk that organisation carries when someone defaults. However such risk for small loan amounts upto 15K is much higher and Bank may lose from 50-100% of approved amt.
- Gross recoveries post charge off are higher upto 25K loan amount and for 35K as well. recoveries increased linearly with loan amount upto 25K, which means Bank is not losing money and able to recover from risk position.
- Loan defaulting increases after 8 years of employment length marginally.
- For longer term loans given for educational purposes to people with more than 8 years employment do have small risk of defaulting.



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
Pandas Version : 1.0.5
Numpy  Version : 1.22.3
Seaborn Version : 0.10.1
Matplotlib Version : 3.2.2
Python 3
<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Various ideas were picked up from searachable internet content to build the analysis in addition to lectures in upgrad.


## Contact
Created by [@dhanu10] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
