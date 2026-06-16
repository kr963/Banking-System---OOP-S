# Project Flow

The objective of this project is to simulate how a basic banking system processes transactions while maintaining account information and balance accuracy.

Rather than starting with code, the flow was designed by thinking about how a real bank operates when a customer performs a transaction.

---

## Understanding the Account

A bank account acts as the central entity in the system.

The account maintains information such as:

* Account Number
* Account Holder Name
* Account Type
* Current Balance

Every operation performed by the customer eventually affects the account balance.

---

## Deposit Flow

A deposit operation follows a simple sequence.

1. The customer enters an amount.
2. The system validates the amount.
3. The current balance is retrieved.
4. The deposit amount is added to the balance.
5. The balance is updated.
6. A transaction record is created.
7. The updated balance is displayed.

Example:

```text
Current Balance = 1000

Deposit Amount = 500

Updated Balance = 1500
```

The purpose of this flow is to ensure that every deposit updates the account consistently.

---

## Withdrawal Flow

A withdrawal operation requires additional validation.

1. The customer enters an amount.
2. The system validates the amount.
3. The system checks available balance.
4. If sufficient funds exist, the amount is deducted.
5. The balance is updated.
6. A transaction record is created.
7. The updated balance is displayed.

Example:

```text
Current Balance = 1500

Withdrawal Amount = 300

Updated Balance = 1200
```

If the withdrawal amount exceeds the available balance, the transaction is rejected.

---

## Transaction Recording

Every successful operation should leave a record.

Each transaction can contain:

* Transaction Type
* Amount
* Date and Time
* Balance After Transaction

This information forms the basis of a bank statement.

---

## Validation Strategy

The project applies basic validation rules before modifying account data.

Examples:

* Deposit amount must be greater than zero.
* Withdrawal amount must be greater than zero.
* Withdrawal amount cannot exceed available balance.

The purpose of validation is to prevent invalid account states.

---

## Design Philosophy

The design follows a simple principle:

```text
Store account information safely.
Perform operations through controlled methods.
Validate before updating data.
Record important transactions.
```

This mirrors the way real-world banking systems maintain accuracy and consistency.
