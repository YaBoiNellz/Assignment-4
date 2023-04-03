Name: Darnell Chambers Gordon

GitHub Username: YaBoiNellz

GitHub Repository: https://github.com/YaBoiNellz/Assignment-4.git

GitHub Pages Website: https://yaboinellz.github.io/my-react-app/

Group Members: None

Code May Give Issue when running on regular terminal the first time this command fixed the issue: export NODE_OPTIONS=--openssl-legacy-provider. There is a issue that was caused, it was caused by Node.js software when it upgraded from v16 to v18. It has nothing to nothing to do with my code. I tried many other solutions but the NODE_OPTIONS=--openssl-legacy-provider command was able to get it to work. once I added this command the code was working. The GitHub Pages Works just fine though the code is able to run on terminal after using the NODE_OPTIONS=--openssl-legacy-provider.

I solved the assignment by modifying three files: App.js, Credit.js, and Debit.js
App.js

1.	Added a new function named ‘addCredit’

-	This function takes in a credit object and adds it to the creditList state. The creditList state holds an array of all the credits made.
-	Additionally, this method calls the updateAccountBalance() method that updates the account balance once a credit is made.

2.	Added a new function  ‘addDebit’
-	This function takes in a debit object and adds it to the list of debits.
-	Similar to addCredit(), this method also calls the updateAccountBalance() method

3.	Added a new function ‘updateAccountBalance()’ that updates the account balance once a debit or credit is made.
4.	Implemented the componentDidMount() function that fetches sample data using axios from the given URLs and loads them to the credit and debit array states.

Credit.js
1.	Converted the component from functional to class component for easy state tracking.
2.	The class has two states, amount and description
3.	Improved the form appearance and accessibility
4.	Added an updateAmount() method to update the amount state as the user types
5.	Added an updateDescription() method to update the description state as the user types
6.	Added a function handleSubmit() that takes in credit data from user and adds it to the creditList record. Once the form has been submitted, a credit object is created and passed as a parameter to the addCredit() method.
7.	Created a generateId() method that generates an id from the last max id inserted
8.	Added a method creditsView() to display the previously inserted debit transactions

Debit.js
1.	Similar to the Credit component, I converted the component from functional to class component for easy state tracking.
2.	The class has two states, amount and description
3.	Improved the form appearance and accessibility
4.	Added an updateAmount() method to update the amount state as the user types
5.	Added an updateDescription() method to update the description state as the user types
6.	Added a function handleSubmit() that takes in credit data from user and adds it to the creditList record. Once the form has been submitted, a credit object is created and passed as a parameter to the addCredit() method.
7.	Created a generateId() method that generates an id from the last max id inserted
8.	Added a method debitsView() to display the previously inserted debit transactions


