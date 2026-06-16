# Project Learnings

Building this project helped bridge the gap between understanding programming concepts and applying them to a real-world scenario.

Rather than starting with code, the project began by understanding how a bank account works from a business perspective.

This approach made it easier to identify the information that needed to be stored and the operations that needed to be performed.

---

## Understanding Before Coding

One of the biggest takeaways from this project was that software development starts with problem understanding rather than code implementation.

Before writing any logic, it was necessary to answer questions such as:

* What information should a bank account store?
* What actions should a bank account perform?
* What validation rules should exist?
* What should happen during deposits and withdrawals?

Answering these questions provided a clear structure for the implementation.

---

## Thinking in Objects

This project reinforced the idea that Object-Oriented Programming is a way of modeling real-world entities.

A bank account naturally contains:

* Information
* Rules
* Actions

Representing these concepts within a single object creates a more organized and maintainable design.

---

## Importance of Encapsulation

One important observation was the need to protect sensitive information such as account balances.

Allowing unrestricted access to account data could lead to inconsistent states and invalid operations.

Encapsulation provides a controlled way to manage data modifications through approved methods.

---

## Validation as a Business Requirement

Validation is often viewed as a programming task, but this project highlighted that validation originates from business rules.

Examples include:

* Preventing negative deposits
* Preventing negative withdrawals
* Preventing withdrawals that exceed available balance

The code simply enforces rules that already exist in the real world.

---

## Relationship Between Business Logic and Code

Another key learning was that code is only an implementation of business logic.

For example:

```text
Deposit:
Current Balance + Deposit Amount

Withdrawal:
Current Balance - Withdrawal Amount
```

These rules exist independently of programming languages.

The role of software is to execute those rules consistently.

---

## CRUD in Real Scenarios

The project also demonstrated how CRUD operations appear naturally within business processes.

Creating transactions, reading account information, and updating balances occur frequently within banking systems.

Delete operations are intentionally limited because transaction history must be preserved for auditing purposes.

---

## Final Reflection

One of the most valuable outcomes of this project was understanding that programming is not primarily about writing code.

It is about understanding a problem, designing a solution, and then expressing that solution through code.

The banking system provided a practical example of how business requirements can be translated into structured software using Object-Oriented Programming principles.
