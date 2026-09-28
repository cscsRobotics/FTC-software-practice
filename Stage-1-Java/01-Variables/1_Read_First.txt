# Stage 1: Java
## 01 - Variables

### Goal

Learn what variables are, how to create them, and how to use them in a program.

---

## 1. What is a variable?

A variable is a named place in the program that stores a value.

For example:

```java
double motorPower = 0.5;

motor.setPower(motorPower);

instead 

motor.setPower(0.5);

## 2. Variables have types

-int: Stores whole numbers

int motors = 4;
int targetPosition = 1000;

-double: Stores numbers that can have decimals

double power = 0.5;
double speed = 0.75;

-Boolean: stores either true or false

boolean clawOpen = true;
boolean robotReady = false;

-string: stores text

String robotName = "BioBuzz";

-long: stores numbers that exceed standard capacity of 'int'

long worldPopulation = 8100000000L;
System.out.println("The world population is: " + worldPopulation);

## 3. Creating and Changing Variables

You can create a variable:

double power = 0.5;

Then change its value:

power = 1.0;

The variable is still called power, but its value is now 1.0.

## 4. Using variables in calculations

Variables can be used in calculations.

double drive = 0.5;
double turn = 0.2;

double leftPower = drive + turn;
double rightPower = drive - turn;

The values become:

leftPower  = 0.7
rightPower = 0.3

The variables don't just store information. They can be used as part of the program's logic.


