---
layout: satellite
title: "Extra Questions - Introduction to C Programming"
date: 2024-01-15
author: "Course Material"
categories: [Software-I, C Programming]
tags: [C programming, extra questions, programming practice]
---

# Extra Questions: Introduction to C Programming

## Part A: Multiple Choice Questions

### 1. Which of the following is NOT a valid data type in C?
a) int
b) float
c) char
d) string

### 2. What is the correct way to include a header file in C?
a) include <stdio.h>
b) #include stdio.h
c) #include <stdio.h>
d) include stdio.h

### 3. Which operator has the highest precedence among arithmetic operators?
a) +
b) -
c) *
d) /

### 4. What will be the output of: `printf("%d", 5 % 2);`?
a) 2
b) 1
c) 0
d) Error

### 5. Which loop is best when the number of iterations is known?
a) while loop
b) do-while loop
c) for loop
d) All are same

### 6. What is the default case in a switch statement called?
a) default
b) else
c) otherwise
d) case default

### 7. Which function is used to read a string input in C?
a) scanf()
b) gets()
c) fgets()
d) All of the above

### 8. What is the starting index of an array in C?
a) 1
b) 0
c) -1
d) Depends on declaration

### 9. Which symbol is used to terminate a string in C?
a) \n
b) \0
c) \t
d) \r

### 10. What happens if you don't return a value from a function that expects one?
a) Compilation error
b) Runtime error
c) Garbage value returned
d) 0 is returned

### 11. Which of the following correctly declares an array of 10 integers?
a) int arr[10];
b) int arr(10);
c) int arr{10};
d) array int arr[10];

### 12. What is the result of: `10 > 5 && 3 < 2`?
a) 1
b) 0
c) True
d) False

### 13. Which assignment operator is used for adding a value to a variable?
a) =+
b) +=
c) =-
d) -=

### 14. What is the purpose of `break` statement in a loop?
a) Skip current iteration
b) Exit the loop
c) Restart the loop
d) Pause the loop

### 15. Which format specifier is used for floating-point numbers?
a) %d
b) %f
c) %c
d) %s

## Part B: Programming Questions

### 16. **Basic Arithmetic Calculator**
Write a program that takes two numbers and performs all four arithmetic operations (+, -, *, /) and displays the results.

### 17. **Grade Classification**
Create a program that inputs a student's marks and displays the grade:
- A: 90-100
- B: 80-89
- C: 70-79
- D: 60-69
- F: Below 60

### 18. **Sum of Natural Numbers**
Write a program to find the sum of first n natural numbers using:
a) for loop
b) while loop
c) do-while loop

### 19. **Factorial Calculator**
Create a program to calculate factorial of a number using:
a) Iterative approach
b) Function-based approach

### 20. **Number Pattern**
Write a program to print the following pattern:
```
*
**
***
****
*****
```

### 21. **Array Maximum and Minimum**
Write a program that finds the largest and smallest elements in an array of integers.

### 22. **String Operations**
Create a program that:
- Counts the length of a string manually (without strlen)
- Reverses a string
- Counts vowels in a string

### 23. **Menu-Driven Calculator**
Develop a calculator program with a menu that allows users to:
- Add two numbers
- Subtract two numbers
- Multiply two numbers
- Divide two numbers
- Exit

### 24. **Prime Number Checker**
Write a program to check if a given number is prime or not. Also, find all prime numbers between 1 and n.

### 25. **Simple Interest Calculator**
Create a program that calculates simple interest using the formula:
SI = (P * R * T) / 100
Where P = Principal, R = Rate, T = Time

### 26. **Even-Odd Array Separation**
Write a program that separates even and odd numbers from an array into two different arrays.

### 27. **Digit Counter**
Create a program that counts the number of digits in a given integer.

### 28. **Reverse Number**
Write a program to reverse the digits of a number. For example: 1234 becomes 4321.

### 29. **ASCII Value Display**
Create a program that displays the ASCII values of characters 'A' to 'Z' and 'a' to 'z'.

### 30. **Area Calculator Functions**
Write functions to calculate:
- Area of circle
- Area of rectangle
- Area of triangle
Use a menu to let users choose which area to calculate.

## Part C: Practical Applications

### 31. **Student Report Card**
Create a program that:
- Stores information for 5 students (name, roll no, 3 subject marks)
- Calculates total and percentage for each student
- Displays a complete report card
- Finds the class average

### 32. **Simple Banking System**
Develop a basic banking program that:
- Creates an account with initial balance
- Allows deposits and withdrawals
- Displays current balance
- Maintains transaction history (last 5 transactions)

### 33. **Employee Salary Calculator**
Write a program to calculate employee salary with:
- Basic salary input
- HRA = 10% of basic
- DA = 8% of basic
- Gross salary = Basic + HRA + DA
- Tax = 5% of gross (if gross > 10000)
- Net salary = Gross - Tax

### 34. **Library Book Management**
Create a simple library system that:
- Stores book information (title, author, book ID)
- Allows adding new books
- Searches for books by title or author
- Displays all available books

### 35. **Temperature Monitoring System**
Simulate a temperature monitoring system that:
- Reads temperature values for a week
- Calculates average temperature
- Finds highest and lowest temperatures
- Displays temperature trend

### 36. **Marksheet Generator**
Design a program that:
- Inputs student details and marks for 5 subjects
- Calculates total, percentage, and grade
- Determines pass/fail status
- Generates a formatted marksheet

### 37. **Simple Inventory System**
Create an inventory management program that:
- Maintains product details (name, quantity, price)
- Allows adding new products
- Updates product quantities
- Calculates total inventory value

### 38. **Voting System**
Develop a simple voting program that:
- Registers candidates
- Records votes
- Counts votes for each candidate
- Declares the winner

### 39. **Expense Tracker**
Build an expense tracking system that:
- Records daily expenses with categories
- Calculates total expenses
- Shows expense breakdown by category
- Provides weekly/monthly summaries

### 40. **Quiz System**
Create a multiple-choice quiz program that:
- Stores questions and answers
- Presents questions to users
- Calculates and displays the score
- Provides feedback on performance

## Answer Key

### Multiple Choice Questions:
1. d) string
2. c) #include <stdio.h>
3. c) *
4. b) 1
5. c) for loop
6. a) default
7. d) All of the above
8. b) 0
9. b) \0
10. c) Garbage value returned
11. a) int arr[10];
12. b) 0
13. b) +=
14. b) Exit the loop
15. b) %f

## Programming Tips

### For Beginners:
1. Always include proper header files
2. Use meaningful variable names
3. Add comments to explain logic
4. Test programs with different inputs
5. Handle invalid inputs gracefully

### Best Practices:
1. Initialize variables before use
2. Check array bounds
3. Use functions to avoid code repetition
4. Format output clearly
5. Follow consistent coding style

### Common Mistakes to Avoid:
1. Forgetting semicolons
2. Using = instead of == in conditions
3. Array index out of bounds
4. Infinite loops
5. Not handling division by zero

---

*These questions focus on the fundamental C programming concepts covered in Chapter 5, helping students practice essential skills for IoT development.*