# Personal Bank Account System

## Overview
This project implements a simple personal bank account system using Python. It consists of two main classes:

- **Amount**: Represents a transaction amount with a timestamp and type.
- **PersonalAccount**: Represents a personal bank account that manages deposits, withdrawals, and transaction history.

The `main.py` file demonstrates the usage of these classes by allowing user input for deposits and withdrawals.

## Features
- Create a personal bank account.
- Deposit and withdraw money.
- Maintain a transaction history.
- Retrieve account details and balance.
- Overloaded `+` and `-` operators for deposits and withdrawals.

## Class Structure
### `Amount` Class
- **Attributes:**
  - `amount (float)`: Transaction amount.
  - `timestamp (datetime)`: Transaction date and time.
  - `transaction_type (str)`: Transaction type ('DEPOSIT' or 'WITHDRAWAL').
- **Methods:**
  - `__init__(self, amount, timestamp, transaction_type)`: Initializes an Amount object.
  - `__str__(self)`: Returns a string representation of the transaction.

### `PersonalAccount` Class
- **Attributes:**
  - `account_number (int)`: Unique account identifier.
  - `account_holder (str)`: Name of the account holder.
  - `balance (float)`: Current balance.
  - `transactions (list)`: List of Amount objects.
- **Methods:**
  - `__init__(self, account_number, account_holder)`: Initializes an account with a zero balance.
  - `deposit(self, amount)`: Deposits money and updates transaction history.
  - `withdraw(self, amount)`: Withdraws money if the balance allows and updates transaction history.
  - `print_transaction_history(self)`: Displays all transactions.
  - `get_balance(self)`: Returns the current balance.
  - `get_account_number(self) / set_account_number(self, account_number)`: Get/set account number.
  - `get_account_holder(self) / set_account_holder(self, account_holder)`: Get/set account holder name.
  - `__str__(self)`: Returns a string representation of the account.
  - `__add__(self, amount)`: Overloads `+` operator to deposit money.
  - `__sub__(self, amount)`: Overloads `-` operator to withdraw money.


