# Lesson 4: Control Statements in C

Control statements in C are used to control the flow of the program. There are two types of control statements in C:

1. Decision Making Statements:
- If Statement: The if statement is used to execute a block of code only if the specified condition is true. Syntax:

```c
if (condition) {
    // code to be executed if the condition is true
}

```
- If-else Statement: The if-else statement is used to execute one block of code if the condition is true and another block of code if the condition is false. Syntax:

```c
if (condition) {
    // code to be executed if the condition is true
} else {
    // code to be executed if the condition is false
}

```

- Nested If Statement: The nested if statement is used when we want to check multiple conditions. Syntax:
vbnet

```c
if (condition1) {
    // code to be executed if condition1 is true
    if (condition2) {
        // code to be executed if condition2 is also true
    }
}

```
- Switch Statement: The switch statement is used when we have multiple cases to check. Syntax:
java
```c
switch (expression) {
    case value1:
        // code to be executed if expression is equal to value1
        break;
    case value2:
        // code to be executed if expression is equal to value2
        break;
    ...
    default:
        // code to be executed if none of the above cases are true
}

```
## Looping Statements:
- While Loop: The while loop is used to execute a block of code repeatedly as long as the specified condition is true. Syntax:
javascript
```c
while (condition) {
    // code to be executed
}

```
- Do-while Loop: The do-while loop is used to execute a block of code at least once and then repeatedly as long as the specified condition is true. Syntax:
javascript

```c
do {
    // code to be executed
} while (condition);
For Loop: The for loop is used to execute a block of code repeatedly for a specified number of times. Syntax:
css
Copy code
for (initialization; condition; increment/decrement) {
    // code to be executed
}

```
These control statements are essential for making decisions and controlling the flow of the program. Understanding how to use them is an important step in becoming proficient in C programming.
