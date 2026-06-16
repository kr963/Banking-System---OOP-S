# Design Decisions

This document explains the reasoning behind the main design choices used in the banking system project.

---

## BankAccount as the Main Object

The `BankAccount` object was chosen as the center of the project because most banking operations revolve around an account.

Deposits, withdrawals, balance checks, and transaction activity all depend on the account.

This made `BankAccount` the natural place to keep account-related information and behavior together.

---

## Keeping Balance Private

The account balance is one of the most important pieces of information in the system.

It should not be changed directly from outside the account object.

Instead, balance changes should happen only through controlled operations such as deposit and withdrawal.

This protects the account from invalid updates and supports encapsulation.

---

## Using Methods for Banking Operations

Banking actions were separated into methods to keep the logic clear and reusable.

Examples:

* `deposit()`
* `withdraw()`
* `checkBalance()`

Each method represents one specific operation and keeps the code organized.

---

## Adding Validation Before Updating Balance

Validation is required before changing the balance.

For example:

* Deposit amount should be greater than zero.
* Withdrawal amount should be greater than zero.
* Withdrawal amount should not exceed available balance.

These checks prevent invalid transactions and keep the account state accurate.

---

## Transaction History Consideration

A banking system should maintain a record of account activity.

Transaction history is important because it helps track:

* What type of transaction happened
* How much money was involved
* When the transaction happened
* What the balance was after the transaction

This also supports auditability and traceability.

---

## Why Delete Is Not Included

Delete functionality was intentionally excluded from the current design.

In financial systems, transaction records should usually be preserved instead of removed.

If a mistake happens, a correction or reversal transaction is safer than deleting the original record.

This helps maintain a complete transaction trail.

---

## Simple Design First

The project starts with a simple design to make the core concepts clear.

The focus is on understanding:

* OOP structure
* Banking logic
* CRUD mapping
* Validation
* Clean design thinking

Advanced features such as database integration, APIs, inheritance, polymorphism, and frontend dashboards can be added later.
