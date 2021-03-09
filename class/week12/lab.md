# Lab 12

## Expectations

We are expecting you to commit your work often with useful commit messages.
This is helpful for you so that there are regular commits that demonstrate your progress. 
In case you forget to push your final commits before the deadline, at least you will get partial marks.

This means that you should commit and push your changes to the repository at least **FIVE** times as you work this lab (more is recommended).
Repositories that have very few commits will be flagged for careful scrutiny and review, and you will **definitely** lose marks for this! 

## Q1: [10 marks] Cuboid

Creates a class named `Cuboid` to represent cuboid objects and contains:

* Three double attributes `l`, `w`, and `h` specifying the length, width and height of the cuboid. 
* A String attribute `color` that specifies the color of the cuboid. 
* A constructor (with 4 arguments) that creates a cuboid with specified values. 
* A constructor (with no arguments) that sets `l`, `w`, and `h` to 1 and `color` to “white”. This constructor should invoke the 4-argument constructor using `this`. 
* Your program should have these methods:
  * Getter methods for all fields (e.g. `getColor()` which returns the color).
  * `getVolume()`: returns the cuboid volume which is 𝑙 * 𝑤 * h.
  * `getSurfaceArea()`: returns the surface area of the cuboid: 2(𝑙 * 𝑤 + 𝑙 * h + 𝑤 * h)
  * `displayInfo()`: displays on the screen the color, dimensions, surface area, and volume of this cuboid. 

### Test program

Write a test program that creates two objects of the Cuboid class — first object should have default values and the second object must be green of length 8, width 3.5, and height 5.9. Print the dimensions, color, surface area, and volume of each object as shown in the sample run below.

### Sample run:
```
Cuboid 1
  Color: White
  Dimentions: 1.00 X 1.00 X 1.00
  Surface Area: 6.00
  Volume: 1.00
Cuboid 2
  Color: Green
  Dimentions: 8.00 X 3.50 X 5.90
  Surface Area: 191.70
  Volume: 165.20
```

## Q2: [10 marks] Bank Accounts

Write a program that creates a class named BankAccount and contains:
* Private attributes:
  * `id(int)`,  `balance(double)`, and `annualInterestRate(double)`. 
  * `count(static int)` to keep a record of the number of created objects.
* Constructors:
  * A 2-argument constructor that creates an account with given `annualInterestRate` and `balance`, increments `count` by 1, and then stores the new `count` into `id`.
  * A no-argument constructor that invokes the above 2-arg constructor and sets both `balance` and `annualInterestRate` to 0. 
* Methods:
  * Getter methods for `balance`, `annualInterestRate`, and `id`.
  * Setter methods for `balance` and `annualInterestRate`.
  * `getMonthlyInterest()`: returns the monthly interest (not the interest rate). Monthly interest is `balance * annualInterestRate / 12`. Note that the interest rate is a percentage, e.g. 4.5%. You need to divide it by 100. 
  * `withdraw(double amount)`: withdraws a specified amount from the account.
  * `deposit(double amount)`: deposits a specified amount to the account.
  * `displayInfo()`: displays the information of a bank account as shown in the sample run below.
 
### Test Program

Write a test program that creates an object of `BankAccount` with a balance of $33,000, and an annual interest rate of 6.7%. Use withdraw to withdraw $1,500, use `deposit()` to deposit $1,000, then use `displayInfo()` to display the account information. 

### Sample run:
```
Account ID: 1
Current balance: 32500.0
Annual interest rate: 6.700%
Monthly interest rate: 0.558%
Monthly interest: $181.458
```

## Grading area

### Link to files

You do not have to do anything in this section.

[Q1 Java file](./Q1.java)

[Q2 Java file](./Q2.java)

Remember to commit all your changes and to submit the link to this repository on Canvas.
