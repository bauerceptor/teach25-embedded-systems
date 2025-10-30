---
title: "Extra Questions - C Programming"
date: "2025-10-28"
thumbnail: "/assets/img/thumbnail/sample.png"
bookmark: true
---

# Extra Questions: Introduction to C Programming

## Programming Questions

### 1. **Basic Arithmetic Calculator**

Write a program that takes two numbers and performs all four arithmetic operations (+, -, *, /) and displays the results.

**Solution:**

```c
#include <stdio.h>

int main() {
    float num1, num2;
    
    printf("Enter two numbers: ");
    scanf("%f %f", &num1, &num2);
    
    printf("Addition: %.2f + %.2f = %.2f\n", num1, num2, num1 + num2);
    printf("Subtraction: %.2f - %.2f = %.2f\n", num1, num2, num1 - num2);
    printf("Multiplication: %.2f * %.2f = %.2f\n", num1, num2, num1 * num2);
    
    if (num2 != 0) {
        printf("Division: %.2f / %.2f = %.2f\n", num1, num2, num1 / num2);
    } else {
        printf("Division by zero is not allowed!\n");
    }
    
    return 0;
}
```

### 2. **Grade Classification**

Create a program that inputs a student's marks and displays the grade:

- A: 90-100
- B: 80-89
- C: 70-79
- D: 60-69
- F: Below 60

**Solution:**

```c
#include <stdio.h>

int main() {
    int marks;
    
    printf("Enter student marks (0-100): ");
    scanf("%d", &marks);
    
    if (marks < 0 || marks > 100) {
        printf("Invalid marks! Please enter marks between 0 and 100.\n");
    } else if (marks >= 90) {
        printf("Grade: A\n");
    } else if (marks >= 80) {
        printf("Grade: B\n");
    } else if (marks >= 70) {
        printf("Grade: C\n");
    } else if (marks >= 60) {
        printf("Grade: D\n");
    } else {
        printf("Grade: F\n");
    }
    
    return 0;
}
```

### 3. **Sum of Natural Numbers**

Write a program to find the sum of first n natural numbers using:
a) for loop
b) while loop
c) do-while loop

**Solution:**

```c
#include <stdio.h>

int main() {
    int n, sum;
    
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    
    if (n <= 0) {
        printf("Please enter a positive integer.\n");
        return 1;
    }
    
    // Using for loop
    sum = 0;
    for (int i = 1; i <= n; i++) {
        sum += i;
    }
    printf("Sum using for loop: %d\n", sum);
    
    // Using while loop
    sum = 0;
    int i = 1;
    while (i <= n) {
        sum += i;
        i++;
    }
    printf("Sum using while loop: %d\n", sum);
    
    // Using do-while loop
    sum = 0;
    i = 1;
    do {
        sum += i;
        i++;
    } while (i <= n);
    printf("Sum using do-while loop: %d\n", sum);
    
    return 0;
}
```

### 4. **Factorial Calculator**

Create a program to calculate factorial of a number using:
a) Iterative approach
b) Function-based approach

**Solution:**

```c
#include <stdio.h>

// Function to calculate factorial
long long factorial(int n) {
    long long fact = 1;
    for (int i = 1; i <= n; i++) {
        fact *= i;
    }
    return fact;
}

int main() {
    int n;
    
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    
    if (n < 0) {
        printf("Factorial is not defined for negative numbers.\n");
        return 1;
    }
    
    // Iterative approach
    long long fact = 1;
    for (int i = 1; i <= n; i++) {
        fact *= i;
    }
    printf("Factorial using iterative approach: %d! = %lld\n", n, fact);
    
    // Function-based approach
    printf("Factorial using function: %d! = %lld\n", n, factorial(n));
    
    return 0;
}
```

### 5. **Number Pattern**

Write a program to print the following pattern:

```bash
*
**
***
****
*****
```

**Solution:**

```c
#include <stdio.h>

int main() {
    int rows;
    
    printf("Enter number of rows: ");
    scanf("%d", &rows);
    
    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }
    
    return 0;
}
```

### 6. **Array Maximum and Minimum**

Write a program that finds the largest and smallest elements in an array of integers.

**Solution:**

