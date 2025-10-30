---
layout: satellite
title: "Exercise Solutions - Introduction to C Programming"
date: 2024-01-15
author: "Course Material"
categories: [Software-I, C Programming]
tags: [C programming, exercise solutions, programming practice]
---

# Exercise Solutions: Introduction to C Programming

## Multiple Choice Questions

### 1. Which of the following characters are used to comment in C?
a. \\b. /* */ c. % d. Both a and b

**Answer: d) Both a and b**

**Explanation:** C supports two types of comments:
- `//` - Single line comment  
- `/* */` - Multi-line comment

### 2. Which one of the following is a format specifier of char?
a. %d b. &l c. %c d. Both a and b

**Answer: c) %c**

**Explanation:** `%c` is the format specifier for character data type.

### 3. Which of the following functions is used to take inputs from users?
a. sprintf() b. printf() c. scanf() d. None of these

**Answer: c) scanf()**

**Explanation:** `scanf()` function is used to read input from the user.

### 4. Which one of the following is a format specifier of string?
a. %s b. &l c. %c d. Both a and b

**Answer: a) %s**

**Explanation:** `%s` is the format specifier for string data type.

### 5. Which one of the following is a format specifier of int?
a. %d b. &l c. %c d. Both a and b

**Answer: a) %d**

**Explanation:** `%d` is the format specifier for integer data type.

## Programming Questions

### 1. Write a program to take input of name, roll no and marks obtained by a student in 5 subjects. Each subject have 100 full marks. Display the name, roll no with percentage score secured.

**Solution:**
```c
#include <stdio.h>

int main() {
    char name[50];
    int rollNo;
    int marks[5];
    int totalMarks = 0;
    float percentage;
    
    printf("Enter student name: ");
    scanf("%s", name);
    
    printf("Enter roll number: ");
    scanf("%d", &rollNo);
    
    printf("Enter marks for 5 subjects (out of 100 each):\n");
    for(int i = 0; i < 5; i++) {
        printf("Subject %d: ", i+1);
        scanf("%d", &marks[i]);
        totalMarks += marks[i];
    }
    
    percentage = (float)totalMarks / 5.0;
    
    printf("\n--- Student Report ---\n");
    printf("Name: %s\n", name);
    printf("Roll No: %d\n", rollNo);
    printf("Total Marks: %d/500\n", totalMarks);
    printf("Percentage: %.2f%%\n", percentage);
    
    return 0;
}
```

### 2. Write a program to add two numbers (5&7) and display its sum.

**Solution:**
```c
#include <stdio.h>

int main() {
    int num1 = 5;
    int num2 = 7;
    int sum;
    
    sum = num1 + num2;
    
    printf("First number: %d\n", num1);
    printf("Second number: %d\n", num2);
    printf("Sum: %d + %d = %d\n", num1, num2, sum);
    
    return 0;
}
```

### 3. Write a program to input marks of 5 subjects (Physics, Chemistry, Math, English & Biology) for a student. Display the rank of each subjects and also the result of total marks and percentage obtained with his/her rank in the class. The rank is categorized as fail (marks < 40%), pass & third division (marks between 40 to 55%), second (marks between 55 to 65%), first (marks between 65 to 80%), Distinction (marks between 80 to 95%), extra ordinary (marks above 95 to 100%).

**Solution:**
```c
#include <stdio.h>

int main() {
    char subjects[5][20] = {"Physics", "Chemistry", "Math", "English", "Biology"};
    int marks[5];
    int totalMarks = 0;
    float percentage;
    
    printf("Enter marks for each subject (out of 100):\n");
    for(int i = 0; i < 5; i++) {
        printf("%s: ", subjects[i]);
        scanf("%d", &marks[i]);
        totalMarks += marks[i];
    }
    
    percentage = (float)totalMarks / 5.0;
    
    printf("\nSubject-wise Results:\n");
    for(int i = 0; i < 5; i++) {
        printf("%s: %d marks - ", subjects[i], marks[i]);
        if(marks[i] < 40) printf("Fail\n");
        else if(marks[i] >= 40 && marks[i] < 55) printf("Pass & Third Division\n");
        else if(marks[i] >= 55 && marks[i] < 65) printf("Second Division\n");
        else if(marks[i] >= 65 && marks[i] < 80) printf("First Division\n");
        else if(marks[i] >= 80 && marks[i] < 95) printf("Distinction\n");
        else printf("Extraordinary\n");
    }
    
    printf("\nOverall Performance:\n");
    printf("Total Marks: %d/500\n", totalMarks);
    printf("Percentage: %.2f%%\n", percentage);
    
    if(percentage < 40) printf("Result: FAIL\n");
    else if(percentage >= 40 && percentage < 55) printf("Result: PASS & THIRD DIVISION\n");
    else if(percentage >= 55 && percentage < 65) printf("Result: SECOND DIVISION\n");
    else if(percentage >= 65 && percentage < 80) printf("Result: FIRST DIVISION\n");
    else if(percentage >= 80 && percentage < 95) printf("Result: DISTINCTION\n");
    else printf("Result: EXTRAORDINARY\n");
    
    return 0;
}
```

