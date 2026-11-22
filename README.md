# Python Banking System

A menu-driven banking simulation developed in Python for ICT100 at Murdoch University.

The application supports savings and credit accounts, basic transactions and monthly account updates. It demonstrates functions, conditional logic, loops, input validation and exception handling.

## Features

- Create a savings or credit account.
- Deposit money and update the account balance.
- Withdraw money subject to account-specific rules.
- Display the account holder's name, account type and current balance.
- Apply monthly interest and fees.
- Continue performing operations through a repeating menu.
- Exit with a closing message.

## Account Rules

| Feature | Savings account | Credit account |
|---|---|---|
| Starting balance | Non-negative | Negative balances permitted within the credit limit |
| Deposits | Positive amounts accepted | Positive amounts accepted |
| Withdrawals | Cannot exceed the available balance | Cannot take the balance below the credit limit |
| Monthly update | Adds interest and deducts a bank fee | Applies an overdue fee when the balance is negative |

The assignment uses a 2% monthly savings interest rate, a $5 monthly bank fee, a $2,000 credit limit and a $25 overdue fee. These are simulation settings specified in the program.

## Python Skills Demonstrated

- Variables and numeric data types.
- Reusable functions for individual operations.
- A while loop for the main menu.
- if, elif and else statements for menu selection and account rules.
- User input and conversion to numeric values.
- try and except ValueError for invalid numeric input.
- Formatted strings for displaying currency.
- Updating application state through account variables.
- Breaking a loop to exit the application.

## Program Structure

| Function | Responsibility |
|---|---|
| v_app_header() | Display the welcome message |
| account_creation() | Capture account details and set the starting balance |
| money_deposit() | Validate and process deposits |
| money_withdraw() | Validate withdrawals and apply account limits |
| print_account() | Display account details |
| apply_monthly_update() | Apply the relevant interest or fees |
| v_app_footer() | Display the closing message |

## Input Validation

The program includes checks for:

- Non-numeric transaction amounts.
- Zero or negative deposits and withdrawals.
- Transactions attempted before an account exists.
- Savings withdrawals exceeding the available balance.
- Credit withdrawals exceeding the credit limit.
- Invalid main-menu selections.

## Development and Testing

The assignment follows an incremental approach organised around user stories.

Each story documents:

1. Requirements and intended tests.
2. Problem analysis.
3. Solution design.
4. Python implementation.
5. Testing evidence.

Documented test scenarios include normal transactions, invalid inputs, insufficient funds and credit-limit boundaries.

The retrospective discusses lessons learned about modular functions, debugging, input validation and testing under different conditions.

## Reviewing the Project

Open the uploaded assignment report to review the user stories, design explanations, code, testing screenshots and development retrospective.

The complete Python source is included in the report's Full Code section.

To run that version:

1. Copy the code from the Full Code section into a plain-text file named banking_system.py.
2. Check that indentation and quotation marks are preserved when copying from Word.
3. Open a terminal in the folder containing the file.
4. Run `python banking_system.py` or `python3 banking_system.py`.
5. Create an account and use the numbered menu to explore the features.

## Scope and Limitations

- Account information is held in memory and is lost when the program closes.
- The program manages one current account at a time.
- It uses procedural functions and global variables.
- Authentication, persistent storage and a transaction history are outside the implemented scope.

## Possible Future Improvements

- Store account information in a database.
- Support multiple accounts.
- Add transaction history.
- Separate account data from the command-line interface.
- Introduce automated tests.
- Use decimal arithmetic for monetary calculations.

## Tools and Academic Context

- Language: Python
- Interface: Command line
- Unit: ICT100
- Institution: Murdoch University
- Author: Vaibhav Saini
- Year: 2025
