# Concepts Used

This project started with a simple question:

How does a real bank account work?

Before writing any code, the first step was identifying what information a bank account should remember and what actions it should perform.

A bank account naturally needs information such as account number, account holder name, account type, and current balance. It also needs the ability to perform operations like depositing money, withdrawing money, and checking the available balance.

This led to the use of Object-Oriented Programming (OOP), where real-world entities are represented as objects.

---

## Class

The idea of a class became useful when defining what a bank account should look like.

Instead of creating separate variables and logic for every customer, a single BankAccount blueprint can be created and reused whenever a new account is needed.

The class acts as a structure that combines account information and account behavior in one place.

---

## Object

Once the BankAccount blueprint exists, actual accounts can be created from it.

For example, different customers may have different balances and account details, but they all follow the same structure defined by the BankAccount class.

Each real account created from the blueprint becomes an object.

---

## Encapsulation

A bank account balance is sensitive information.

Allowing any part of the application to directly change the balance would create a risk of inconsistent or invalid data.

To avoid this, account data is protected and can only be modified through approved operations such as deposit and withdrawal.

This approach keeps the account state controlled and reliable.

---

## Constructor

When a new account is created, it should immediately receive its starting information.

A constructor provides a way to initialize the account with values such as account number, account holder name, account type, and opening balance.

This ensures every account starts in a valid state.

---

## Methods

Methods represent actions that a bank account can perform.

Instead of repeatedly writing the same logic, operations such as deposit, withdrawal, and balance inquiry are grouped into reusable methods.

This makes the system easier to maintain and understand.

---

## Validation

A banking application cannot assume that every request is valid.

For example:

* Depositing a negative amount should not be allowed.
* Withdrawing a negative amount should not be allowed.
* Withdrawing more than the available balance should not be allowed.

Validation rules are applied before processing transactions to ensure that account data remains accurate.

---

## CRUD Operations

The project also demonstrates basic CRUD concepts.

* Create: Creating transaction records during deposits and withdrawals.
* Read: Viewing account information and balance.
* Update: Modifying the balance after successful transactions.
* Delete: Not implemented because banking systems generally preserve transaction history for auditing purposes.

---

## Key Takeaway

The main objective of this project is not just performing deposits and withdrawals. The goal is to understand how real-world business requirements can be translated into structured software using Object-Oriented Programming principles.
