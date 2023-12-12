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


<h1>Getting Started:</h1>
To utilize our application, follow these simple steps:


# 1. Clone the Repository:
Begin by cloning our application's repository to your local machine:
``
git clone https://github.com/pedro4r/api-rest-node
``

## 2. Install Dependencies:
Navigate to the cloned directory and install the necessary dependencies using npm:
``
npm install
``

## 3. Start the Development Environment:
After the installation is complete, start the development environment with:
``
npm run dev
``

This command will launch the Storybook environment, allowing you to view and interact with our project.


To use the application in production, I recommend using Insomnia with the following routes:

#### Creating new transaction:
- **POST** Method 
- URL: `https://node-rest-api-ev6k.onrender.com/transactions`
- Body: 
    ```json
    {
        "title": "Freelancer job",
        "amount": 4000,
        "type": "credit"
    }
    ```

#### List transactions
- **GET** Method 
- URL: `https://node-rest-api-ev6k.onrender.com/transactions`

#### List specific transaction
- **GET** Method 
- URL: `https://node-rest-api-ev6k.onrender.com/transactions/transaction_ID`

#### Show Summary of transactions
- **GET** Method 
- URL: `https://node-rest-api-ev6k.onrender.com/transactions/summary`

