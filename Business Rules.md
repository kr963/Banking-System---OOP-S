# Business Rules

Business rules define the conditions that must be followed before an operation can be performed.

The application logic is built around these rules.

---

## Account Rules

### Rule 1

Every account must have:

* Account Number
* Account Holder Name
* Account Type
* Balance

An account cannot exist without these basic details.

---

## Deposit Rules

### Rule 2

Deposit amount must be greater than zero.

Valid Example:

```text
Deposit = 500
```

Invalid Example:

```text
Deposit = -500
```

---

## Withdrawal Rules

### Rule 3

Withdrawal amount must be greater than zero.

Valid Example:

```text
Withdraw = 300
```

Invalid Example:

```text
Withdraw = -300
```

---

### Rule 4

Withdrawal amount cannot exceed the available balance.

Valid Example:

```text
Balance = 1000
Withdraw = 500
```

Invalid Example:

```text
Balance = 1000
Withdraw = 1500
```

---

## Balance Rules

### Rule 5

Balance should only change through approved banking operations.

Examples:

* Deposit
* Withdrawal

Direct modification of balance is not allowed.

---

## Transaction Rules

### Rule 6

Every successful financial operation should generate a transaction record.

Transaction records improve traceability and account transparency.

---

## Data Integrity Rules

### Rule 7

Account information should remain consistent throughout the lifecycle of the account.

Validation must occur before updating any critical account data.

---

## Purpose

The purpose of these rules is to ensure that the banking system remains predictable, reliable, and aligned with real-world banking practices.
