# Project Name
> Lending Club Case Study


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

- Provide general information about your proje
## General Information
You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

 * If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

 * If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
 
### Project Backgroud
When a person applies for a loan, there are two types of decisions that could be taken by the company:

* Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:

    * Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

    * Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

    * Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 

* Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

### What are we trying to solve?

This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). The credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. 

* Identification of such applicants using EDA is the aim of this project.
* This project will help the lending club company to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment.
* Using the information given about past loan applicants and whether they ‘defaulted’ or not, this project will identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

## Dataset used
* loan.csv
* Data_Dictonary.xls

## Conclusions
Close to 15% of the total applicants are defaulters.

Below factors play a major role in identifying defaulters:

* Purpose
     Debt consolidation has the highest number of loans granted.
     Small business has the highest number of defaulter ratio.
     Defaulter applicants count are high for loan amount:
        10000 to 25000 under debt_consolidation
        spread across for small_business

* Home ownership
    Rented and Mortgage have highest number of defaulters.
    Default rates are high for loan amount = 5000 to 13000 under RENT category
    Default rates are high for loan amount = 10000 to 25000 under MORTGAGE category

* Employment length
    Employees with 10+years of experience tend to default more.

* Verification Status
    There is a huge number of applicants whose annual incomes are not verified, this needs to be completed to understand the trends with more clarity.

* DTI and Annual income
    Applicants with higher dti and low annual incomes tend to default.


* DTI and Inquiry in last 6 months
    Less number of inquires indicate more dti rates which further indicate less annual incomes, implying the borrower to be a defaulter.

* Term
    More number of loans were requested for 36 month tenure.
    Borrowers who request for loan amounts between 0 and 14000 with 36 months tenure tend to default more.
    Borrowers having annual incomes in ranges, 20000-40000, 40000-60000, 60000-90000 tend to default more.

* Address States
    Applicants from CA tend to default more compared to other states.

* Grades and Interest Rates
    High quality loans[grades A and B] have high loan applicantion requests.
    Higher interest rate have higher tendency to default the loan.

## Technologies Used
- Jupyter Notebook
- Python 3.8
- seaborn - version 0.11.2
- matplotlib - version 3.4.3
- plotly - version 5.4.0
- pandas - version 1.2.3
- numpy - version 1.20.1

## Acknowledgements
- This project was case study given by Upgrad IIIT Bangalore to do analysis & recommendations for the Lending Club company on loan defaulting mechanism

## Contact
- Created by Nikhil Patel [@np4800]
- Created by Shruthi N [@ShruthiNandakumar]