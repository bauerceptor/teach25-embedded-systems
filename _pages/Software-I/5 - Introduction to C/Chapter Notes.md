---
title: "Chapter Notes - C Programming"
date: "2025-10-25"
thumbnail: "/assets/img/thumbnail/book.jpg"
bookmark: true
---

# Chapter Notes: Introduction to C Programming

## 1. Introduction to C Programming

### What is C?
C is a **general-purpose, procedural programming language** that provides:
- **Easy to learn** - Simple syntax and structure
- **Structured programming** - Organized code with functions
- **Efficient programs** - Fast execution
- **Low-level access** - Direct hardware control
- **Portability** - Runs on many platforms

### Why Learn C?
- **Foundation language** - Base for many other languages
- **System programming** - Operating systems, embedded systems
- **IoT development** - Microcontroller programming
- **Performance** - Fast execution for resource-constrained devices
- **Industry standard** - Widely used in professional development

## 2. C Program Structure

### Basic Program Components
Every C program consists of:

```c
#include <stdio.h>    // Preprocessor commands

int main() {          // Main function
    // Your code here
    printf("Hello World!\n");
    return 0;
}
```

**Key Parts:**
- **Header files** (`#include`) - Include necessary libraries
- **main() function** - Program execution starts here
- **Statements** - Instructions to execute
- **Comments** - Documentation (ignored by compiler)

### Program Development Cycle
1. **Write source code** (.c file)
2. **Compile** - Convert to machine language
3. **Link** - Combine with libraries
4. **Execute** - Run the program

## 3. Data Types

### Essential Data Types
Focus on these fundamental types:

| Type | Purpose | Example |
|------|---------|---------|
| `int` | Whole numbers | `int age = 25;` |
| `float` | Decimal numbers | `float price = 99.99;` |
| `char` | Single characters | `char grade = 'A';` |

### Variable Declaration
```c
int count;           // Declaration
count = 10;          // Assignment
int total = 50;      // Declaration + initialization
```

## 4. Input and Output

### Basic I/O Functions

**printf() - Output**
```c
printf("Hello World\n");
printf("Age: %d\n", age);
printf("Price: %.2f\n", price);
```

**scanf() - Input**
```c
int number;
printf("Enter a number: ");
scanf("%d", &number);
```

### Format Specifiers
| Specifier | Data Type |
|-----------|-----------|
| `%d` | int |
| `%f` | float |
| `%c` | char |
| `%s` | string |

## 5. Operators

### Arithmetic Operators
```c
int a = 10, b = 3;
int sum = a + b;      // Addition: 13
int diff = a - b;     // Subtraction: 7
int product = a * b;  // Multiplication: 30
int quotient = a / b; // Division: 3
int remainder = a % b; // Modulus: 1
```

### Assignment Operators
```c
int x = 5;
x += 3;    // x = x + 3 (now x is 8)
x -= 2;    // x = x - 2 (now x is 6)
x *= 2;    // x = x * 2 (now x is 12)
```

### Comparison Operators
```c
if (a == b)  // Equal to
if (a != b)  // Not equal to
if (a > b)   // Greater than
if (a < b)   // Less than
if (a >= b)  // Greater than or equal
if (a <= b)  // Less than or equal
```

### Logical Operators
```c
if (age >= 18 && hasLicense)     // AND
if (day == 6 || day == 7)        // OR
if (!(isRaining))                // NOT
```

## 6. Control Structures

### If-Else Statements
```c
if (score >= 90) {
    printf("Grade A\n");
} else if (score >= 80) {
    printf("Grade B\n");
} else {
    printf("Grade C\n");
}
```

### Switch Statement
```c
switch (choice) {
    case 1:
        printf("Option 1 selected\n");
        break;
    case 2:
        printf("Option 2 selected\n");
        break;
    default:
        printf("Invalid choice\n");
}
```

### Loops

**While Loop**
```c
int i = 1;
while (i <= 5) {
    printf("%d ", i);
    i++;
}
```

**For Loop**
```c
for (int i = 1; i <= 5; i++) {
    printf("%d ", i);
}
```

**Do-While Loop**
```c
int num;
do {
    printf("Enter positive number: ");
    scanf("%d", &num);
} while (num <= 0);
```

## 7. Functions

### Function Basics
Functions help organize code and avoid repetition.

**Function Definition:**
```c
int add(int a, int b) {
    int sum = a + b;
    return sum;
}
```

**Function Call:**
```c
int result = add(5, 3);
printf("Sum: %d\n", result);
```

### Function Components
- **Return type** - What the function gives back
- **Function name** - What you call it
- **Parameters** - Input values
- **Function body** - The actual code

### Example: Calculator Function
```c
float calculate(float num1, float num2, char operation) {
    switch (operation) {
        case '+': return num1 + num2;
        case '-': return num1 - num2;
        case '*': return num1 * num2;
        case '/': return num1 / num2;
        default: return 0;
    }
}
```

## 8. Arrays

### Array Basics
Arrays store multiple values of the same type.

**Declaration and Initialization:**
```c
int numbers[5];                    // Declaration
int scores[5] = {85, 92, 78, 96, 88}; // Initialization
```

