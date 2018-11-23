# M-Kopa Data Science Hiring Exercise

## Introduction

The goal of this exercise is to help us understand your abilities around exploring data, building machine learning models, and evaluating those models' results. The exercise uses a dummy data similar in style to M-KOPA's loan book. It is meant as a fairly quick undertaking, and shouldn't take more than 1-3 hours. Feel free to seek clarifications on variable meanings or other features of the dataset.

## The Exercise

Attached alongside this file is a data file named: `Data Science Assessment.csv`. Each row in this file consists of a single loan. Each loan has two outcome variables (explained in the following section): `AmountPaid360` and `LoanStatus360`. The first of these variables is a continuous numerical value, the second is a categorical variable. Your objective is:

- build a regression model to predict `AmountPaid360` OR a classification model to predict `LoanStatus360` OR both (your choice) 
- evaluate the performance of your model(s)
- briefly communicate your process for model building, your model results, any limitations that you faced, and what next steps you might take with additional data access

You can submit your results in any format (including working formats like a Jupyter notebook or an R Markdown file). Your submission should be clear but does not need to be formal. 

**Important:** Please treat this exercise as something close to a [Fizz Buzz](https://imranontech.com/2007/01/24/using-fizzbuzz-to-find-developers-who-grok-coding/) equivalent for data science. You need to show that you can build a basic model, evaluate its results, and communicate that evaluation professionally. However this is not a Kaggle competition - you do not need to produce a model with earth-shattering performance! This exercise should take a few hours at most. If you find yourself being bogged down in an excessive amount of work, please reach out to your contact person at M-Kopa to explore alternatives.

## Dataset Structure

### Input Features

- `Product`: The product type purchased by the customer
- `CustomerGender`: Self-explanatory
- `Location`: The location where the loan was issued. (Also includes a long-tail of legacy locations)
- `Region`: The sales region where the device was purchased. Includes many regions which have since been changed. The current set of main sales regions are Regions 1-7.
- `TotalPrice`: The total amount to-be-paid by the customer over the course of the loan (including deposit and daily payments)
- `StartDate`: The day on which the customer's loan became active
- `Deposit`: The initial deposit required from the customer prior to loan activation
- `DailyRate`: The amount that the customer must pay daily in order to continue to use their device
- `TotalDays`: The number of days for which the customer is expected to continue paying the daily rate
- `AmountPaid30`: The amount that the customer had repaid as of the 30th day of their loan
- `AmountPaid60`: The amount that the customer had repaid as of the 60th day of their loan

### Outcome Variables

- `AmountPaid360`: The amount that the customer had repaid as of the 360th day of their loan
- `LoanStatus360`: The status of the loan as of day 360:
  - `Active`: The customer is still actively repaying their loan.
  - `Blocked`: The customer has had their account blocked after more than 30 days without a payment.
  - `Finished Payment`: The customer has successfully repaid their loan.


