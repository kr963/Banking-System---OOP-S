# CRUD Operations

Although this project is intentionally simple, it demonstrates how CRUD operations appear in a real-world banking workflow.

CRUD stands for:

* Create
* Read
* Update
* Delete

Rather than treating CRUD as a technical concept, this project approaches it through banking operations.

---

## Create

A create operation occurs whenever a new transaction is generated.

Examples:

* Deposit transaction
* Withdrawal transaction

Every successful operation results in the creation of a transaction record containing information such as transaction type, amount, timestamp, and updated balance.

---

## Read

Read operations are performed whenever account information is viewed.

Examples:

* Checking current balance
* Viewing account details
* Viewing transaction history

These operations retrieve information without modifying any existing data.

---

## Update

Update operations occur whenever existing account information changes.

The most common update in this project is balance modification.

Examples:

```text
Current Balance = 1000

Deposit = 500

Updated Balance = 1500
```

```text
Current Balance = 1500

Withdrawal = 300

Updated Balance = 1200
```

The account balance is updated only after validation rules are successfully passed.

---

## Delete

Delete functionality is intentionally excluded from the current version of the project.

In banking systems, transaction history is generally preserved for auditing, compliance, and traceability purposes.

Instead of deleting transactions, real-world systems typically create adjustment or reversal transactions to maintain a complete record of account activity.

---

## CRUD Mapping Within The Project

| Operation | Banking Example                      |
| --------- | ------------------------------------ |
| Create    | Create transaction record            |
| Read      | View balance and account information |
| Update    | Update account balance               |
| Delete    | Not implemented intentionally        |

---

## Key Observation

One of the interesting observations during this project was that a banking system naturally relies more heavily on Create, Read, and Update operations than Delete operations.

This is because financial systems prioritize maintaining historical records and transaction transparency.
