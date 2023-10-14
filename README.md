# Lending Club Case Study

Lending loans to applicants deemed as high-risk constitutes the most significant contributor to financial loss within the lending industry, a phenomenon commonly referred to as credit loss. Credit loss represents the monetary value that lenders incur when borrowers either fail to repay their loans or abscond with the owed funds.

The primary objective at hand is to develop a robust capability for identifying these high-risk loan applicants effectively. Achieving this goal would lead to a reduction in the issuance of loans to such individuals, consequently mitigating the overall credit loss. The crux of this case study lies in employing Exploratory Data Analysis (EDA) techniques to discern the critical factors, often referred to as driver variables, that strongly correlate with loan defaults.

By successfully identifying these key driver variables, the company can harness this valuable knowledge to enhance its portfolio management and risk assessment strategies. This newfound understanding will enable more informed decision-making processes, ultimately fostering a more secure and sustainable lending environment.


## Table of Contents
* [General Info]
* [Business Objective]
* [Dataset Overview]
* [Technologies Used]
* [Observations]
* [Conclusion]


## General Information

When an application for the loan is done, the bank will take either of the below two decisions:

- Loan approved: If approved, there are 3 possible outcomes as mentioned below:

    1. Fully paid: Applicant has fully paid the loan (both the principal and the interest)

    2. Current: Applicant is still paying the installments, (i.e.,) the loan is not fully paid.

    3. Charged-off: Applicant has not paid the installments in due time for a long period of time, i.e. defaulter

- Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)
- Provide general information about your project here.
- What is the background of your project?
- What is the business probem that your project is trying to solve?
- What is the dataset that is being used?


## Business Objective

In this case study, we will undertake a comprehensive exploration of a dataset containing loan data from the period 2007 to 2011. The primary objective is to gain a deep understanding of the factors driving loan default. This analysis will equip our organization with valuable insights to enhance portfolio management and risk assessment.


## Dataset Overview

Dataset Overview:
Dataset Period: 2007 to 2011
Rows: 39,717
Columns: 111
Missing Values: 54 columns have substantial missing values
Purpose: Understand the primary drivers of loan default


## Technologies Used
- Python - version 3.10.4
- ipywidgets - version 8.1.1


## Observations

### Unordered Univariate Analysis:

-	Loan Term: Approximately 73% of loans have a 36-month tenure, while 26% have a 60-month tenure.

-	Loan Grade: Most common loan grades are B (30%), A (25%), and C (20%).

-	Home Ownership and Purpose: About 92% of borrowers either rent or have a mortgage, with only 1% having a loan purpose of "house." 47% of borrowers' primary purpose is "debt consolidation."

-	Verification Status: 42% of borrowers' income is "not verified," which represents a risk.

-	Loan Status: Only 14% of borrowers are classified as "Defaulters."

### Bivariate Analysis on Categorical Variables:

-	Loan Term: Loans with a 60-month tenure are more likely to default (22.6%) than 36-month loans (11.1%).
-	Loan Grade: G-grade loans have the highest default rate (32%), while A-grade loans have the lowest (6%).
-	Employment Length: Loans are more likely to default (15%) when the borrower's employment length is 10+ years.
-	Home Ownership: Borrowers without their own homes have a 13-15% chance of default.
-	Verification Status: "Not Verified" loans carry a 12% default risk.
-	Purpose: Loans with the "small business" purpose have the highest default probability (26%).

### Ordered Univariate Analysis:

-	Employment Length: Most borrowers (22.4%) have 10+ years of employment.
-	Inquiries in the Last 6 Months: 48% of the time, there are no inquiries or 0 inquiries in the last 6 months.

###	Inferences - Segmented Univariate Analysis:

-	Loan Amount and Term: Loan amounts are higher for 60-month loans.
-	Loan Amount and Grade: Loan amounts are higher for G, F, and E-grade loans.
-	Loan Amount and Verification Status: Verified loans tend to have higher loan amounts.
-	Interest Rate and Term: Interest rates are higher for 60-month loans.
-	Interest Rate and Grade: Interest rates increase with lower loan grades.

### Segmented Univariate Analysis on Default Status:

-	Interest Rate: Default loans have higher interest rates, with an average of 13.88% compared to 11.7% for non-default loans.
-	Annual Income: Defaulters tend to have lower annual incomes.
-	Principal Received: Defaulters receive significantly less principal.
-	Revolving Line Utilization Rate: Higher utilization rates are associated with loan default.
-	Open Credit Lines: Defaulters have fewer open credit lines.

### Segmented Univariate Analysis on Default Status Over Time:

-	Loan Applicants: The number of loan applicants increased over time, with the highest in 2011.
-	Loan Amount: Higher loan amounts are observed in the second half of the year.

### Bivariate Analysis on Continuous Variables:

-	Loan Amount: Highly correlated with funded amount.
-	Loan Amount and Installment: Strong positive correlation.
-	Total Account Lines and Open Account Lines: Highly correlated.
-	Revolving Line Utilization Rate and Interest Rate: Moderately correlated.

### Correlations Between Loan Amount, Funded Amount, and Installment:

-	Funded amounts are highly correlated with loan amounts and installments.

## Conclusion:

- This exploratory data analysis provides a robust foundation for further data preprocessing, feature engineering, and predictive modelling. 
- It is evident that various factors such as loan term, grade, employment length, and verification status significantly influence the likelihood of loan default. 
- These insights will be instrumental in enhancing our portfolio management and risk assessment strategies.





## Contact
Created by [Pooja and Shyam1693] - feel free to contact us!