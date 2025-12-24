# Google Pay Inspired Expense Sharing System

## Project Overview
This project implements a Google Pay–inspired expense sharing system that allows a group of users to fairly split expenses and calculate settlements. The system ensures that each participant pays their fair share and generates a clear settlement showing who owes whom.

## Methodology
- Expenses are split equally among participants.
- The payer is reimbursed based on how much they paid on behalf of others.
- Net balances are calculated for each user.
- A settlement algorithm matches debtors and creditors efficiently.

## Data Processing Steps
- User inputs are collected via CLI.
- Inputs are cleaned using string stripping and validation.
- Balances are updated after every expense.
- Creditors and debtors are identified based on final balances.

## Data Science Techniques Used
- Dictionary-based aggregation for balance tracking.
- Sorting and greedy matching for settlement calculation.
- Error handling for edge cases (missing input, invalid users).

## Handling Edge Cases
- Uneven contributions handled via balance adjustment.
- Empty participant list prevented.
- Incorrect payer names validated.
- Multiple expenses supported.

## Sample Input
Friends: vani, vaithi, vaishara  
Expense: vani paid 1000 for vani, vaithi, vaishara

## Sample Output
vaishara owes vani: Rs.300.00  
vaithi owes vani: Rs.100.00

## Challenges & Improvements
- Handling user input validation in CLI.
- Future improvement: GUI or web app using Flask.
- Can add expense visualization using charts.
