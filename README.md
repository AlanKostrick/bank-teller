# Bank Teller

## Objective

Design an `Account` class that will perform capabilities of a single Bank Account, a `Bank` class that will house multiple accounts and a `BankingApp` (with a `main` method) to simulate a user interface where you can access your accounts and perform banking transactions.

### Tasks

Inside of `Account` Class program the following:
- 3 instance variables to handle `String accountNum`, `String type`, and `double balance`
- note the `accountNum` will be a unique identifier
- create the `Constructor` that handles the 3 pieces of instance data in the order mentioned above
- create the following methods: appropriate accessor methods and behavior methods needed for bank transactions


Inside of the `Bank` Class complete the following:
- Create a `list` called `accounts`
- `public void showAllAccounts` to display all accounts (use an enhanced for loop to iterate over the collection)
- A method to add a Bank Account 
- A  method to get access a particular account by `accountNum`
- A  method to `close` a particular account by `accountNum`

Hint: Think of what a Bank does...it houses many bank accounts...that is why this class is created to "maintain" the collection

Inside of the `BankingApp` Class program the following:
- A `Bank` object called `myBank`
- A `BankAccount` object called `account1` with the following properties `("1111","Checking",500.00)`
- A `BankAccount` object called `account2` with the following properties `("2222","Savings",2500.00)`
- Have `myBank` `add` the 2 accounts to the collection
- Set up a user interface to give similar output to the console:
  
### Sample Output

- There is flexibility here, feel free to design your user interface to have the functionality your desire 

```
Here are your accounts at our bank:
Checking 500.0
Savings 100.0

What would you like to do?
Press 1 to deposit
Press 2 to withdrawal
Press 3 to check balance
Press 4 to close an account
Press -1 to exit
1
You want to deposit.
Here are your accounts
(1111) Checking 500.0
(2222) Savings 100.0
Select the account by (acct num) to perform this transaction.
1111
You have selected 1111
Enter the amount to deposit:
2000
Your updated balance is now 2500.0

What would you like to do?
Press 1 to deposit
Press 2 to withdrawal
Press 3 to check balance
Press 4 to close an account
Press -1 to exit
4
You would like to close an account.
Here are your accounts
(1111) Checking 2500.0
(2222) Savings 100.0
Enter the account number of the account you would like to close:
2222
You are closing account # 2222
Here are your remaining accounts
(1111) Checking 2500.0

What would you like to do?
Press 1 to deposit
Press 2 to withdrawal
Press 3 to check balance
Press 4 to close an account
Press -1 to exit
```

## Stretch Tasks
- Use the NumberFormat class to format your money 
- Add an option to be able to transfer funds between accounts
- Build in functionality so that one cannot withdrawal more than what is in an account
- Password protect your accounts
