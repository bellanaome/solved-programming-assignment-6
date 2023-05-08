Download Link: https://assignmentchef.com/product/solved-programming-assignment-6
<br>
5/5 - (2 votes)

Develop a polymorphic banking application using the Account hierarchy you created in Assignment #5. Create the following two SavingsAccount objects and two CheckingAccount objects and store them in an array called “arrays” of Account references to the objects:



Account NameAccount NumberInitial BalanceFee ChargedInterest Rate[your name]-Savings-111.000

4%[your name]-Savings-222.000

5%[your name]-Checking-133.0003.00

[your name]-Checking-244.0004.00

Using a “foreach” loop, iterate over each account in the array. For each Account in the array, first print the account. Next, allow the user to specify an amount of money to withdraw from the Account using method Debit and an amount of money to deposit into the Account using method Credit. Specifically, for each account, prompt the user to enter an amount to deposit in the account and call the Credit method. Print the object. Next, prompt the user to enter an amount to withdraw and call the Debit method. Print the object. After the user has made a deposit and a withdrawal from an account, calculate interest if the account is a SavingsAccount and print the object. To perform this step, you must first determine the object’s type. If the Account is a SavingsAccount, calculate the amount of interest owed to the Account using method CalculateInterest and print the account a final time. If the account is a CheckingAccount, you do not need to CalculateInterest nor print the account a final time.

Hint: To determine if an account is a savings or checking account, use the .getType method which returns a string representing the Name or FullName property. Then use the “.Equals” method to determine if the returned string is equal to the name of the class.For example:

acct.getType().Name returns the string “SavingsAccount” or “CheckingAccount”.Once you have determined that an account is a SavingsAccount object, you must “cast” the account object into a SavingsAccount object in order to access its CalculateInterest method. I like to perform this in two steps: declare a different variable to hold the reference to the object that has been cast from an Account object into a SavingsAccount object. Then, using this new variable, invoke its CalculateInterest method. For example, at the beginning of the Main() method, I declare a variable of type SavingsAccount as follows:

SavingsAccount temp_account;In my foreach loop, I have a variable called “acct” that is defined as an Account object. To downcast this Account object into a SavingsAccount object, I use the syntax: