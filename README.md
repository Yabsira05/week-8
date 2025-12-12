# week-8
In this lab, I wrote a C++ program that simulates a simple BankAccount.
: What my code does
Start a bank account
- Creates a BankAccount object with a starting balance of 0.
: Adds money (deposit)
- Uses a deposit(double amount) to add money to the balance.
- Prints a message like:
- Added starting balance of 100
: Makes purchases
- Uses makePurchase(string item, double cost) to “buy” items (for example, Coffee or Book).
- If there is enough money, it:
- subtracts the cost from the balance
- prints: Purchased Coffee
- saves the purchase in a file
- If there is not enough money, it prints:
- Insufficient funds for <item>
: Shows the final balance
- Uses displayBalance() to print the current balance, for example:
Current Balance: $70.5
: Saves transactions to a file
- Every deposit and purchase is written to a text file called transactions.txt.
- The file includes lines like:
Deposit: $100
Purchase - Coffee: $4.5
Purchase - Book: $25
How I built it
: To build this program, I first created a `BankAccount` class and gave it a `balance` variable to track the money in the account. After that, I added the key functions I needed: one to deposit money, one to make purchases (with a check for enough funds), one to display the current balance, and one that writes each deposit or purchase to transactions.txt.
Once the class was set up, I tested it in the main() function. I made an initial deposit, then called makePurchase a couple of times to simulate buying items like Coffee and a Book. Finally, I printed the balance and opened transactions.txt to confirm that every action in the program matched the transaction history saved in the file.