**Accessing Elements:**
```c
scores[0] = 90;        // Set first element
int first = scores[0]; // Get first element
```

### Working with Arrays
```c
// Print all elements
for (int i = 0; i < 5; i++) {
    printf("Score %d: %d\n", i+1, scores[i]);
}

// Find maximum
int max = scores[0];
for (int i = 1; i < 5; i++) {
    if (scores[i] > max) {
        max = scores[i];
    }
}
```

## 9. Strings

### String Basics
Strings are arrays of characters ending with '\0'.

**Declaration:**
```c
char name[20];
char greeting[] = "Hello";
```

**String Input/Output:**
```c
printf("Enter your name: ");
scanf("%s", name);
printf("Hello, %s!\n", name);
```

### String Example
```c
char message[] = "Programming";
printf("Message: %s\n", message);
printf("First character: %c\n", message[0]);
```

## 10. Common Programming Patterns

### Input Validation
```c
int num;
do {
    printf("Enter a number between 1-10: ");
    scanf("%d", &num);
    if (num < 1 || num > 10) {
        printf("Invalid input! Try again.\n");
    }
} while (num < 1 || num > 10);
```

### Menu System
```c
int choice;
do {
    printf("\n1. Add\n2. Subtract\n3. Exit\n");
    printf("Enter choice: ");
    scanf("%d", &choice);
    
    switch (choice) {
        case 1:
            // Add operation
            break;
        case 2:
            // Subtract operation
            break;
        case 3:
            printf("Goodbye!\n");
            break;
        default:
            printf("Invalid choice!\n");
    }
} while (choice != 3);
```

### Array Processing
```c
// Calculate average
float sum = 0;
for (int i = 0; i < size; i++) {
    sum += array[i];
}
float average = sum / size;
```

## 11. Best Practices

### Code Organization
1. **Use meaningful variable names**
   ```c
   int student_count;    // Good
   int x;               // Bad
   ```

2. **Add comments for clarity**
   ```c
   // Calculate total marks
   int total = 0;
   for (int i = 0; i < 5; i++) {
       total += marks[i];
   }
   ```

3. **Use proper indentation**
   ```c
   if (condition) {
       statement1;
       statement2;
   }
   ```

### Error Prevention
1. **Initialize variables**
   ```c
   int count = 0;  // Good
   int sum = 0;
   ```

2. **Check array bounds**
   ```c
   if (index >= 0 && index < array_size) {
       array[index] = value;
   }
   ```

3. **Validate input**
   ```c
   if (scanf("%d", &number) != 1) {
       printf("Invalid input!\n");
   }
   ```

## 12. Common Mistakes to Avoid

1. **Forgetting semicolons**
   ```c
   int x = 5;  // Don't forget the semicolon
   ```

2. **Array index out of bounds**
   ```c
   int arr[5];
   arr[5] = 10;  // Error! Index 5 doesn't exist
   ```

3. **Uninitialized variables**
   ```c
   int sum = 0;  // Always initialize
   ```

4. **Infinite loops**
   ```c
   for (int i = 0; i < 10; i++) {  // Make sure i increases
       printf("%d\n", i);
   }
   ```

## 13. Problem-Solving Approach

### Step-by-Step Method
1. **Understand the problem** - What is required?
2. **Plan the solution** - Break into smaller steps
3. **Write pseudocode** - Plan the logic
4. **Code the solution** - Implement in C
5. **Test the program** - Verify with different inputs

### Example: Find Largest Number
```c
#include <stdio.h>

int main() {
    int numbers[5];
    int largest;
    
    // Input numbers
    printf("Enter 5 numbers:\n");
    for (int i = 0; i < 5; i++) {
        printf("Number %d: ", i+1);
        scanf("%d", &numbers[i]);
    }
    
    // Find largest
    largest = numbers[0];
    for (int i = 1; i < 5; i++) {
        if (numbers[i] > largest) {
            largest = numbers[i];
        }
    }
    
    printf("Largest number: %d\n", largest);
    return 0;
}
```

## 14. IoT Applications

### Microcontroller Programming
C is essential for:
- **Sensor data reading**
- **Motor control**
- **Communication protocols**
- **Real-time processing**

### Example: Temperature Monitor
```c
// Simplified IoT temperature monitoring
int read_temperature() {
    // Read from temperature sensor
    return temperature_value;
}

void check_temperature() {
    int temp = read_temperature();
    
    if (temp > 30) {
        printf("Temperature high: %d°C\n", temp);
        // Turn on cooling system
    } else if (temp < 15) {
        printf("Temperature low: %d°C\n", temp);
        // Turn on heating system
    }
}
```

## Key Takeaways

1. **C is fundamental** - Essential for system and IoT programming
2. **Practice is crucial** - Write lots of small programs
3. **Understand concepts** - Focus on logic over memorization
4. **Start simple** - Build complexity gradually
5. **Debug systematically** - Use printf to trace execution
6. **Plan before coding** - Think through the problem first

---

*This chapter provides the foundation for C programming essential for IoT and embedded systems development. Focus on understanding concepts and practicing with real programs.*