## DO NOT OPEN UNTIL YOU HAVE FINISHED THE PRACTICE PROBLEMS!!!

## Answer Key: 01-Variables/

## Practice 1:

Create variables for:

The robot's name  
The number of motors  
Motor power  
Whether the claw is open

Choose an appropriate type for each variable.

-ANSWER-

May vary but should be along the lines of

```java
String robotName = "10830-Robot";
int numOfMotors = 4;
double motorPower = 1.0;
Boolean clawOpen = false;
```

## Practice 2

Predict the values before running the code:

```java
double drive = 0.6;
double turn = 0.2;

double leftPower = drive + turn;
double rightPower = drive - turn;
```

What are:

leftPower = ?  
rightPower = ?

-ANSWER-

```java
leftPower = 0.8;
rightPower = 0.4;
```

## Practice 3

What happens here?

```java
double power = 0.5;

power = 1.0;
power = 0.25;
```

What is the final value of power?

Explain why.

-ANSWER-

```java
power = 0.25;
```

```java
// reason: value of power has changed in code sequence from 0.5 -> 1.0 -> 0.25
```

## Practice 4

Find the problem:

```java
int motorPower = 0.5;
```

Why might Java reject this?

What type should be used instead?

-ANSWER-

```java
// Java may reject variable type because it is incorrect syntax
// must be a double or float to hold a decimal value
```

## Challenge

Without running the code, determine the final values:

```java
double power = 0.5;
double adjustment = 0.2;

power = power + adjustment;
adjustment = 0.1;
power = power - adjustment;
```

What is:

power = ?  
adjustment = ?

Explain each change in order.

-ANSWER-

```java
// First 0.5 + 0.2 = 0.7
// Second 0.7 - 0.1 = 0.6
// power = 0.6
// adjustment = 0.1
```
