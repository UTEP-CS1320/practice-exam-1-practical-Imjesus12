# Exam 1: Practical

This Practical Exam has three problems.

The first two problems are required, while the third is provided for extra credit.

These three problems are found inside an if statement, used to select each problem. Below you will find the description of what you have to do for each problem, as well as the grading rubric for each.

The `main.c` file contains code that can help you check each problem when you press the "Run" button.

Remember: you are allowed to check back on zyBooks in case you forgot how to do certain things.

**Make sure to comment and format your code!** Unclear code in the actual exam will be penalized.

For this practice exam I highly encourage you to discuss the exam with your fellow students and share ideas and code snippets on how to tackle each individual problem.

Just remember, on the actual exam **you must work on the code on your own. Your code must be your own original creation.** You are allowed to use external resources, such as zyBooks, to help remind you how certain things work, but otherwise your code must be as original as you can make it. *Copying someone else's code entirely is not going to help you truly learn anything*, in addition to being a potential case for Academic Dishonesty, which we treat very, *very* seriously in this course.

### Grade Breakdown

Problem | Points Possible
--------|----------------
P1: Last Digits | 25
P2: Lotto | 35
**Total** | 60
P3: Hex2Dec (Extra credit) | 10

## Problem 1: Last Digits

For this problem, you have to **fix existing code**.

This is the general algorithm of the code:

1. Take 2 integers as input (x and y)
2. Get the last two digits of x, and the last two digit of y
3. If the last two digits of x and the last two digits of y are the same, print out `TRUE`.
4. If they are not the same, print out `FALSE`

Inside `main.c` you will find code that does something that does not quite match the intended algorithm. You have to correct it, making sure it compiles, runs, and functions properly.

#### Grading Rubric

Rubric | Points
-------|--------
Code is clean, passes all automated tests | 25
Code is a little messy, fails some tests | 20
Code intention is clear, but does not compile | 10
No functional changes from original code | 0

## Problem 2: Lottery Number

This code is supposed to do a simple lottery matching:

1. User inputs a 4-digit lottery ticket.
2. If the ticket matches the 4 digits of the winning number, print out a message that reads `1st Prize!\n`.
2. If the ticket matches only 3 digits of the winning number, print out a message that reads `2nd Prize!\n`.
3. If the ticket matches only 2 digits of the winning number, print out a message that reads `3rd Prize!\n`.
4. In all other cases, print out a message that reads: `No Prize! Better luck next time!\n`

The digits have to match in both number and position. For example, if the winning number is `1234`, the lottery ticket `1534` would be a 2nd Prize winner, but the ticket `5134` would be a 3rd Prize winner. Ticket `3415` has all the digits but in a different position from the original, so it would be a losing ticket.

Your objective is to write code that checks the numbers and prints out the correct message. The existing code must not be changed and includes the winning ticket number, and code that takes the user's input.

Your code must be written after the line that reads `//TODO: Your P2 code goes here`. Make sure to comment your code to make clear what you intend to do with it!

Rubric | Points
-------|--------
Code is clean and well commented, passes all 5 automated tests | 35
Code is a little messy, fails some tests | 25
Code intention is clear, but does not compile | 15
Code is messy, uncommented, is far from complete | 5
No functional changes from original code | 0

## Problem 3: Hex2Dec (*Extra Credit*)

The numerical system that we are used to is called "decimal", as it uses 10 as its base: digits 0-9 are used to represent each digit, and each place in a string of digits represents a power of 10.

Computers use a *binary* system with two digits (0 and 1), in which each place in a string of digits represents a power of 2. For example, 100 in binary is the number 8 in decimal, because the 1 is on the third position (2^3 = 8).

Another system that is widely used is [Hexadecimal](https://simple.wikipedia.org/wiki/Hexadecimal). It represents numbers on a 16-number scale: the decimal digits 0-9, plus the letters A to F to represent the values 10 thru 15, respectively.

For this Extra Credit problem, you have to write code that reads a *four-character string*, representing a hexadecimal number, and prints out its decimal value. Your code should be able to ignore casing, meaning lowercase `f` and uppercase `F` should both return `15`. In case the input is not hexadecimal digit (Meaning: not a number, and not a letter in the A-F range), it should print out `ERROR`.

Your code must be written after the line that reads `//TODO: Your P3 code goes here`. Make sure to comment your code to make clear what you intend to do with it!

Rubric | Points
-------|--------
Code passes all 5 automated tests | 10
Code is a little messy, fails some tests | 2-8
No functional changes from original code | 0