```c
#include <stdio.h>

int main() {
    int n;
    
    printf("Enter the size of array: ");
    scanf("%d", &n);
    
    int arr[n];
    
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        printf("Element %d: ", i + 1);
        scanf("%d", &arr[i]);
    }
    
    int max = arr[0];
    int min = arr[0];
    
    for (int i = 1; i < n; i++) {
        if (arr[i] > max) {
            max = arr[i];
        }
        if (arr[i] < min) {
            min = arr[i];
        }
    }
    
    printf("Largest element: %d\n", max);
    printf("Smallest element: %d\n", min);
    
    return 0;
}
```

### 7. **String Operations**

Create a program that:

- Counts the length of a string manually (without strlen)
- Reverses a string
- Counts vowels in a string

**Solution:**

```c
#include <stdio.h>

int main() {
    char str[100];
    char reversed[100];
    int length = 0, vowels = 0;
    
    printf("Enter a string: ");
    scanf("%s", str);
    
    // Count length manually
    while (str[length] != '\0') {
        length++;
    }
    printf("Length of string: %d\n", length);
    
    // Reverse the string
    for (int i = 0; i < length; i++) {
        reversed[i] = str[length - 1 - i];
    }
    reversed[length] = '\0';
    printf("Reversed string: %s\n", reversed);
    
    // Count vowels
    for (int i = 0; i < length; i++) {
        char ch = str[i];
        if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
            ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
            vowels++;
        }
    }
    printf("Number of vowels: %d\n", vowels);
    
    return 0;
}
```

### 8. **Menu-Driven Calculator**

Develop a calculator program with a menu that allows users to:

- Add two numbers
- Subtract two numbers
- Multiply two numbers
- Divide two numbers
- Exit

**Solution:**

```c
#include <stdio.h>

int main() {
    int choice;
    float num1, num2, result;
    
    do {
        printf("\n=== Calculator Menu ===\n");
        printf("1. Addition\n");
        printf("2. Subtraction\n");
        printf("3. Multiplication\n");
        printf("4. Division\n");
        printf("5. Exit\n");
        printf("Enter your choice (1-5): ");
        scanf("%d", &choice);
        
        if (choice >= 1 && choice <= 4) {
            printf("Enter two numbers: ");
            scanf("%f %f", &num1, &num2);
        }
        
        switch (choice) {
            case 1:
                result = num1 + num2;
                printf("Result: %.2f + %.2f = %.2f\n", num1, num2, result);
                break;
                
            case 2:
                result = num1 - num2;
                printf("Result: %.2f - %.2f = %.2f\n", num1, num2, result);
                break;
                
            case 3:
                result = num1 * num2;
                printf("Result: %.2f * %.2f = %.2f\n", num1, num2, result);
                break;
                
            case 4:
                if (num2 != 0) {
                    result = num1 / num2;
                    printf("Result: %.2f / %.2f = %.2f\n", num1, num2, result);
                } else {
                    printf("Error: Division by zero!\n");
                }
                break;
                
            case 5:
                printf("Thank you for using the calculator!\n");
                break;
                
            default:
                printf("Invalid choice! Please try again.\n");
        }
    } while (choice != 5);
    
    return 0;
}
```

### 9. **Prime Number Checker**

Write a program to check if a given number is prime or not. Also, find all prime numbers between 1 and n.

**Solution:**

```c
#include <stdio.h>

int isPrime(int num) {
    if (num <= 1) {
        return 0; // Not prime
    }
    
    for (int i = 2; i * i <= num; i++) {
        if (num % i == 0) {
            return 0; // Not prime
        }
    }
    return 1; // Prime
}

int main() {
    int n, num;
    
    printf("Enter a number to check if it's prime: ");
    scanf("%d", &num);
    
    if (isPrime(num)) {
        printf("%d is a prime number.\n", num);
    } else {
        printf("%d is not a prime number.\n", num);
    }
    
    printf("\nEnter a number to find all primes up to that number: ");
    scanf("%d", &n);
    
    printf("Prime numbers between 1 and %d are:\n", n);
    for (int i = 2; i <= n; i++) {
        if (isPrime(i)) {
            printf("%d ", i);
        }
    }
    printf("\n");
    
    return 0;
}
```

### 10. **Even-Odd Array Separation**

Write a program that separates even and odd numbers from an array into two different arrays.

**Solution:**

