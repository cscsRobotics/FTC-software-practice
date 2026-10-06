# Stage 1: Java
## 02 - Conditionals

### Goal

Learn how to make a program choose what to do based on a condition.

---

## 1. What is a conditional?

A conditional allows your program to make a decision.

The basic structure is:

```java
if (condition) {
    // code runs if the condition is true
}

//For example:

if (gamepad1.a) {
    claw.setPosition(1.0);
}

//The code inside the { } runs when gamepad1.a is true.
```

## 2. if/else

You can give the program two possible actions:
```java
if (gamepad1.a) {
    claw.setPosition(1.0);
} else {
    claw.setPosition(0.0);
}
```
If A is pressed:

claw → 1.0

If A is not pressed:

claw → 0.0

Only one of the two blocks runs each time the conditional is evaluated.

## 3. else if

You can check multiple conditions:
```java
if (gamepad1.a) {
    claw.setPosition(1.0);
} else if (gamepad1.b) {
    claw.setPosition(0.0);
} else {
    // Neither button is pressed
}
```
The program checks the conditions from top to bottom.

It runs the first condition that is true.

## 4. comparison operators

Conditionals can compare values.
```java
Equal to
==

Example:

if (power == 1.0) {
    // code
}

Not equal to
!=

Greater than
>

Less than
<

Greater than or equal to
>=

Less than or equal to
<=
```
## Important: = vs ==

These are different:
```java
power = 1.0;
```
means:

Set power equal to 1.0.

But:
```java
power == 1.0
```
means:

Check whether power is equal to 1.0.
