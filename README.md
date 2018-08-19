# retirement_goal_calc

The retirement_goal_calc determines how much per-month you will need to save to meet your monthly retirement dividend goal. It creates an amortization calendar for your current mortgage to determine what your payoff date will be at your current rate of payment, estimates what your retirement account monthly divident will be based on your current rate of savings, and compares those two things to tell you whether you are on track to retire on your goal date. If you are not on track, it will tell you how much more you need to put into savings and/or your mortgage to be on track.

To do these calculations, the retirement_goal_calc will use information from the YNAB API (api.youneedabudget.com) and information you enter, such as target retirement date and estimated rate of return.


## Information to GET from YNAB API: 
  * https://api.youneedabudget.com/v1#/Budgets/getBudgets Returns a list of all budgets. Ask user to identify which budget to use.
  * https://api.youneedabudget.com/v1#/Accounts/getAccounts Returns a list of accounts in that budget. Ask user to identify which are their mortgages and which are investment accounts.
  * https://api.youneedabudget.com/v1#/Accounts/getAccountById Use when updating account amounts after the correct accounts have been identified. Returns specific account balance by ID. Use for mortgages and investments.
  
## Information to GET from USER:
  * Mortgage interest rate
  * Life of Loan Left
  * Target Retirement Date
  * Estimated Investment Rate of Return
  * Name of Mortgage Budget Item
  * Name of Investments Budget Item
  
## Calculations:
  * Principal Payment Required to Pay off House By Target Date
  * Required Total Investment for Desired Dividend
  * Compound Interest on Investment
  * Boolean for Current Rate match Future Goal
  
  
