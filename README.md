# Online Payment Fraud Exploratory Data Analysis 


![HDB](./pictures/fraud1.jpg "HDB")

## Project Overview

As online transactions continue to grow in popularity, so does the prevalence of fraudulent activities. The data analytics team of SPREE!, an E-commerce company has been tasked with analyzing a dataset of online payment fraud to uncover key insights, identify emerging patterns, and develop strategies to detect and prevent fraudulent transactions more effectively.

## Table of Contents
1. [Problem Definition](#problem-definition)
2. [Data Collection](#data-collection)
3. [Exploratory Data Analysis](#exploratory-data-analysis)
4. [Key Insights](#key-insights)

## Problem Definition
- Problem Statement
  - Conduct exploratory data analysis of online payment transaction dataset and provide insights to key stakeholders.


## Data Collection
- **Dataset Source**:
  - https://www.kaggle.com/datasets/jainilcoder/online-payment-fraud-detection

  
## Exploratory Data Analysis


1. What percentage of the total transactions are fraudulent?
   
   A total of 8,213 (out of 6,354,407) fraudulent transactions occurred, making up approximately 0.13% of all transactions.

    ![distribution](./pictures/Q1.png "distribution")

2. Were we able to flag the fraudulent transactions as 'isFlaggedFraud'?

   No, only 16 out of 8213 fraudulent transactions were flagged as fraudulent, which represents just 0.195% of the total fraud transactions.

    ![distribution](./pictures/Q2.png "distribution")
    
3. What types of online transactions are available, and which are the most common?

   Payment, transfer, cash out, debit and cash in. Payment and cash out are the most common.

   ![distribution](./pictures/Q3.png "distribution")

4. Which payment transfer type is most affected by fraud?
   
   Fraud has occurred exclusively in the 'cashout' and 'transfer' payment types. Specifically, 0.183% (4116 / 2233384) of transactions in the 'cashout' mode were fraudulent, while 0.769 (4097/528812) of transactions in the 'transfer' mode were fraudulent.

   ![distribution](./pictures/Q4.png "distribution")
  
5. Are all the transactions marked as 'isFlaggedFraud' correctly identified as fraud?

   Yes, all 16 transactions flagged as fraud are indeed fraudulent

   ![distribution](./pictures/Q6.png "distribution")
  
8. What is the amount range for fraudulent transactions?
   
   Fraudulent transaction amounts range from $4,500 to $360,000, with the highest frequency occurring in the $340,000 to $360,000 range.

   ![distribution](./pictures/Q5.png "distribution")


## Key Insights

- A significant number of records have been incorrectly flagged as '0'. This misclassification could have a major impact in the future if not addressed properly, as it may lead to an inflated online payment fraud percentage, especially given the growing reliance on online payments.

- Fraudsters typically target amounts ranging from $340,000 to $360,000, which represents top 10 percentile of transaction amount. Their focus is primarily on 'cashout' and 'transfer' modes. Interestingly, fraud is much less likely to occur during 'payment' mode transfers, despite the increasing use of online payments.