### 4. Write a program to input two integer numbers and display the sum of even numbers between these two input numbers.

**Solution:**
```c
#include <stdio.h>

int main() {
    int num1, num2, start, end;
    int sum = 0;
    
    printf("Enter two integers: ");
    scanf("%d %d", &num1, &num2);
    
    if(num1 < num2) {
        start = num1;
        end = num2;
    } else {
        start = num2;
        end = num1;
    }
    
    printf("Even numbers between %d and %d: ", start, end);
    
    for(int i = start; i <= end; i++) {
        if(i % 2 == 0) {
            printf("%d ", i);
            sum += i;
        }
    }
    
    printf("\nSum of even numbers: %d\n", sum);
    
    return 0;
}
```

### 5. Write a program to add, subtract, multiply and divide two integers using user defined type function with return type.

**Solution:**
```c
#include <stdio.h>

int add(int a, int b);
int subtract(int a, int b);
int multiply(int a, int b);
float divide(int a, int b);

int main() {
    int num1, num2, choice;
    
    printf("Enter two integers: ");
    scanf("%d %d", &num1, &num2);
    
    do {
        printf("\n--- Calculator Menu ---\n");
        printf("1. Addition\n");
        printf("2. Subtraction\n");
        printf("3. Multiplication\n");
        printf("4. Division\n");
        printf("5. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);
        
        switch(choice) {
            case 1:
                printf("Result: %d + %d = %d\n", num1, num2, add(num1, num2));
                break;
            case 2:
                printf("Result: %d - %d = %d\n", num1, num2, subtract(num1, num2));
                break;
            case 3:
                printf("Result: %d * %d = %d\n", num1, num2, multiply(num1, num2));
                break;
            case 4:
                if(num2 != 0) {
                    printf("Result: %d / %d = %.2f\n", num1, num2, divide(num1, num2));
                } else {
                    printf("Error: Division by zero!\n");
                }
                break;
            case 5:
                printf("Goodbye!\n");
                break;
            default:
                printf("Invalid choice!\n");
        }
    } while(choice != 5);
    
    return 0;
}

int add(int a, int b) {
    return a + b;
}

int subtract(int a, int b) {
    return a - b;
}

int multiply(int a, int b) {
    return a * b;
}

float divide(int a, int b) {
    return (float)a / b;
}
```

### 6. Write a program to find separately the sum of the positive and negative integer elements of an array of size 10. Define a function called sortarray(int[]), pass the array to this function and display the array elements into ascending order.

**Solution:**
```c
#include <stdio.h>

void sortarray(int arr[]);
void displayArray(int arr[]);

int main() {
    int numbers[10];
    int positiveSum = 0, negativeSum = 0;
    
    printf("Enter 10 integers:\n");
    for(int i = 0; i < 10; i++) {
        printf("Number %d: ", i+1);
        scanf("%d", &numbers[i]);
        
        if(numbers[i] > 0) {
            positiveSum += numbers[i];
        } else if(numbers[i] < 0) {
            negativeSum += numbers[i];
        }
    }
    
    printf("\nOriginal array: ");
    displayArray(numbers);
    
    printf("Sum of positive numbers: %d\n", positiveSum);
    printf("Sum of negative numbers: %d\n", negativeSum);
    
    sortarray(numbers);
    
    printf("Sorted array (ascending): ");
    displayArray(numbers);
    
    return 0;
}

void sortarray(int arr[]) {
    for(int i = 0; i < 9; i++) {
        for(int j = 0; j < 9 - i; j++) {
            if(arr[j] > arr[j + 1]) {
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
}

void displayArray(int arr[]) {
    for(int i = 0; i < 10; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
}
```

### 7. Write a program to read a sentence and count the number of characters & words in that sentence.

**Solution:**
```c
#include <stdio.h>

int main() {
    char sentence[1000];
    int characters = 0, words = 0;
    int i = 0;
    int inWord = 0;
    
    printf("Enter a sentence: ");
    fgets(sentence, sizeof(sentence), stdin);
    
    while(sentence[i] != '\0' && sentence[i] != '\n') {
        characters++;
        
        if(sentence[i] == ' ' || sentence[i] == '\t') {
            inWord = 0;
        } else {
            if(inWord == 0) {
                words++;
                inWord = 1;
            }
        }
        i++;
    }
    
    printf("\nSentence Analysis:\n");
    printf("Total characters: %d\n", characters);
    printf("Total words: %d\n", words);
    
    return 0;
}
```

---

*These solutions cover the fundamental C programming concepts as outlined in the course syllabus.*