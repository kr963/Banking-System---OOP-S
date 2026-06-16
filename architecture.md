# System Architecture

The system is designed around a simple banking workflow where a bank account acts as the central entity.

The account stores account information and provides controlled operations for managing balance updates.

---

## High-Level Architecture

```text
User
 |
 v
BankAccount
 |
 +--> Deposit
 |
 +--> Withdraw
 |
 +--> Check Balance
 |
 +--> Transaction History
```

---

## Core Components

### BankAccount

The primary object responsible for:

* Maintaining account information
* Maintaining account balance
* Processing deposits
* Processing withdrawals
* Providing account details

---

### Transaction

Represents a financial activity performed on an account.

A transaction may contain:

* Transaction Type
* Amount
* Timestamp
* Balance After Transaction

Multiple transactions collectively form an account statement.

---

## Data Flow

### Deposit

```text
Input Amount
      |
      v
Validation
      |
      v
Balance Update
      |
      v
Transaction Creation
      |
      v
Updated Balance
```

---

### Withdrawal

```text
Input Amount
      |
      v
Validation
      |
      v
Balance Check
      |
      v
Balance Update
      |
      v
Transaction Creation
      |
      v
Updated Balance
```

---

## Design Objective

The architecture focuses on keeping:

* Data organized
* Operations controlled
* Validation centralized
* Business logic easy to understand

The design intentionally remains simple so that the relationship between business requirements and implementation remains clear.