```c
#include <stdio.h>

int main() {
    int n;
    
    printf("Enter the size of array: ");
    scanf("%d", &n);
    
    int arr[n], even[n], odd[n];
    int evenCount = 0, oddCount = 0;
    
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        printf("Element %d: ", i + 1);
        scanf("%d", &arr[i]);
        
        if (arr[i] % 2 == 0) {
            even[evenCount] = arr[i];
            evenCount++;
        } else {
            odd[oddCount] = arr[i];
            oddCount++;
        }
    }
    
    printf("\nOriginal array: ");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    
    printf("\nEven numbers: ");
    for (int i = 0; i < evenCount; i++) {
        printf("%d ", even[i]);
    }
    
    printf("\nOdd numbers: ");
    for (int i = 0; i < oddCount; i++) {
        printf("%d ", odd[i]);
    }
    printf("\n");
    
    return 0;
}
```

### 11. **Digit Counter**

Create a program that counts the number of digits in a given integer.

**Solution:**

```c
#include <stdio.h>

int main() {
    int num, count = 0;
    int original;
    
    printf("Enter an integer: ");
    scanf("%d", &num);
    
    original = num;
    
    // Handle special case for 0
    if (num == 0) {
        count = 1;
    } else {
        // Make number positive for counting
        if (num < 0) {
            num = -num;
        }
        
        while (num > 0) {
            count++;
            num /= 10;
        }
    }
    
    printf("Number of digits in %d: %d\n", original, count);
    
    return 0;
}
```

### 12. **Reverse Number**

Write a program to reverse the digits of a number. For example: 1234 becomes 4321.

**Solution:**

```c
#include <stdio.h>

int main() {
    int num, reversed = 0, remainder;
    int original;
    
    printf("Enter an integer: ");
    scanf("%d", &num);
    
    original = num;
    
    // Handle negative numbers
    int isNegative = 0;
    if (num < 0) {
        isNegative = 1;
        num = -num;
    }
    
    while (num != 0) {
        remainder = num % 10;
        reversed = reversed * 10 + remainder;
        num /= 10;
    }
    
    if (isNegative) {
        reversed = -reversed;
    }
    
    printf("Original number: %d\n", original);
    printf("Reversed number: %d\n", reversed);
    
    return 0;
}
```

### 13. **ASCII Value Display**

Create a program that displays the ASCII values of characters 'A' to 'Z' and 'a' to 'z'.

**Solution:**

```c
#include <stdio.h>

int main() {
    char ch;
    
    printf("ASCII values of uppercase letters (A-Z):\n");
    for (ch = 'A'; ch <= 'Z'; ch++) {
        printf("%c = %d\n", ch, ch);
    }
    
    printf("\nASCII values of lowercase letters (a-z):\n");
    for (ch = 'a'; ch <= 'z'; ch++) {
        printf("%c = %d\n", ch, ch);
    }
    
    printf("\nEnter a character to find its ASCII value: ");
    scanf(" %c", &ch);
    printf("ASCII value of '%c' is %d\n", ch, ch);
    
    return 0;
}
```

### 14. **Area Calculator Functions**

Write functions to calculate:

- Area of circle
- Area of rectangle
- Area of triangle
Use a menu to let users choose which area to calculate.

**Solution:**

```c
#include <stdio.h>
#define PI 3.14159

float circleArea(float radius) {
    return PI * radius * radius;
}

float rectangleArea(float length, float width) {
    return length * width;
}

float triangleArea(float base, float height) {
    return 0.5 * base * height;
}

int main() {
    int choice;
    float radius, length, width, base, height;
    
    do {
        printf("\n=== Area Calculator ===\n");
        printf("1. Circle Area\n");
        printf("2. Rectangle Area\n");
        printf("3. Triangle Area\n");
        printf("4. Exit\n");
        printf("Enter your choice (1-4): ");
        scanf("%d", &choice);
        
        switch (choice) {
            case 1:
                printf("Enter radius of circle: ");
                scanf("%f", &radius);
                printf("Area of circle: %.2f\n", circleArea(radius));
                break;
                
            case 2:
                printf("Enter length and width of rectangle: ");
                scanf("%f %f", &length, &width);
                printf("Area of rectangle: %.2f\n", rectangleArea(length, width));
                break;
                
            case 3:
                printf("Enter base and height of triangle: ");
                scanf("%f %f", &base, &height);
                printf("Area of triangle: %.2f\n", triangleArea(base, height));
                break;
                
            case 4:
                printf("Thank you for using the area calculator!\n");
                break;
                
            default:
                printf("Invalid choice! Please try again.\n");
        }
    } while (choice != 4);
    
    return 0;
}
```

---

*These questions focus on the fundamental C programming concepts covered in Chapter 5, helping students practice essential skills for IoT development.*
