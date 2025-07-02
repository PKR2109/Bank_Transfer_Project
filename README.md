#  Bank Transfer Transaction Project (MySQL + Python)

##  Description

This project demonstrates **safe money transfer logic** using `mysql.connector` in Python, implementing:

- Manual transaction handling
- Savepoint creation
- Rollback if failure occurs
- Full ACID-compliant logic

##  Project Structure

| File | Purpose |
|------|---------|
| `bank_transfer_transaction.py` | Main logic for transferring ₹500 between two accounts |
| `README.md` | Project description and usage guide |

##  MySQL Table Setup

Use this to create the database table:

```sql
CREATE TABLE accounts (
    account_id INT PRIMARY KEY,
    account_name VARCHAR(100),
    balance DECIMAL(10, 2)
);

INSERT INTO accounts (account_id, account_name, balance) VALUES
(1, 'Pavan Reddy', 10000),
(2, 'Rahul Kumar', 5000);
