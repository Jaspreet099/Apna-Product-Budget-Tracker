# Apna-Product ~ Bugdet-tracker
Budget Tracker app with React and Speechly!

![image](https://user-images.githubusercontent.com/75212002/208305764-9dad9df3-f3b5-4081-8a98-e0ceef261612.png)

The budget tracker can be further developed to include more features and capabilities. For example, it could be enhanced with income and expense tracking and forecasting, as well as a more comprehensive budgeting system. We are also planning to add authentication system in our website. 
Additionally, the budget tracker could be incorporated into a larger personal finance application, allowing users to manage all of their finances in one place. Finally, the budget tracker could be connected to other financial services, such as banks and investment accounts, to provide a more integrated financial management experience.

 
 ## This is the code for speechly to work how it is susposed to!
 ```javascript
  category_income = [
    Business
    Investments
    Extra income
    Deposits
    Lottery
    Gifts
    Salary
    Savings
    Rental income
]
category_expense = [
    Bills
    Car
    Clothes
    Travel
    Food
    Shopping
    House
    Entertainment
    Phone
    Pets
    Other
]
*create_transaction [Create|Finish|Save] {transaction}
*cancel_transaction [Cancel|Delete|Remove|Clear] {transaction}
*add_category [Set|Change] category {to} [$category_expense|$category_income](category)
*add_category {[i mean|i meant|i said]} {the} ![category {[is|of]} | [$category_expense|$category_income](category)]
*add_date [Set|Change|Add] date {[to|for]} $SPEECHLY.DATE(date)
*add_date {[i mean|i meant|i said]} {[{the} date is|for]} $SPEECHLY.DATE(date)
*add_amount [Set|Change] amount {to} $SPEECHLY.NUMBER(amount) {dollars}
*add_amount {[i mean|i meant|i said]} {{the} amount {[is|of]}} $SPEECHLY.NUMBER(amount) {dollars}
*add_expense {Add} {an} expense ![{[for|of]} $SPEECHLY.NUMBER(amount) {dollars} | {in} | {category} | [$category_expense|$category_income](category) | {[for|in]} $SPEECHLY.DATE(date)]
*add_expense $SPEECHLY.NUMBER(amount) {[dollar|dollars]} expense {in} ![{category} | [$category_expense|$category_income](category)] {[for|in]} $SPEECHLY.DATE(date)
*add_income {Add} {[{an} income|{a} balance]} ![{[for|of]} $SPEECHLY.NUMBER(amount) {dollars} | {in} | {category} | [$category_expense|$category_income](category) | {[for|in]} $SPEECHLY.DATE(date)]
*add_income $SPEECHLY.NUMBER(amount) {[dollar|dollars]} [income|balance] {in} ![{category} | [$category_expense|$category_income](category)] {[for|in]} $SPEECHLY.DATE(date)
 ```
 #
### To build this application I have used next technologies:
  * Front End
    - React
      - Context API
      - Hooks
    - react-chartjs-2(for creating charts)
    - chart.js(for creating charts)
    - uuid(for creating unique ids)
    - material-ui(for styling)
