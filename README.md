# Lesson_20
# Primary application file
Integrating crypto_wallet.py and fintech_finder.py files will automate the tasks associated with generating a digital wallet, accessing Ethereum account balances, and signing and sending transactions via a personal Ethereum blockchain called Ganache.

Specifically, as the perspective of a Fintech Finder customer in order to do the following:

Generate a new Ethereum account instance by using the mnemonic seed phrase provided by Ganache.

Fetch and display the account balance associated with your Ethereum account address.

Calculate the total value of an Ethereum transaction, including the gas estimate, that pays a Fintech Finder candidate for their work.

Digitally sign a transaction that pays a Fintech Finder candidate, and send this transaction to the Ganache blockchain.

Review the transaction hash code associated with the validated blockchain transaction.



---

## Technologies

The following Technologies were used to develop this program:

Python 
    Version 3.9.7

Terminal
    Version 2.12.5 (444)

Visual Studio Code
    Version: 1.66.2 (Universal)
    Commit: dfd34e8260c270da74b5c2d86d61aee4b6d56977
    Date: 2022-04-11T07:49:20.994Z
    Electron: 17.2.0
    Chromium: 98.0.4758.109
    Node.js: 16.13.0
    V8: 9.8.177.11-electron.0
    OS: Darwin x64 21.4.0
    
---

## General information about analysis.
There are three parts to this Lesson:

### Import Ethereum Transaction Functions into the Fintech Finder Application:

In the first part you will review the code contained in the crypto_wallet.py file.  You have modules built through Lesson 19 already incorporated into starting files.  After that you add you mnemonic seed phrase from Ganache into your .env file.

After that go into the fintech_finder.py file and import the functions from crypto_wallet.py file for:

generate_account

get_balance

send_transaction

Then using the Streamlit sidebar section of code, create a variable named account. Set this variable equal to a call on the generate_account function. This function will create the Fintech Finder customer’s (in this case, your) HD wallet and Ethereum account.

The last step in this part using same section of the fintech_finder.py file, define a new st.sidebar.write function that will display the balance of the customer’s account. Inside this function, call the get_balance function and pass it your Ethereum account.address.



### Sign and Execute a Payment Transaction:

For this section you'll write the code that will calculate a fintech professional’s wage, in ether, based on the worker’s hourly rate and the number of hours that they work for a customer. 

Then write code that uses the calculated wage value to send a transaction that pays the worker. This code should allow the Fintech Finder customer to authorize the transaction with their digital signature. For the purpose of testing out this application, you will use your own Ethereum account information as the customer account information.


### Inspect the Transaction

Now it's time to put it all together and test the Fintech Finder application with your newly integrated Ethereum wallet. You will send a test transaction by using the application’s web interface, and then look up the resulting transaction in Ganache.

First you need to launch the streamlit application.  Then hire a candidate using the drop down menu and number of hours for the candidate selected and click the send transaction button.

Including a screen shotshoot of address balance and history from Ganache:


![balances](/Account_balances_Ganache.png)

You can see the balance was reduced from the first line and increased on the second line with the transaction completed.

Transaction history:

![history](transaction_history.png)

Screenshot of showing recipient's balance:

![Rbalance](Increase_client_acct.png)

Also showing receipient's history:

![history](transaction_history.png)

---

## Information about datasets

List of candidates and attributes:

candidate_database

people

db_list

candidate 

hourly_rate 

candidate_address

Generate account:

account

Wage calculation:

wage

Calling send_transaction for account, candidate_address and wage:

transaction_hash

---

## Libraries used in analysis

Streamlit

dataclass

typing

web3

w3

generate_account

get_balance

send_transaction

---

## Contributors


**Chris Miskovich**

Contact Information:

Email: cmiskovich@verizon.net

[LinkedIn](https://www.linkedin.com/in/christopher-miskovich-9a61b0234/) 

---

## License

[MIT](/license.txt)
