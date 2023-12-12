This Node API, built with Fastify and Knex, aims to register transactions for personal financial control. Through it, the user can create a transaction, list all transactions, access their summary (credit - debit), and search for a specific transaction

# Functional Requirements

- [x] The user must be able to create a new transaction.
- [x] The user must be able to get a summary of their account.
- [x] The user must be able to list all past transactions.
- [x] The user must be able to view a single transaction.

# Business Rules
- [x] Transactions can be of the credit type, which will add to the total value, or debit type, which will subtract.
- [x] It should be possible to identify the user across requests.
- [x] The user can only view transactions that they have created.
